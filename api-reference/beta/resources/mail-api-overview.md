---
title: Usar a API REST de Email do Outlook
description: O Microsoft Graph permite que o seu aplicativo obtenha acesso autorizado aos dados de email do Outlook do usuário em uma conta pessoal ou da organização.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: a42b1508ab022bfd530b9338dc8049c65f478727
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463793"
---
# <a name="use-the-outlook-mail-rest-api"></a>Usar a API REST de Email do Outlook

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O Microsoft Graph permite que o seu aplicativo obtenha acesso autorizado aos dados de email do Outlook do usuário em uma conta pessoal ou da organização. Com as [permissões de aplicativo e delegadas apropriadas](/graph/permissions-reference), seu aplicativo pode acessar os dados de email do usuário conectado ou qualquer usuário em um locatário. Os dados de email podem estar na nuvem no Exchange Online como parte do Office 365, ou no Exchange no local em uma [implantação híbrida](/graph/hybrid-rest-support).

## <a name="using-the-mail-rest-api"></a>Usar a API REST do email

As solicitações de API de email são realizadas em nome de um [usuário](../resources/user.md) que pode ser identificado pela propriedade **id** do usuário (um GUID exclusivo), endereço de email ou alias do atalho do `me` para o usuário conectado.

As mensagens de email são representadas pelo recurso [message](../resources/message.md) e organizado em uma [mailFolder](../resources/mailfolder.md). As mensagens e as pastas principais são identificadas por sua propriedade **id**, obtida das operações de `GET`.

> **Observação:** em geral, não pressupõem que as IDs de **message** e **mailfolder** são únicas e imutáveis em uma caixa de correio. Elas podem mudar após certas ações, como copiar, mover ou enviar.

Os corpos de mensagens podem estar no formato HTML ou no formato de texto.

Você pode usar nomes comuns, como `Inbox`, `Drafts`, `SentItems` ou `DeletedItems`, para identificar certas pastas de email que existem por padrão para todos os usuários. Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).

Por exemplo, você pode obter mensagem na pasta **Itens enviados** do Outlook do usuário conectado, sem primeiro obter o ID da pasta:

```http
GET /me/mailFolders('SentItems')/messages?$select=sender,subject
```

## <a name="common-use-cases"></a>Casos de uso comuns

O recurso **message** expõe propriedades como **categories**, **conversationId**, **flag** e **importance** que correspondem a recursos disponíveis na interface do usuário, permitindo que os aplicativos automatizem ou integrem a experiência de usuário interna do Outlook.

A API do Microsoft Graph também fornece métodos e ações que ofereçam suporte a casos de uso comuns de mensagens.

