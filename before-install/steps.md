# Antes de borrar todo el sistema

## limpiar la carpeta de Downloads y Documents

se tiene que seleccionar los archivos utiles y hacer un backup o hacer push de los repos, al final despues de que lo importante este seguro limpiar las carpeta

## backup de dotfiles

existe un comando `config` que en realidad es un alias de git

mas info aqui:

- https://www.atlassian.com/git/tutorials/dotfiles
- https://www.ackama.com/what-we-think/the-best-way-to-store-your-dotfiles-a-bare-git-repository-explained/

no ejecutar `config add .` directamente

### backup de dconf

```sh
dconf dump / > dconf-backup.conf
config add dconf-backup.conf
```

### paso final

```sh
config push origin master
```

##
