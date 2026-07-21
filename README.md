# Informarx Connect

Remote desktop solution baseada em RustDesk, personalizada para a Informarx.

## Download

Baixe a versão mais recente na [página de Releases](https://github.com/danileeraa/informarx-connect/releases).

### Windows

1. Baixe o arquivo `informarx-connect.exe` e `sciter.dll` da release
2. Coloque ambos na mesma pasta
3. Execute `informarx-connect.exe --install` para instalar como serviço (opcional)
4. Ou apenas execute `informarx-connect.exe` para uso avulso (portable mode)

> **Nota**: O `sciter.dll` é necessário para a interface gráfica. Mantenha-o sempre junto do executável.

## Build manual

```sh
git clone https://github.com/danileeraa/informarx-connect
cd informarx-connect
cargo build --release --features inline
```

O binário estará em `target/release/informarx-connect.exe`.

Execute `python res/inline-sciter.py` antes do build se quiser recursos UI embutidos.

## Licença

Baseado em [RustDesk](https://github.com/rustdesk/rustdesk), licenciado sob AGPL-3.0.
