* Based on [https://github.com/rstudio/rstudio/pull/1921/files](https://github.com/rstudio/rstudio/pull/1921/files)
	* `flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo`
	* `flatpak install flathub io.qt.qtwebkit.BaseApp`
	* `flatpak install flathub org.kde.Sdk 5.9`
	* `flatpak install flathub org.freedesktop.Sdk.Extension.gfortran-62`
	* `flatpak install flathub org.freedesktop.Sdk.Extension.openjdk9`
	* `flatpak-builder --force-clean --ccache --repo=rstudio-repo rstudio-build com.rstudio.RStudio.json`
	* `flatpak remote-add --no-gpg-verify rstudio-repo rstudio-repo`
	* `flatpak install rstudio-repo com.rstudio.RStudio`
	* `flatpak run com.rstudio.RStudio`

* Updated with [https://github.com/Alexander-Wilms/flathub/tree/rstudio](https://github.com/Alexander-Wilms/flathub/tree/rstudio)
