---
title: Exchange Web Services (EWS) para mapeamentos de API Graph Microsoft
description: Este artigo lista as APIs do Microsoft Graph mapeadas para apIs Exchange Web Services (EWS).
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: 89aa884baf0ae5d2a67d31f3e28d4c818be2c9af
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516544"
---
# <a name="exchange-web-services-ews-to-microsoft-graph-api-mappings"></a>Exchange Web Services (EWS) para mapeamentos de API Graph Microsoft

Este artigo lista as APIs do Microsoft Graph mapeadas para apIs Exchange Web Services (EWS).

## <a name="utility-apis"></a>APIs de utilitário

| EWS API                                                                                             | API do Microsoft Graph |
|-----------------------------------------------------------------------------------------------------|-----|
| [ConvertId](/exchange/client-developer/web-service-reference/convertid-operation)                   | [Traduzir Exchange IDs](/graph/api/user-translateexchangeids) |
| [ResolveNames](/exchange/client-developer/web-service-reference/resolvenames-operation)             | [Listar pessoas](/graph/api/user-list-people) |
| [GetServerTimeZones](/exchange/client-developer/web-service-reference/getservertimezones-operation) | [Obter opções de fuso horário](/graph/api/outlookuser-supportedtimezones) |

## <a name="mail-apis"></a>APIs de email

### <a name="messages"></a>Mensagens

| EWS API                                                                             | API do Microsoft Graph |
|-------------------------------------------------------------------------------------|-----|
| [CreateItem](/exchange/client-developer/web-service-reference/createitem-operation) | [Criar mensagem](/graph/api/user-post-messages) |
| [CopyItem](/exchange/client-developer/web-service-reference/copyitem-operation)     | [Copiar mensagem](/graph/api/message-copy) |
| [DeleteItem](/exchange/client-developer/web-service-reference/deleteitem-operation) | [Excluir mensagem](/graph/api/message-delete) |
| [FindItem](/exchange/client-developer/web-service-reference/finditem-operation)     | [Listar mensagens](/graph/api/user-list-messages) |
| [GetItem](/exchange/client-developer/web-service-reference/getitem-operation)       | [Obter mensagem](/graph/api/message-get) |
| [MoveItem](/exchange/client-developer/web-service-reference/moveitem-operation)     | [Mover mensagem](/graph/api/message-move) |
| [SendItem](/exchange/client-developer/web-service-reference/senditem-operation)     | [Enviar mensagem](/graph/api/message-send) ou [enviar email](/graph/api/user-sendmail) |
| [UpdateItem](/exchange/client-developer/web-service-reference/updateitem-operation) | [Atualizar mensagem](/graph/api/message-update) |

### <a name="folders"></a>Folders

| EWS API                                                                                 | API do Microsoft Graph |
|-----------------------------------------------------------------------------------------|-----|
| [CreateFolder](/exchange/client-developer/web-service-reference/createfolder-operation) | [Criar pasta de email](/graph/api/user-post-mailfolders) |
| [CopyFolder](/exchange/client-developer/web-service-reference/copyfolder-operation)     | [Copiar pasta de email](/graph/api/mailfolder-copy) |
| [DeleteFolder](/exchange/client-developer/web-service-reference/deletefolder-operation) | [Excluir pasta de email](/graph/api/mailfolder-delete) |
| [GetFolder](/exchange/client-developer/web-service-reference/getfolder-operation)       | [Obter pasta de email](/graph/api/mailfolder-get) |
| [MoveFolder](/exchange/client-developer/web-service-reference/movefolder-operation)     | [Mover pasta de email](/graph/api/mailfolder-move) |
| [UpdateFolder](/exchange/client-developer/web-service-reference/updatefolder-operation) | [Atualizar pasta de email](/graph/api/mailfolder-update) |

### <a name="attachments"></a>Attachments

| EWS API                                                                                         | API do Microsoft Graph |
|-------------------------------------------------------------------------------------------------|-----|
| [CreateAttachment](/exchange/client-developer/web-service-reference/createattachment-operation) | [Add attachment](/graph/api/message-post-attachments) |
| [GetAttachment](/exchange/client-developer/web-service-reference/getattachment-operation)       | [Obter anexo](/graph/api/attachment-get) |
| [DeleteAttachment](/exchange/client-developer/web-service-reference/deleteattachment-operation) | [Excluir anexo](/graph/api/attachment-delete) |

