---
title: Privacy Policy - WA Automation Bridge
---

# Política de Privacidade — WA Automation Bridge

*Última atualização: 20 de outubro de 2026*

O WA Automation Bridge é uma extensão do Google Chrome que conecta o WhatsApp Web, aberto no seu navegador, a uma plataforma de automação escolhida e configurada por você (por exemplo, n8n, Make, Zapier ou um webhook próprio). Esta política explica quais dados a extensão trata, para onde eles vão e como você os controla.

## Resumo

- A extensão envia dados **somente para os endereços que você configura** nas opções (URL do webhook, URL da fila de comandos e origens de mídia permitidas).
- O desenvolvedor da extensão **não recebe, não armazena e não tem acesso** a nenhum dado seu ou dos seus contatos. A extensão não tem servidor próprio, não usa análise de uso (analytics) e não exibe anúncios.
- Os dados ficam no seu navegador e na plataforma que você escolheu.

## Quais dados a extensão trata

A integração só pode ser ativada depois que você aceita, nas opções da extensão, o tratamento de dados descrito aqui. Enquanto a integração está ativa e o WhatsApp Web está aberto, a extensão lê, na sua sessão do WhatsApp Web, os eventos que você habilitou nas opções e os envia à sua plataforma:

- **Mensagens:** texto ou legenda, tipo, data e hora, identificadores da mensagem e da conversa, se foi enviada ou recebida, se é de grupo e se partiu da automação ou de uma pessoa.
- **Contatos:** identificadores do WhatsApp (número de telefone e/ou identificador LID) e o nome de perfil exibido pelo WhatsApp.
- **Mídia:** apenas metadados (tipo, nome do arquivo e tamanho). O conteúdo de uma mídia só é enviado quando a sua plataforma pede explicitamente, pela ação `download_media`.
- **Outros eventos:** confirmações de entrega e leitura, reações, mensagens editadas ou apagadas, novas conversas, descadastros (opt-out) e resultados de comandos.
- **Conta conectada:** o número e o identificador da conta do WhatsApp Web em uso.

A extensão também executa no WhatsApp Web as ações que a sua plataforma devolve (por exemplo, enviar uma mensagem em uma conversa existente), sempre respeitando os limites de envio e a lista de descadastro.

## Para onde os dados vão

- **Para a sua plataforma de automação**, nas URLs que você informou. A extensão exige HTTPS (HTTP só é aceito para `localhost`) e pode assinar cada requisição com um segredo HMAC gerado por você.
- **Mídia:** a extensão só baixa arquivos (`send_file`) e só envia arquivos (`download_media`) para as origens que você autorizou. Ela não envia cookies nessas requisições.
- **Nenhum outro destino.** A extensão não envia dados ao desenvolvedor nem a terceiros. Os componentes de análise de uso e de pré-visualização de links de terceiros, presentes na biblioteca de código aberto usada para acessar o WhatsApp Web (wa-js), ficam desligados na versão distribuída.

O tratamento feito pela sua plataforma de automação segue as regras dela e as suas. Você é responsável por ter base legal (por exemplo, pela LGPD) para tratar os dados dos seus contatos e por informá-los quando necessário.

## O que fica armazenado no seu navegador

Os dados abaixo ficam no armazenamento local da extensão (`chrome.storage`), apenas no seu computador:

| Dado | Por quanto tempo |
|---|---|
| Configurações, incluindo URLs e segredo HMAC | Até você alterar ou desinstalar a extensão |
| Lista de descadastro (identificadores do contato, palavra usada e data) | Até você remover o contato nas opções ou desinstalar |
| Fila de falhas: eventos que não puderam ser entregues, com o seu conteúdo (até 200) | Até serem reenviados com sucesso, até você limpar a fila ou até serem substituídos por falhas mais novas |
| Identificadores de comandos já processados (até 1.000) | Substituídos pelos mais novos |
| Estado da sessão, métricas e contadores | Apagados ao fechar o navegador |

Os registros técnicos (logs) da extensão não incluem o conteúdo das mensagens.

## O que não fazemos

- Não vendemos, alugamos nem compartilhamos dados com terceiros.
- Não usamos dados para publicidade, análise de crédito ou qualquer finalidade alheia à integração.
- Não coletamos histórico de navegação. A extensão só atua em `web.whatsapp.com` e nos endereços que você configura.
- Pessoas não leem os seus dados, porque eles nunca chegam ao desenvolvedor.

## Seus controles

- Aceitar ou retirar o consentimento, ligar ou desligar a integração e escolher quais eventos são enviados, nas opções da extensão.
- Limpar a fila de falhas e remover contatos da lista de descadastro, nas opções.
- Desinstalar a extensão, o que apaga todos os dados armazenados por ela no navegador.

## Riscos de uso

