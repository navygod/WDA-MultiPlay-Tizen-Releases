# WDA Multiplay — Samsung Tizen

Canal público de pacotes e atualizações do WDA Multiplay para Samsung TV.

**[Versões e downloads](https://github.com/navygod/WDA-MultiPlay-Tizen-Releases/releases/latest)**

O código-fonte é mantido em repositório privado. Este canal distribui pacotes
Samsung assinados, o manifesto assinado `stable.json`, checksums e notas de versão.
O canal Android é independente.

## Atualizar na TV

A preparação inicial instala o aplicativo `.tpk` e o componente
`WDA-Atualizacoes-0.1.0.wgt`, mantendo a identidade do aplicativo existente.
São pacotes de desenvolvimento: a TV precisa estar autorizada no certificado
Samsung utilizado para assiná-los. Não há confirmação de compatibilidade geral
nem publicação na loja Samsung.

Para as próximas atualizações, mantenha Developer Mode ativo, configure **Host PC
IP = 127.0.0.1** e reinicie a TV. Abra **WDA Multiplay → Atualizações → Verificar →
Atualizar**. O componente baixa o pacote público, verifica assinatura e SHA-256 e
solicita a instalação local. Não usa conta GitHub nem guarda senha ou token.

Base de desenvolvimento: Samsung QN50Q60DAGXZD, Tizen 9.0, firmware
T-NKLDUABC-0090-2123.9. O fluxo autônomo completo ainda depende de validação
física. O teste de root temporário foi confirmado nesse aparelho; o atualizador
publicado usa o canal local de instalação do Developer Mode.

Esses arquivos atualizam o aplicativo WDA, sem substituir o firmware da TV.