### <a name="rules"></a>Rules

<!-- markdownlint-disable MD033 -->
| EWS API                                                                                         | API do Microsoft Graph |
|-------------------------------------------------------------------------------------------------|-----|
| [GetInboxRules](/exchange/client-developer/web-service-reference/getinboxrules-operation)       | [Listar regras](/graph/api/mailfolder-list-messagerules) |
| [UpdateInboxRules](/exchange/client-developer/web-service-reference/updateinboxrules-operation) | [Criar regra](/graph/api/mailfolder-post-messagerules)<br/>[Atualizar regra](/graph/api/messagerule-update)<br/>[Excluir regra](/graph/api/messagerule-delete) |
<!-- markdownlint-enable MD033 -->

### <a name="mailtips"></a>MailTips

| EWS API                                                                               | API do Microsoft Graph |
|---------------------------------------------------------------------------------------|-----|
| [GetMailTips](/exchange/client-developer/web-service-reference/getmailtips-operation) | [Get MailTips](/graph/api/user-getmailtips) |

### <a name="out-of-office-oof-settings"></a>Definições Office (OOF)

| EWS API                                                                                             | API do Microsoft Graph |
|-----------------------------------------------------------------------------------------------------|-----|
| [GetUserOofSettings](/exchange/client-developer/web-service-reference/getuseroofsettings-operation) | [Obtém configurações de caixa de correio do usuário](/graph/api/user-get-mailboxsettings) |
| [SetUserOofSettings](/exchange/client-developer/web-service-reference/setuseroofsettings-operation) | [Atualizar configurações da caixa de correio do usuário](/graph/api/user-update-mailboxsettings) |

### <a name="notifications"></a>Notificações

> [!NOTE]
> O Microsoft Graph requer apenas uma assinatura para notificações por push. Se você estiver usando notificações de [pull do EWS](/exchange/client-developer/exchange-web-services/how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange) no momento, consulte [Obter mensagens delta](/graph/api/message-delta).

| EWS API                                                                                                    | API do Microsoft Graph |
|------------------------------------------------------------------------------------------------------------|-----|
| [GetEvents](/exchange/client-developer/web-service-reference/getevents-operation)                          | [Obter mensagens delta](/graph/api/message-delta) |
| [Assinar](/exchange/client-developer/web-service-reference/subscribe-operation) (notificações por push)     | [Criar assinatura](/graph/api/subscription-post-subscriptions) |
| [Cancelar assinatura](/exchange/client-developer/web-service-reference/unsubscribe-operation) (notificações por push) | [Excluir assinatura](/graph/api/subscription-delete) |

### <a name="synchronization"></a>Sincronização

| EWS API                                                                                               | API do Microsoft Graph |
|-------------------------------------------------------------------------------------------------------|-----|
| [SyncFolderHierarchy](/exchange/client-developer/web-service-reference/syncfolderhierarchy-operation) | [Obter a pasta de email delta](/graph/api/mailfolder-delta) |
| [SyncFolderItems](/exchange/client-developer/web-service-reference/syncfolderitems-operation)         | [Obter mensagens delta](/graph/api/message-delta) |

## <a name="calendar-apis"></a>APIs de calendário

### <a name="availability"></a>Disponibilidade

| EWS API                                                                                               | API do Microsoft Graph |
|-------------------------------------------------------------------------------------------------------|-----|
| [GetUserAvailability](/exchange/client-developer/web-service-reference/getuseravailability-operation) | [Obter agenda de disponibilidade](/graph/api/calendar-getschedule) |

### <a name="reminders"></a>Reminders

<!-- markdownlint-disable MD033 -->
| EWS API                                                                                                   | API do Microsoft Graph |
|-----------------------------------------------------------------------------------------------------------|-----|
| [GetReminders](/exchange/client-developer/web-service-reference/getreminders-operation)                   | [Modo de exibição de lembrete](/graph/api/user-reminderview) |
| [PerformReminderAction](/exchange/client-developer/web-service-reference/performreminderaction-operation) | [Descartar lembrete](/graph/api/event-dismissreminder)<br/>[Adiar lembrete](/graph/api/event-snoozereminder) |
<!-- markdownlint-enable MD033 -->
