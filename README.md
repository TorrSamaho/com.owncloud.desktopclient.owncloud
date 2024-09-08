# Install prerequisites
```
flatpak install --user flathub org.kde.Platform//6.7 org.kde.Sdk//6.7 io.qt.qtwebengine.BaseApp//6.7 flathub org.flatpak.Builder
```

# Build and install (using the flatpak version of flatpak-builder)
```
flatpak run org.flatpak.Builder --disable-rofiles-fuse --force-clean build-dir com.owncloud.desktopclient.owncloud.yml
flatpak run org.flatpak.Builder --user --install --force-clean build-dir com.owncloud.desktopclient.owncloud.yml
```
