# Offline runtime exported from the validated image in offline-manifest.json.
# No remote image, Dockerfile frontend, apt or pip is needed for this build.
FROM scratch
ADD rootfs.tar.gz /
ENV PATH="/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin"
ENV LANG="C.UTF-8"
ENV GPG_KEY="7169605F62C751356D054A26A821E680E5FA6305"
ENV PYTHON_VERSION="3.12.14"
ENV PYTHON_SHA256="5c8462af5790baf43a321a1559dbe0db06d1be4300fb85fb53c40060668e548a"
ENV PYTHONUNBUFFERED="1"
WORKDIR /app
CMD ["python", "-m", "app.main"]
