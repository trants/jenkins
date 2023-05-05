<p align="center">
	<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e3/Jenkins_logo_with_title.svg/640px-Jenkins_logo_with_title.svg.png">
</p>

This project comes as a pre-built docker image that enables you to easily forward to your Jenkins websites running at home or otherwise, without having to know too much about setup Jenkins.

## Features

- Easy Installation. Jenkins is a platform-agnostic, self-contained Java-based program, ready to run with packages for Windows, Mac OS, and Unix-like operating systems.
- Easy configuration.
- Available plugins.
- Easy distribution.

## Quick Setup

1. Install Docker and Docker-Compose

- [Docker Install documentation](https://docs.docker.com/install/)
- [Docker-Compose Install documentation](https://docs.docker.com/compose/install/)

2. Bring up your stack by running

```bash
docker-compose up -d
```

3. Log in to the UI

- When your docker container is running, connect to it on port `8080` for the admin interface. Sometimes this can take a little bit because of the entropy of keys.

- [http://127.0.0.1:8080(http://127.0.0.1:8080)

4. Get default admin user:
```bash
docker exec <container_name> cat /var/jenkins_home/secrets/initialAdminPassword
```
- Immediately after logging in with this default user you will be asked to modify your details and change your password.

## Security

If you discover any security related issues, please email info@walruship.com instead of using the issue tracker.

## License

This software is released under the [BSD 3-Clause][link-license] License. Please see the [LICENSE](LICENSE) file or https://walruship.com/LICENSE.txt for more information.

[link-license]:   https://opensource.org/license/bsd-3-clause/