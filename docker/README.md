QTCI Docker Images
===============

Setup

```
npm install
npm run docker_image_build
npm run docker_container_build
npm run docker_container_start
```

Install and Use Specific Qt version
```
npm use:qt5.9.2
```

```
npm run shell
```

Configuration
=====

Mount your own directory

```
npm config set qtci:docker_container_build_args "-v HOST_DIR:DOCKER_DIR"
npm run docker_container_build
```

Change Docker Image name
```
npm config set qtci:docker_image new_name
npm run docker_image_build
```

Change Docker Container Name

```
npm config set qtci:docker_container new_name
npm run docker_container_build
```
