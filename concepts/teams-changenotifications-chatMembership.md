---
title: Obtenha as notificações de alteração para associação de chat o usando o Microsoft Graph
description: Saiba como obter notificações de alterações de associação de chat usando as APIs do Microsoft Graph.
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: aa8fa5ddea9c8e0df8eb8bf81558840392bdd306
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53367014"
---
# <a name="get-change-notifications-for-chat-membership-using-microsoft-graph"></a><span data-ttu-id="66660-103">Obtenha as notificações de alteração para associação de chat o usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="66660-103">Get change notifications for chat membership using Microsoft Graph</span></span>

<span data-ttu-id="66660-104">As notificações de alteração permitem que você se inscreva para receber alterações (criar e excluir) na associação de chats.</span><span class="sxs-lookup"><span data-stu-id="66660-104">Change notifications enable you to subscribe to changes (create and delete) in chats membership.</span></span> <span data-ttu-id="66660-105">Você pode ser notificado sempre que um membro for adicionado ou removido de um chat.</span><span class="sxs-lookup"><span data-stu-id="66660-105">You can get notified whenever a member is added or removed from a chat.</span></span> <span data-ttu-id="66660-106">Você também pode obter os dados do recurso nas notificações e, portanto, evitar chamar a API para obter o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="66660-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

## <a name="subscribe-to-changes-in-membership-of-any-chat-at-tenant-level"></a><span data-ttu-id="66660-107">Inscrever-se para alterações na associação de qualquer chat a nível de locatário</span><span class="sxs-lookup"><span data-stu-id="66660-107">Subscribe to changes in membership of any chat at tenant level</span></span>

<span data-ttu-id="66660-108">Para obter notificações de alteração para alterações de associação em qualquer chat do locatário, inscreva-se em `/chats/getAllMembers`.</span><span class="sxs-lookup"><span data-stu-id="66660-108">To get change notifications for membership changes in any chat across the tenant, subscribe to `/chats/getAllMembers`.</span></span> <span data-ttu-id="66660-109">Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.</span><span class="sxs-lookup"><span data-stu-id="66660-109">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="66660-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="66660-110">Permissions</span></span>

|<span data-ttu-id="66660-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66660-111">Permission type</span></span>      | <span data-ttu-id="66660-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66660-112">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="66660-113">Versões com suporte</span><span class="sxs-lookup"><span data-stu-id="66660-113">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="66660-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66660-114">Delegated (work or school account)</span></span> | <span data-ttu-id="66660-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66660-115">Not supported.</span></span> | <span data-ttu-id="66660-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66660-116">Not supported.</span></span> |
|<span data-ttu-id="66660-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66660-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66660-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66660-118">Not supported.</span></span>    | <span data-ttu-id="66660-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66660-119">Not supported.</span></span> |
|<span data-ttu-id="66660-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66660-120">Application</span></span> | <span data-ttu-id="66660-121">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66660-121">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span>  | <span data-ttu-id="66660-122">beta</span><span class="sxs-lookup"><span data-stu-id="66660-122">beta</span></span>|

### <a name="example"></a><span data-ttu-id="66660-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66660-123">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/getAllMembers",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-membership-of-a-particular-chat"></a><span data-ttu-id="66660-124">Inscrever-se para alterações na associação de um chat específico</span><span class="sxs-lookup"><span data-stu-id="66660-124">Subscribe to changes in membership of a particular chat</span></span>

<span data-ttu-id="66660-125">Para obter notificações de alteração de membros em um chat específico, inscreva-se em `/chats/{id}/members`.</span><span class="sxs-lookup"><span data-stu-id="66660-125">To get change notifications for membership changes in a particular chat, subscribe to `/chats/{id}/members`.</span></span> <span data-ttu-id="66660-126">Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.</span><span class="sxs-lookup"><span data-stu-id="66660-126">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="66660-127">Permissões</span><span class="sxs-lookup"><span data-stu-id="66660-127">Permissions</span></span>

|<span data-ttu-id="66660-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66660-128">Permission type</span></span>      | <span data-ttu-id="66660-129">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66660-129">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="66660-130">Versões com suporte</span><span class="sxs-lookup"><span data-stu-id="66660-130">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="66660-131">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66660-131">Delegated (work or school account)</span></span> | <span data-ttu-id="66660-132">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66660-132">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="66660-133">beta</span><span class="sxs-lookup"><span data-stu-id="66660-133">beta</span></span> |
|<span data-ttu-id="66660-134">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66660-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66660-135">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66660-135">Not supported.</span></span>    | <span data-ttu-id="66660-136">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66660-136">Not supported.</span></span> |
|<span data-ttu-id="66660-137">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66660-137">Application</span></span> | <span data-ttu-id="66660-138">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66660-138">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span>  | <span data-ttu-id="66660-139">beta</span><span class="sxs-lookup"><span data-stu-id="66660-139">beta</span></span> |

