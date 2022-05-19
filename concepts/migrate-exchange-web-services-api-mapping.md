---
title: Exchange EWS (Serviços Web) para o Microsoft API do Graph mapeamentos
description: Este artigo lista as APIs Graph Microsoft que são mapeadas Exchange APIs dos Serviços Web (EWS).
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: 93ecef5daccc29743a74258eae1624e8e78dcd4f
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549607"
---
# <a name="exchange-web-services-ews-to-microsoft-graph-api-mappings"></a>Exchange EWS (Serviços Web) para o Microsoft API do Graph mapeamentos

Este artigo lista as APIs Graph Microsoft que são mapeadas Exchange APIs dos Serviços Web (EWS).

## <a name="utility-apis"></a>APIs de utilitário

| EWS API                                                                                             | API do Microsoft Graph |
|-----------------------------------------------------------------------------------------------------|-----|
| [ConvertId](/exchange/client-developer/web-service-reference/convertid-operation)                   | [Traduzir Exchange IDs](/graph/api/user-translateexchangeids) |
| [ResolveNames](/exchange/client-developer/web-service-reference/resolvenames-operation)             | [Listar pessoas](/graph/api/user-list-people) |
| [GetServerTimeZones](/exchange/client-developer/web-service-reference/getservertimezones-operation) | [Obter opções de fuso horário](/graph/api/outlookuser-supportedtimezones) |

## <a name="mail-apis"></a>APIs de Email

### <a name="messages"></a>Mensagens

| EWS API                                                                             | API do Microsoft Graph |
|-------------------------------------------------------------------------------------|-----|
| [CreateItem](/exchange/client-developer/web-service-reference/createitem-operation) | [Criar mensagem](/graph/api/user-post-messages) |
| [CopyItem](/exchange/client-developer/web-service-reference/copyitem-operation)     | [Copiar mensagem](/graph/api/message-copy) |
| [DeleteItem](/exchange/client-developer/web-service-reference/deleteitem-operation) | [Excluir mensagem](/graph/api/message-delete) |
| [FindItem](/exchange/client-developer/web-service-reference/finditem-operation)     | [Listar mensagens](/graph/api/user-list-messages) |
| [GetItem](/exchange/client-developer/web-service-reference/getitem-operation)       | [Obter mensagem](/graph/api/message-get) |
| [MoveItem](/exchange/client-developer/web-service-reference/moveitem-operation)     | [Mover mensagem](/graph/api/message-move) |
| [SendItem](/exchange/client-developer/web-service-reference/senditem-operation)     | [Enviar mensagem ou](/graph/api/message-send) [Enviar email](/graph/api/user-sendmail) |
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

### <a name="attachments"></a>Anexos

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

### <a name="out-of-office-oof-settings"></a>Configurações de Office (OOF)

| EWS API                                                                                             | API do Microsoft Graph |
|-----------------------------------------------------------------------------------------------------|-----|
| [GetUserOofSettings](/exchange/client-developer/web-service-reference/getuseroofsettings-operation) | [Obtém configurações de caixa de correio do usuário](/graph/api/user-get-mailboxsettings) |
| [SetUserOofSettings](/exchange/client-developer/web-service-reference/setuseroofsettings-operation) | [Atualizar configurações da caixa de correio do usuário](/graph/api/user-update-mailboxsettings) |

### <a name="notifications"></a>Notificações

> [!NOTE]
> O Microsoft Graph requer apenas uma assinatura para notificações por push. Se você estiver usando notificações de [pull do EWS](/exchange/client-developer/exchange-web-services/how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange) no momento, consulte [Obter delta de mensagens](/graph/api/message-delta).

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

## <a name="calendar-apis"></a>APIs de Calendário

### <a name="availability"></a>Disponibilidade

| EWS API                                                                                               | API do Microsoft Graph |
|-------------------------------------------------------------------------------------------------------|-----|
| [GetUserAvailability](/exchange/client-developer/web-service-reference/getuseravailability-operation)<br/>FindAvailableMeetingTimes | [Obter agenda de disponibilidade](/graph/api/calendar-getschedule)|
 

### <a name="reminders"></a>Reminders

<!-- markdownlint-disable MD033 -->
| EWS API                                                                                                   | API do Microsoft Graph |
|-----------------------------------------------------------------------------------------------------------|-----|
| [GetReminders](/exchange/client-developer/web-service-reference/getreminders-operation)                   | [Modo de exibição de lembrete](/graph/api/user-reminderview) |
| [PerformReminderAction](/exchange/client-developer/web-service-reference/performreminderaction-operation) | [Descartar lembrete](/graph/api/event-dismissreminder)<br/>[Adiar lembrete](/graph/api/event-snoozereminder) |
<!-- markdownlint-enable MD033 -->

