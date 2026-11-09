# WDA Multiplay — Samsung Tizen

Canal público de pacotes e atualizações do WDA Multiplay para Samsung TV.

**[Versões e downloads](https://github.com/navygod/WDA-MultiPlay-Tizen-Releases/releases/latest)**

Na página da versão, abra **Assets**. A release 0.0.41 contém:

- `WDA-Multiplay-0.0.41.tpk`: aplicativo com relógio de Brasília (HH:mm:ss) ao lado do nome no painel de botões.
- `WDA-Atualizacoes-0.1.3.wgt`: componente de atualização com retorno ao WDA pelo botão Voltar.
- `stable.json`: manifesto assinado consultado pela TV.
- `SHA256SUMS.txt`: hashes dos pacotes.

O código-fonte é mantido em repositório privado. Este canal distribui pacotes
Samsung assinados, o manifesto assinado `stable.json`, checksums e notas de versão.
O canal Android é independente.

## Atualizar na TV

A preparação inicial instala o aplicativo `.tpk` e o componente
`WDA-Atualizacoes-0.1.3.wgt`, mantendo a identidade do aplicativo existente.
São pacotes de desenvolvimento: a TV precisa estar autorizada no certificado
Samsung utilizado para assiná-los. Não há confirmação de compatibilidade geral
nem publicação na loja Samsung.

Para as próximas atualizações, mantenha Developer Mode ativo, configure **Host PC
IP = 127.0.0.1** e reinicie a TV. Abra **WDA Multiplay → Atualizações → Verificar →
Atualizar**. O componente baixa o pacote público, verifica assinatura e SHA-256 e
solicita a instalação local. Não usa conta GitHub nem guarda senha ou token.

O componente 0.1.0 da release 0.0.37 falhou no teste de instalação. A 0.1.1 usa
o comando Samsung `vd_appinstall` e o protocolo SDB SYNC. Esses mesmos módulos
confirmaram uma instalação assistida na TV. Em 01/11/2026, o proprietário também
confirmou a atualização **0.0.37 → 0.0.38 pela própria TV**, com o atualizador 0.1.1
e Host PC IP = 127.0.0.1, sem computador na instalação.

Base de desenvolvimento: Samsung QN50Q60DAGXZD, Tizen 9.0, firmware
T-NKLDUABC-0090-2123.9. A validação física citada se limita a esse aparelho e
firmware. O teste de root temporário foi confirmado nesse aparelho; o atualizador
publicado usa o canal local de instalação do Developer Mode.

Esses arquivos atualizam o aplicativo WDA, sem substituir o firmware da TV.
