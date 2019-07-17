# Rook-Ceph

Original Release: https://github.com/rook/rook/releases/tag/v1.0.4

## GKE固有の設定

- FlexVolumeのPathが普通じゃない。

```
        - name: FLEXVOLUME_DIR_PATH
          value: "/home/kubernetes/flexvolume"
```

- ノードプールのデフォルトOS(cos)だとRBD Kernel Moduleが使えないので、Ubuntuを選択する必要がある。