| Casos de uso | Recursos REST | Confira também |
|:----------|:---------------|:---------|
| **Ações centradas no usuário** | | |
| Rascunho, ler, responder, encaminhar, enviar, atualizar ou excluir mensagens | [message](../resources/message.md) | [Métodos de mensagem](../resources/message.md#methods) |
| Delegar outro usuário para enviar mensagens em nome do proprietário da caixa de correio | [message](../resources/message.md) | Configurar as propriedades **from** e **sender** em uma [mensagem](../resources/message.md) |
| Permitir que o usuário visualize as mensagens mais importantes primeiro | [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) | [Caixa de Entrada Prioritária](../resources/manage-focused-inbox.md) |
| Obter o conteúdo de MIME de uma mensagem ou anexo de mensagem (versão prévia) | [message](../resources/message.md) | [Obter conteúdo de MIME](/graph/outlook-get-mime-message) |
| Adicionar, obter ou excluir anexos de uma mensagem | [attachment](../resources/attachment.md), <br> [fileAttachment](../resources/fileattachment.md), <br> [itemAttachment](../resources/itemattachment.md), <br> [referenceAttachment](../resources/referenceattachment.md), <br> [message](../resources/message.md) | [Métodos de anexo](../resources/attachment.md#methods) |
| Acessar as opções de idioma e fuso horário para um usuário | [localeInfo](localeinfo.md), <br> [timeZoneInformation](timezoneinformation.md) | [supportedLanguages](../api/outlookuser-supportedlanguages.md), <br> [supportedTimeZones](../api/outlookuser-supportedtimezones.md) |
| Obter ou atualizar resposta automática, localidade, fuso horário ou horário de trabalho de um usuário | [mailboxSettings](../resources/mailboxsettings.md), <br> [automaticRepliesSetting](../resources/automaticrepliessetting.md), <br> [localeInfo](../resources/localeinfo.md), <br> [workingHours](../resources/workinghours.md) | [Obter configurações da caixa de correio do usuário](../api/user-get-mailboxsettings.md), <br> [Atualizar configurações da caixa de correio do usuários](../api/user-update-mailboxsettings.md) |
| Obter MailTips do status especial de outros destinatários, como ausência temporária | [user](../resources/user.md), <br> [mailTips](../resources/mailtips.md) | [Get MailTips](../api/user-getmailtips.md) |
| Alertar usuário se mencionado em outras mensagens (visualização) | [mention (visualização)](../resources/mention.md) | [Obter os detalhes de @menções em uma mensagem](../api/message-get.md#request-2) |
| Cancelar a assinatura de usuário de uma lista de distribuição de emails (visualização) | [message (visualização)](../resources/message.md) | [Cancelar assinatura](../api/message-unsubscribe.md) |
| **Gerenciamento de pasta e email** | | |
| Organizar mensagens em uma hierarquia de pasta de email | [mailFolder](../resources/mailfolder.md)  | [Métodos de mailFolder](../resources/mailfolder.md#methods) |
| Categorizar mensagens | [outlookCategory (visualização)](../resources/outlookcategory.md) | [Métodos de outlookCategory](../resources/outlookcategory.md#methods) |
| Usar regras de Caixa de Entrada para automatizar ações como encaminhar mensagens de entrada específicas | [messageRule (visualização)](../resources/messagerule.md) | [Métodos de messageRule](../resources/messagerule.md#methods) |
| Obter cabeçalhos de mensagens da Internet de uma mensagem | [message (visualização)](../resources/message.md) | [Obter a propriedade **internetMessageHeaders** de uma mensagem](../api/message-get.md#request-4). |
| Pesquisar e filtrar mensagens | [message](../resources/message.md) | [Parâmetros de consulta](/graph/query-parameters)  |
| Receber notificações de alterações para as mensagens em uma pasta | [subscription](../resources/subscription.md) | [Trabalhando com webhooks no Microsoft Graph](../resources/webhooks.md) |
| Sincronizar mensagens ou a hierarquia da pasta de email | [message](../resources/message.md) | [Obter as alterações incrementais para as mensagens em uma pasta](/graph/delta-query-messages) |
| **Desenvolvimento de aplicativo** | | |
| Adicionar dados de aplicativos personalizados como cabeçalhos de mensagens da Internet de uma mensagem | [message](../resources/message.md) | Adicionar dados personalizados à coleção **internetMessageHeaders** da mensagem. |
| Adicionar dados personalizados de aplicativo a uma mensagem usando extensões | [openTypeExtension](../resources/opentypeextension.md), <br>[schemaExtension](../resources/schemaextension.md) | [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview) |
| Acessar dados personalizados para propriedades subexpostas de MAPI do Outlook | [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), <br> [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) | [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md) |

## <a name="next-steps"></a>Próximas etapas

A API de email pode permitir novas formas de envolvimento com os usuários:

- [Visão geral da API de email do Outlook](/graph/outlook-mail-concept-overview)
- Analise em detalhes os [métodos](../resources/message.md#methods), [propriedades](../resources/message.md#properties) e [relações](../resources/message.md#relationships) dos recursos de [message](../resources/message.md) e [mailFolder](../resources/mailfolder.md).
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

Precisa de mais ideias? Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).
