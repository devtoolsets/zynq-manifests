# INIT & SYNC
```bash
repo init -u ${MANIFEST_URI} -m manifest.xml --repo-url=${MIRROR_URI}
repo sync
```

## e.g.
```bash
    repo init -u git@gitlab.com:sections/zynq-manifests.git
```

```bash
    repo init -u git@gitlab.com:sections/zynq-manifests.git -b master -m manifest-v2023.1.xml \
        --repo-url=https://mirrors.tuna.tsinghua.edu.cn/git/git-repo --no-clone-bundle
```

sync
```bash

    repo sync -c --no-clone-bundle -j $(nproc)
```