A extensão usa uma integração não oficial com o WhatsApp Web. O uso de integrações não oficiais pode violar os Termos de Serviço do WhatsApp e levar ao bloqueio do número. A extensão aplica limites para reduzir esse risco (envio apenas em conversas existentes, limite de envios por minuto e respeito ao descadastro), mas não o elimina.

## Uso Limitado

O uso das informações recebidas pelas APIs do Chrome segue a Política de Dados do Usuário da Chrome Web Store, incluindo os requisitos de Uso Limitado.

## Alterações nesta política

Mudanças nesta política serão publicadas neste endereço, com nova data de atualização. Mudanças no tratamento de dados serão informadas nas notas da versão da extensão antes de entrarem em vigor.

## Contato

E-mail: waautomationbridge@gmail.com

---

# Privacy Policy — WA Automation Bridge

*Last updated: October 20, 2026*

WA Automation Bridge is a Google Chrome extension that connects WhatsApp Web, open in your browser, to an automation platform that you choose and configure (for example n8n, Make, Zapier or your own webhook). This policy explains what data the extension handles, where it goes and how you control it.

## Summary

- The extension sends data **only to the addresses you configure** in its options (webhook URL, command queue URL and allowed media origins).
- The developer of the extension **does not receive, store or have access to** any of your data or your contacts' data. The extension has no server of its own, uses no analytics and shows no ads.
- Data stays in your browser and on the platform you chose.

## What data the extension handles

The integration can only be enabled after you accept, in the extension options, the data processing described here. While the integration is enabled and WhatsApp Web is open, the extension reads, in your WhatsApp Web session, the events you enabled in the options and sends them to your platform:

- **Messages:** text or caption, type, date and time, message and chat identifiers, whether it was sent or received, whether it is a group message and whether it came from the automation or from a person.
- **Contacts:** WhatsApp identifiers (phone number and/or LID identifier) and the profile name shown by WhatsApp.
- **Media:** metadata only (type, file name and size). Media content is sent only when your platform explicitly requests it through the `download_media` action.
- **Other events:** delivery and read receipts, reactions, edited or deleted messages, new chats, opt-outs and command results.
- **Connected account:** the number and identifier of the WhatsApp Web account in use.

The extension also performs in WhatsApp Web the actions your platform returns (for example, sending a message in an existing chat), always within the sending limits and the opt-out list.

## Where data goes

- **To your automation platform**, at the URLs you entered. The extension requires HTTPS (HTTP is accepted only for `localhost`) and can sign every request with an HMAC secret you generate.
- **Media:** the extension only downloads files (`send_file`) from, and only uploads files (`download_media`) to, the origins you allowed. It sends no cookies with these requests.
- **Nowhere else.** The extension sends no data to the developer or to third parties. The third-party analytics and link-preview components included in the open-source library used to access WhatsApp Web (wa-js) are disabled in the distributed version.

Processing by your automation platform is governed by its rules and yours. You are responsible for having a legal basis (for example under the LGPD or the GDPR) to process your contacts' data and for informing them when required.

## What is stored in your browser

The data below is kept in the extension's local storage (`chrome.storage`), on your computer only:

| Data | How long |
|---|---|
| Settings, including URLs and the HMAC secret | Until you change them or uninstall the extension |
| Opt-out list (contact identifiers, keyword used and date) | Until you remove the contact in the options or uninstall |
| Failure queue: events that could not be delivered, with their content (up to 200) | Until they are resent successfully, you clear the queue, or newer failures replace them |
| Identifiers of processed commands (up to 1,000) | Replaced by newer ones |
| Session state, metrics and counters | Deleted when the browser closes |

The extension's technical logs do not include message content.

## What we do not do

- We do not sell, rent or share data with third parties.
- We do not use data for advertising, credit assessment or any purpose unrelated to the integration.
- We do not collect browsing history. The extension only acts on `web.whatsapp.com` and on the addresses you configure.
- No person reads your data, because it never reaches the developer.

## Your controls

- Give or withdraw consent, turn the integration on or off and choose which events are sent, in the extension options.
- Clear the failure queue and remove contacts from the opt-out list, in the options.
- Uninstall the extension, which deletes all data it stored in the browser.

## Usage risks

The extension uses an unofficial integration with WhatsApp Web. Using unofficial integrations may violate the WhatsApp Terms of Service and lead to the number being blocked. The extension applies limits to reduce this risk (sending only in existing chats, a per-minute sending limit and honoring opt-outs), but does not eliminate it.

## Limited Use

The use of information received from Chrome APIs will adhere to the Chrome Web Store User Data Policy, including the Limited Use requirements.

## Changes to this policy

Changes to this policy will be published at this address with a new update date. Changes to data handling will be announced in the extension's release notes before they take effect.

## Contact

Email: waautomationbridge@gmail.com
