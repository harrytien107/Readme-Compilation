# Docker

## Cài đặt setup Docker trên windows

Cài đặt file [Docker Desktop Installer.exe](https://www.docker.com/)

Ngay đây có 2 cách để cài đặt:

**1. Cài đặt trực tiếp**

- Chỉ cần double click vào file `Docker Desktop Installer.exe` và theo dõi quá trình cài đặt!

**2. Cài đặt qua `command prompt` bạn có thể thay đổi đường dẫn thư mục cài đặt Docker Desktop**

Bước 1: Mở `command prompt` dưới quyền admin

Bước 2: Dán câu lệnh dưới đây vào `command prompt`

```bash
start /w "" "Docker Desktop Installer.exe" install -accept-license --installation-dir="E:\Docker" --wsl-default-data-root="E:\Docker\wsl" --windows-containers-default-data-root="E:\\Docker"
```

_Lưu ý:_

1. `Command prompt` mở lên là đang trỏ `C:\Users\{username}` thì bạn cần lưu file `Docker Desktop Installer.exe` trong `C:\Users\{username}\Downloads` và trong `command prompt` thì cd vào `C:\Users\{username}\Downloads` và dán câu lệnh trên vào!

```bash
cd .\Downloads
```

2. Bạn có thể thay đổi đường dẫn thư mục đúng với máy của mình (ở trên là đường dẫn thư mục máy của `Glass`)

## Các container hay dùng

### MySQL

Down Image:

```bash
docker pull mysql:8.0.42-debian
```

Run Container:

```bash
docker run --name MySQL -p 3306:3306 -e MYSQL_ROOT_PASSWORD=123 mysql:8.0.42-debian
```

### SQL Server

Down Image:

```bash
docker pull mcr.microsoft.com/mssql/server:2019-latest
```

Run Container:

```bash
docker run -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=P@ssw0rd" -p 1433:1433 --name SQLServer2019 --hostname SQLServer2019 -v sqlvolume:/var/opt/mssql -d mcr.microsoft.com/mssql/server:2019-latest
```

### Postgres

Down Image:

```bash
docker pull postgres:16.0-alpine
```

Run Container:

```bash
docker run --name Postgres -p 5432:5432 -e POSTGRES_PASSWORD=123 -d postgres:16.0-alpine
```