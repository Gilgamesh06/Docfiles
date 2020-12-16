---

<p align="center">
	<a href="https://twitter.com/Gilgamesh_06">
		<img src="/Images/icono.png" alt="twitter" width="80%" height="80%"/>
	</a>
</p>

---

# MyConfiguracion

**Mi configuracion de bspwm y polybar.**

<p align="center">
  <img src="/Images/muestra.jpeg" alt="Polybar">
</p>

---

## Clonan el repositorio

```
$ cd ~
$ git clone https://github.com/Gilgamesh06/Docfiles.git
```

---

## Instalacion de los temas.

```
$ cd ~/Docfiles/ 
$ mv ~/Docfiles/Juno-ocean /usr/share/themes/
$ mv ~/Docfiles/Simply-Blue-Circles /usr/share/icons
```

---

## Administrar temas

<p>
	Para ello primero instalarelos: lxappearance
</p>

### Debian o derivados 

```
$ sudo apt-get install lxappearance
```

### Fedora 

```
$ sudo dnf install lxappearance
```

---

## Rofi 

**Instalacion**

### Debian o derivados 

```
$ sudo apt-get install rofi
```

### Fedora 

```
$ sudo dnf install rofi
```

---

## Compton

**Instalacion**

### Debian o derivados 

```
$ sudo apt-get install compton
```

### Fedora 

```
$ sudo dnf install compton
```
### Archivo de configuracion

```
$ mv ~/Docfiles/compton  ~/.config
```

---

## Feh

**Instalacion**

### Debian o derivados 

```
$ sudo apt-get install feh
```

### Fedora 

```
$ sudo dnf install feh
```

---

## Polybar 

## Dependencias 

### Debian o derivados 

```
$ apt install build-essential git cmake cmake-data pkg-config python3-sphinx libcairo2-dev libxcb1-dev libxcb-util0-dev libxcb-randr0-dev libxcb-composite0-dev python3-xcbgen xcb-proto libxcb-image0-dev libxcb-ewmh-dev libxcb-icccm4-dev

```
```
$ apt install libxcb-xkb-dev libxcb-xrm-dev libxcb-cursor-dev libasound2-dev libpulse-dev i3-wm libjsoncpp-dev libmpdclient-dev libcurl4-openssl-dev libnl-genl-3-dev

```

### Fedora 


```
$ sudo dnf install -y cairo-devel xcb-util-devel libxcb-devel xcb-proto xcb-util-image-devel xcb-util-wm-devel
```
```
$ sudo dnf install -y xcb-util-xrm-devel xcb-util-cursor-devel alsa-lib-devel pulseaudio-libs-devel i3-ipc jsoncpp-devel libmpdclient-devel libcurl-devel wireless-tools-devel libnl3-devel

```

---

## Instalacion polybar 


<p>
	Si su distro tiene paquete no tiene que instalarlo manualmente
	consulte : https://github.com/polybar/polybar
</p>

<p>
	Descarge el archivo .tar de : https://github.com/polybar/polybar/releases 
</p>


``` 
$ tar -xzvf "el archivo descargado con extencion"
```
```
$ mkdir build
$ cd build
$ cmake ..
$ make -j$(nproc)
$ sudo make install
```
### Tema polybar

**Fuentes tema polybar**

```
$ ~/Docfiles/hacks-fonts ~/usr/share/fonts
```
```
$ mv ~/Docfiles/polybar  ~/.config
```

---

## Bspwm

**Instalacion**

### Debian derivados


```
$ sudo apt-get install bspwm
```

### Fedora

```
$ sudo dnf install bspwm

```

---

## Dependencias 

### Debian o derivados 

```
$ sudo apt-get install libxcb-xinerama0-dev libxcb-icccm4-dev libxcb-randr0-dev libxcb-util0-dev libxcb-ewmh-dev libxcb-keysyms1-dev libxcb-shape0-dev 
```

---

## Instalacion

```
$ git clone https://github.com/baskerville/bspwm.git
$ git clone https://github.com/baskerville/sxhkd.git
$ cd bspwm && make && sudo make install
$ cd ../sxhkd && make && sudo make install
```

### config bspwm


```
$ mkdir -p ~/.config/{bspwm,sxhkd}
$ mv ~/Docfiles/bspwmrc  ~/.config/bspwm
$ mv ~/Docfiles/sxhkdrc  ~/.config/sxhkd
$ chmod u+x ~/.config/bspwm/bspwmrc
```

**Fondo de pantalla**

*Si desea cambiarlo edite la **linea 6** del archivo config de que esta en la carpeta `~/.config/bspwm`*

**Terminal**

la terminal por default es tilix si desea puede cambiarla modifique la **Linea 7** 

Si desea instalar **tilix.** 

### Debian o derivados

```
$ sudo apt-get install tilix
```
### Fedora

```
$ sudo dnf install tilix
```

La terminal utiliza el tema wild cherry del script gogh : https://github.com/Mayccoll/Gogh
la cual utiliza zsh y el tema bira del script : https://github.com/ohmybash/oh-my-bash
y la fuente menlo 

**Font terminal**

```
$ ~/Docfiles/Menlo for Powerline.ttf ~/usr/share/fonts
```

---                                                                        