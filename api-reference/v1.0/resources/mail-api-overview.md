---
title: Usar a API REST de Email do Outlook
description: O Microsoft Graph permite que o seu aplicativo obtenha acesso autorizado aos dados de email do Outlook do usuário em uma conta pessoal ou da organização.
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: 38563f65ae0675dce6cf0e21672c4ceb5c894ba9
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474467"
---
# <a name="use-the-outlook-mail-rest-api"></a>Usar a API REST de Email do Outlook

O Microsoft Graph permite que seu aplicativo obtenha acesso autorizado aos dados de email do Outlook de um usuário em uma conta pessoal ou organizacional. Com as [permissões de email](/graph/permissions-reference#mail-permissions) apropriadas delegadas ou do aplicativo, seu aplicativo pode acessar os dados de email do usuário conectado ou de qualquer usuário em um locatário. Para obter mais informações sobre tokens de acesso, registro de aplicativo e permissões delegadas e de aplicativo, consulte [ Noções básicas de autenticação e autorização](/graph/auth/auth-concepts).

[!INCLUDE [outlook-mailbox-type-support](../../includes/outlook-mailbox-type-support.md)]

## <a name="using-the-mail-rest-api"></a>Usar a API REST do email

As solicitações de API de email são realizadas em nome de um [usuário](../resources/user.md) que pode ser identificado pela propriedade **id** do usuário (um GUID exclusivo), endereço de email ou alias do atalho do `me` para o usuário conectado.

As mensagens de email são representadas pelo recurso [message](../resources/message.md) e organizado em uma [mailFolder](../resources/mailfolder.md). As mensagens e as pastas principais são identificadas por sua propriedade **id**, obtida das operações de `GET`.

>[!IMPORTANT] 
> Em geral, não assuma que os IDs das **mensagens** e das **pastas de correio** são exclusivos e sempre permanecem os mesmos em uma caixa de correio. Eles podem mudar após determinadas ações, como copiar ou mover. Você pode optar por usar as [IDs imutáveis](/graph/outlook-immutable-id) para manter a mesma ID, desde que a mensagem permaneça na mesma caixa de correio, _com exceção de envio de uma mensagem de rascunho e alguns outros cenários_. Confira [tempo de vida das IDs imutáveis](/graph/outlook-immutable-id#lifetime-of-immutable-ids) para obter detalhes.

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
| Delegar outro usuário para enviar mensagens em nome do proprietário da caixa de correio | [message](../resources/message.md) | Configurar as propriedades **from** e **sender** em uma [message](../resources/message.md) |
| Permitir que o usuário visualize as mensagens mais importantes primeiro | [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) | [Caixa de Entrada Prioritária](../resources/manage-focused-inbox.md) |
| Consular mensagens e obtê-las em uma pasta de pesquisa  | [mailSearchFolder](../resources/mailsearchfolder.md) | [Métodos de mailSearchFolder](../resources/mailsearchfolder.md#methods) |
| Obter o conteúdo MIME de uma mensagem ou de um anexo de mensagem | [Mensagem](../resources/message.md) | [Obter conteúdo de MIME](/graph/outlook-get-mime-message) |
| Adicionar, obter ou excluir anexos de uma mensagem | [attachment](../resources/attachment.md), <br> [fileAttachment](../resources/fileattachment.md), <br> [itemAttachment](../resources/itemattachment.md), <br> [referenceAttachment](../resources/referenceattachment.md), <br> [message](../resources/message.md) | [Métodos de anexo](../resources/attachment.md#methods) |
| Acessar as opções de idioma e fuso horário para um usuário | [localeInfo](localeinfo.md), <br> [timeZoneInformation](timezoneinformation.md) | [supportedLanguages](../api/outlookuser-supportedlanguages.md), <br> [supportedTimeZones](../api/outlookuser-supportedtimezones.md) |
| Obter ou atualizar resposta automática, localidade, fuso horário ou horário de trabalho de um usuário | [mailboxSettings](../resources/mailboxsettings.md), <br> [automaticRepliesSetting](../resources/automaticrepliessetting.md), <br> [localeInfo](../resources/localeinfo.md), <br> [workingHours](../resources/workinghours.md) | [Obter configurações da caixa de correio do usuário](../api/user-get-mailboxsettings.md), <br> [Atualizar configurações da caixa de correio do usuários](../api/user-update-mailboxsettings.md) |
| Obter MailTips do status especial de outros destinatários, como ausência temporária | [user](../resources/user.md), <br> [mailTips](../resources/mailtips.md) | [Get MailTips](../api/user-getmailtips.md) |
| **Gerenciamento de pasta e email** | | |
| Organizar mensagens em uma hierarquia de pasta de email | [mailFolder](../resources/mailfolder.md)  | [Métodos de mailFolder](../resources/mailfolder.md#methods) |
| Categorizar mensagens | [outlookCategory](../resources/outlookcategory.md) | [Métodos de outlookCategory](../resources/outlookcategory.md#methods) |
| Usar regras de Caixa de Entrada para automatizar ações como encaminhar mensagens de entrada específicas | [messageRule](../resources/messagerule.md) | [Métodos de messageRule](../resources/messagerule.md#methods) |
| Obter cabeçalhos de mensagens da Internet de uma mensagem | [message](../resources/message.md) | [Obter a propriedade **internetMessageHeaders** de uma mensagem](../api/message-get.md#example-2-get-internet-message-headers). |
| Pesquisar e filtrar mensagens | [message](../resources/message.md) | [Parâmetros de consulta](/graph/query-parameters)  |
| Receber notificações de alterações para as mensagens em uma pasta | [subscription](../resources/subscription.md) | [Trabalhando com webhooks no Microsoft Graph](../resources/webhooks.md) |
| Sincronizar mensagens ou a hierarquia da pasta de email | [message](../resources/message.md) | [Obter as alterações incrementais para as mensagens em uma pasta](/graph/delta-query-messages) |
| **Desenvolvimento de aplicativo** | | |
| Adicionar dados de aplicativos personalizados como cabeçalhos de mensagens da Internet de uma mensagem | [message](../resources/message.md) | Adicione dados personalizados à propriedade **internetMessageHeaders** da mensagem. |
| Adicionar dados personalizados de aplicativo a uma mensagem usando extensões | [openTypeExtension](../resources/opentypeextension.md), <br>[schemaExtension](../resources/schemaextension.md) | [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview) |
| Acessar dados personalizados para propriedades subexpostas de MAPI do Outlook | [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), <br> [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) | [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md) |

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="next-steps"></a>Próximas etapas

A API de email pode permitir novas formas de envolvimento com os usuários:

- [Visão geral da API de email do Outlook](/graph/outlook-mail-concept-overview)
- Analise em detalhes os [métodos](../resources/message.md#methods), [propriedades](../resources/message.md#properties) e [relações](../resources/message.md#relationships) dos recursos de [message](../resources/message.md) e [mailFolder](../resources/mailfolder.md).
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

Precisa de mais ideias? Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).

