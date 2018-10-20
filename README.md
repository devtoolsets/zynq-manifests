# INIT & SYNC
```bash
repo init -u ${MANIFEST_URI} -m manifest.xml --repo-url=${MIRROR_URI}
repo sync
```

## example:

```bash
    repo init -u git@gitlab.com:sections/yocto-manifest.git -m manifest.xml \
        --repo-url=https://mirrors.tuna.tsinghua.edu.cn/git/git-repo --no-clone-bundle
    repo sync -c --no-clone-bundle -j $(nproc)
```