> <span data-ttu-id="66660-140">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="66660-140">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="example"></a><span data-ttu-id="66660-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66660-141">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/members",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```



### <a name="notifications-with-resource-data"></a><span data-ttu-id="66660-142">Notificações com dados de recursos</span><span class="sxs-lookup"><span data-stu-id="66660-142">Notifications with resource data</span></span>

<span data-ttu-id="66660-143">Para notificações com dados de recursos, a carga se parece com a seguinte.</span><span class="sxs-lookup"><span data-stu-id="66660-143">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="66660-144">Este conteúdo é para uma alteração na filiação em um chat.</span><span class="sxs-lookup"><span data-stu-id="66660-144">This payload is for a membership change in a chat.</span></span>

```json
{
    "value": [{
        "subscriptionId": "c0125ef2-7a87-4e94-aa71-b995510f369b",
        "changeType": "Created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-06-03T11:04:58.5537601+00:00",
        "resource": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')/members('MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=')",
        "resourceData": {
            "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=",
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "@odata.id": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')/members('MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=')"
        },
        "EncryptedContent": {
            "data": "<<--EncryptedContent-->>",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
    }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

<span data-ttu-id="66660-145">Para obter detalhes sobre como validar tokens e descriptografar a carga útil, consulte [Definir notificações de alteração que incluem dados de recursos](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="66660-145">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="66660-146">A carga de notificação descriptografada parece com a seguinte.</span><span class="sxs-lookup"><span data-stu-id="66660-146">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="66660-147">O conteúdo está em conformidade com o esquema [aaduserconversationmember](/graph/api/resources/aaduserconversationmember?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="66660-147">The payload conforms to the [aaduserconversationmember](/graph/api/resources/aaduserconversationmember?preserve-view=true) schema.</span></span> <span data-ttu-id="66660-148">A carga é semelhante à devolvida pelas operações GET.</span><span class="sxs-lookup"><span data-stu-id="66660-148">The payload is similar to that returned by GET operations.</span></span>

```json
{
    "userId": "2fc60663-19a2-4aa4-852c-f7ba4e90ada2",
    "email": null,
    "tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
    "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=",
    "roles": [
    "Owner"
    ],
    "displayName": null,
    "visibleHistoryStartDateTime": "1970-01-01T00:00:00Z",
    "user": null
}
```

### <a name="notifications-without-resource-data"></a><span data-ttu-id="66660-149">Notificações sem dados de recursos</span><span class="sxs-lookup"><span data-stu-id="66660-149">Notifications without resource data</span></span>

<span data-ttu-id="66660-150">O conteúdo a seguir descreve as informações enviadas na solicitação de notificações sem dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="66660-150">The following payload describes the information sent in the request for notifications without resource data.</span></span> <span data-ttu-id="66660-151">Este conteúdo específico significa que um usuário foi adicionado a um chat.</span><span class="sxs-lookup"><span data-stu-id="66660-151">This particular payload signifies that a user has been added to a chat.</span></span>

```json
{
    "subscriptionId": "cae901f1-ad1d-41b1-95b7-37029ed327bf",
    "changeType": "Created",
    "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
    "clientState": "<<--SpecifiedClientState-->>",
    "subscriptionExpirationDateTime": "2021-06-03T10:58:54.7656077+00:00",
    "resource": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')/members('MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=')",
    "resourceData": {
        "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=",
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "@odata.id": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')/members('MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=')"
    }
}
```

<span data-ttu-id="66660-152">O **recurso** e a propriedades **@odata.id** pode ser usado para fazer chamadas para o Microsoft Graph para obter o conteúdo dos detalhes de membro do chat.</span><span class="sxs-lookup"><span data-stu-id="66660-152">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the chat member details.</span></span> <span data-ttu-id="66660-153">As chamadas GET sempre retornarão o estado atual dos detalhes de membro do chat.</span><span class="sxs-lookup"><span data-stu-id="66660-153">GET calls will always return the current state of the chat member details.</span></span> <span data-ttu-id="66660-154">Se os detalhes do membro do chat tiverem sido alterados entre o momento em que a notificação é enviada e quando os detalhes do membro do chat foram recuperados, a operação retornará os detalhes atualizados de membro do chat.</span><span class="sxs-lookup"><span data-stu-id="66660-154">If the chat member details has changed between when the notification is sent and when the chat member details were retrieved, the operation will return the updated chat member details.</span></span>

## <a name="see-also"></a><span data-ttu-id="66660-155">Confira também</span><span class="sxs-lookup"><span data-stu-id="66660-155">See also</span></span>
- [<span data-ttu-id="66660-156">Notificações de alteração do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="66660-156">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="66660-157">Visão geral da API do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="66660-157">Microsoft Teams API overview</span></span>](teams-concept-overview.md)