```bash
sudo apt update && sudo apt install -y \
    build-essential \
    libncurses-dev \
    bison \
    flex \
    libssl-dev \
    libelf-dev \
    bc \
    cpio \
    wget \
    xorriso \
    grub-pc-bin \
    grub-efi-amd64-bin \
    grub-common \
    mtools \
    squashfs-tools \
    qemu-system-x86 \
    tar
```

| <div align="center">Pacote</div> | <div align="center">Propósito</div> |
| :--- | :--- |
| `build-essential` | GCC (compilador C), make, binutils |
| `libncurses-dev` | Desenha a tela azul do `menuconfig` |
| `bison` | Parser generator exigido pelo build do kernel |
| `flex` | Lexer generator exigido pelo build do kernel |
| `libssl-dev` | Criptografia para assinatura de módulos do kernel |
| `libelf-dev` | Manipulação de binários ELF | 
| `bc` | Calculadora usada pelo Makefile do kernel | 
| `cpio` | Empacota o initramfs no formato do kernel | 
| `wget` | Baixa arquivos da internet (código-fonte, BusyBox) |
| `xorriso` | Gera a imagem ISO bootável | 34 |
| `grub-pc-bin` | Binários do GRUB para boot BIOS (Legacy/MBR) | 
| `grub-efi-amd64-bin` | Binários do GRUB para boot UEFI | 
| `grub-common` | Ferramentas compartilhadas do GRUB (grub-mkrescue) | 
| `mtools` | Manipula imagens FAT (necessário para ISO UEFI) | 
| `squashfs-tools` | Cria o filesystem compactado SquashFS (mksquashfs) |
| `qemu-system-x86` | Emulador de PC completo para testar a ISO sem reiniciar |

- make allnoconfig
- make tinyconfig
- make localmodconfig
