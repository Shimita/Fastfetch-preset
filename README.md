🌸 Fastfetch-preset

Un preset para Fastfetch con información de hardware, software y uso de recursos

---

🛠️ Requirements

- Atención: sólo ha sido probado en Linux Mint 22.3
- - A Brainware
- A Hardware
- Linux
- Terminal
- Package manager:
  - pacman (Arch / CachyOS / Manjaro / Garuda / etc)
  - apt (Debian / Ubuntu / Kali / etc)
  - dnf (Fedora / etc)
  - zypper
  - xbps-install
  - apk
  - nix-env

---

🚀 Instalación
```

Como el preset muestra información de la generación de los módulos RAM, y
para ver esa información se necesita ser superusuario, la estategia es usar un 
script que lea la información al inicio y lo guarde en un archivo de lectura.
La ejecución automática es controlado por un archivo de servicio

1. Copiar el script fastfetchMemory en /usr/local/bin/fastfetchMemory
2. Copiar el archivo de configuración de servicio en /etc/systemd/system/fastfetchMemory.service
3. Activarlo con sudo systemctl start fastfetchMemory.service y 
sudo systemctl enable fastfetchMemory.service
> 4. Mover la configuración de fastfetch en ~/.config/fastfetch/config.jsonc

```