### <a name="permissions"></a>Permissões

<!-- markdownlint-disable MD033 -->
| EWS API                                                                                                   | API do Microsoft Graph |
|-----------------------------------------------------------------------------------------------------------|-----|
| [GetReminders](/exchange/client-developer/web-service-reference/getreminders-operation)                   | [Modo de exibição de lembrete](/graph/api/user-reminderview) |
| [PerformReminderAction](/exchange/client-developer/web-service-reference/performreminderaction-operation) | [Descartar lembrete](/graph/api/event-dismissreminder)<br/>[Adiar lembrete](/graph/api/event-snoozereminder) |
|CreateSharingPermission,GetSharingPermission | [Proprietário do calendário: obter informações e permissões de compartilhamento e delegação](outlook-share-or-delegate-calendar.md#calendar-owner-get-sharing-or-delegation-information-and-permissions)|
|UpdateSharingPermission | [Obtenha informações de calendário sobre compartilhamento, delegados e permissões permitidas e atualize permissões individuais.](outlook-share-or-delegate-calendar.md#get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions)|
|DeleteSharingPermission| [Exclua um compartilhamento ou um representante de um calendário.](outlook-share-or-delegate-calendar.md#delete-a-sharee-or-delegate-of-a-calendar)|
|GetSharingPermissionInfo | [Proprietário do calendário: Obter propriedades de um calendário compartilhado ou delegado](outlook-share-or-delegate-calendar.md#get-properties-of-a-shared-or-delegated-calendar)|

### <a name="invitations"></a>Convites
| EWS API                                                                                                   | API do Microsoft Graph |
|-----------------------------------------------------------------------------------------------------------|-----|
|ActivateSharingInvitation | [Compartilhar ou delegar um calendário no Outlook](/graph/outlook-share-or-delegate-calendar)|
|GetSharingInvitation | [Compartilhamento: Obtenha um calendário compartilhado ou seus eventos diretamente da caixa de correio do proprietário do calendário](outlook-get-shared-events-calendars.md#sharee-get-a-shared-calendar-or-its-events-directly-from-calendar-owners-mailbox)|
|DeleteSharingInvitation | [Proprietário do calendário: atualizar permissões para um compartilhamento existente ou delegado em um calendário](outlook-share-or-delegate-calendar.md#calendar-owner-update-permissions-for-an-existing-sharee-or-delegate-on-a-calendar)|
|CreateSharingInvitation | [Criar eventos do Outlook em um calendário compartilhado ou delegado](outlook-create-event-in-shared-delegated-calendar.md#step-2-adele-creates-and-sends-an-invitation-on-alex-behalf)|

### <a name="shared-information"></a>Informações Compartilhadas
| EWS API                                                                                                   | API do Microsoft Graph |
|-----------------------------------------------------------------------------------------------------------|-----|
| GetCalendarSharedInformation,GetConsumerCalendarSharedInformation | [Listar calendários](/graph/api/user-list-calendars) |
## <a name="groups-apis"></a>APIs de grupos

| EWS API                                                                                               | API do Microsoft Graph |
|-------------------------------------------------------------------------------------------------------|-----|
| GetUserUnifiedGroups | [Listar memberof](/graph/api/user-list-memberof) |
| GetUnifiedGroupsSettings | [groupSetting](/graph/api/resources/groupsetting) |
| GetUnifiedGroupDetails | [Obter grupo](/graph/api/group-get) |
| GetUnifiedGroupMembers | [Listar membros](/graph/api/group-list-members) |
| GetUnifiedGroupUnseenCount | [Obter grupo](/graph/api/group-get) |
| SetUnifiedGroupMembershipState | [Adicionar/remover membro/proprietário](/graph/api/resources/group) |
| FindUnifiedGroups | [Listar grupos](/graph/api/group-list) |
| SetUnifiedGroupUserSubscribeState | [Assinar/cancelar assinaturaByMail](/graph/api/group-subscribebymail) |
| UpdateUnifiedGroup | [Atualizar grupo](/graph/api/group-update) |
| CreateUnifiedGroup | [Criar grupo](/graph/api/group-post-groups) |
| RemoveUnifiedGroup | [Excluir grupo](/graph/api/group-delete) |
| SetUnifiedGroupFavoriteState | [AddFavorite de grupo](/graph/api/group-addfavorite) |
| JoinPrivateUnifiedGroup | [Assinar/cancelar assinaturaByMail](/graph/api/group-subscribebymail) |
| GetDlMembersForUnifiedGroup | [Listar membros de grupo](/graph/api/group-list-members) |
