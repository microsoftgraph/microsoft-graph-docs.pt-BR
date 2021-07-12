---
title: Obtenha notificações de alteração para chats usando o Microsoft Graph
description: Saiba como obter notificações de alterações (criar e atualizar) para chats usando as APIs do Microsoft Graph.
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 246a0236b705f98835a4c8131a04e28d3d8c846c
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53367018"
---
# <a name="get-change-notifications-for-chats-using-microsoft-graph"></a><span data-ttu-id="b3872-103">Obtenha notificações de alteração para chats usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b3872-103">Get change notifications for chats using Microsoft Graph</span></span>

<span data-ttu-id="b3872-104">As notificações de alteração permitem que você se inscreva para receber alterações (criar e atualizar) nos chats.</span><span class="sxs-lookup"><span data-stu-id="b3872-104">Change notifications enable you to subscribe to changes (create and update) to chats.</span></span> <span data-ttu-id="b3872-105">Você pode ser notificado sempre que um chat for criado ou atualizado.</span><span class="sxs-lookup"><span data-stu-id="b3872-105">You can get notified whenever a chat is created or updated.</span></span> <span data-ttu-id="b3872-106">Você também pode obter os dados do recurso nas notificações e, portanto, evitar chamar a API para obter o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b3872-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

## <a name="subscribe-to-changes-in-any-chat-at-tenant-level"></a><span data-ttu-id="b3872-107">Inscrever-se para alterações em qualquer chat a nível de locatário</span><span class="sxs-lookup"><span data-stu-id="b3872-107">Subscribe to changes in any chat at tenant level</span></span>

<span data-ttu-id="b3872-108">Para obter notificações de alteração para todas as alterações (criar e atualizar) relacionadas a qualquer chat em um locatário, inscreva-se em `/chats`.</span><span class="sxs-lookup"><span data-stu-id="b3872-108">To get change notifications for all changes (create and update) related to any chat in a tenant, subscribe to `/chats`.</span></span> <span data-ttu-id="b3872-109">Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.</span><span class="sxs-lookup"><span data-stu-id="b3872-109">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="b3872-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3872-110">Permissions</span></span>

|<span data-ttu-id="b3872-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3872-111">Permission type</span></span>      | <span data-ttu-id="b3872-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3872-112">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="b3872-113">Versões com suporte</span><span class="sxs-lookup"><span data-stu-id="b3872-113">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="b3872-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3872-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b3872-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3872-115">Not supported.</span></span> | <span data-ttu-id="b3872-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3872-116">Not supported.</span></span> |
|<span data-ttu-id="b3872-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3872-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3872-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3872-118">Not supported.</span></span>    | <span data-ttu-id="b3872-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3872-119">Not supported.</span></span> |
|<span data-ttu-id="b3872-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3872-120">Application</span></span> | <span data-ttu-id="b3872-121">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3872-121">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span>   | <span data-ttu-id="b3872-122">beta</span><span class="sxs-lookup"><span data-stu-id="b3872-122">beta</span></span>|

### <a name="example"></a><span data-ttu-id="b3872-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3872-123">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-a-particular-chat"></a><span data-ttu-id="b3872-124">Inscrever-se para alterações em um chat específico</span><span class="sxs-lookup"><span data-stu-id="b3872-124">Subscribe to changes in a particular chat</span></span>


<span data-ttu-id="b3872-125">Para obter notificações de alteração para todas as alterações relacionadas a um chat específico, inscreva-se em `/chats/{id}`.</span><span class="sxs-lookup"><span data-stu-id="b3872-125">To get change notifications for all changes related to a particular chat, subscribe to `/chats/{id}`.</span></span> <span data-ttu-id="b3872-126">Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.</span><span class="sxs-lookup"><span data-stu-id="b3872-126">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="b3872-127">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3872-127">Permissions</span></span>

|<span data-ttu-id="b3872-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3872-128">Permission type</span></span>      | <span data-ttu-id="b3872-129">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3872-129">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="b3872-130">Versões com suporte</span><span class="sxs-lookup"><span data-stu-id="b3872-130">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="b3872-131">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3872-131">Delegated (work or school account)</span></span> | <span data-ttu-id="b3872-132">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3872-132">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="b3872-133">beta</span><span class="sxs-lookup"><span data-stu-id="b3872-133">beta</span></span> |
|<span data-ttu-id="b3872-134">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3872-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3872-135">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3872-135">Not supported.</span></span>    | <span data-ttu-id="b3872-136">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3872-136">Not supported.</span></span> |
|<span data-ttu-id="b3872-137">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3872-137">Application</span></span> | <span data-ttu-id="b3872-138">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3872-138">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> | <span data-ttu-id="b3872-139">beta</span><span class="sxs-lookup"><span data-stu-id="b3872-139">beta</span></span> |

> <span data-ttu-id="b3872-140">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="b3872-140">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="example"></a><span data-ttu-id="b3872-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3872-141">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


### <a name="notifications-with-resource-data"></a><span data-ttu-id="b3872-142">Notificações com dados de recursos</span><span class="sxs-lookup"><span data-stu-id="b3872-142">Notifications with resource data</span></span>

<span data-ttu-id="b3872-143">Para notificações com dados de recursos, a carga se parece com a seguinte.</span><span class="sxs-lookup"><span data-stu-id="b3872-143">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="b3872-144">Este conteúdo é para uma alteração de propriedade em um chat.</span><span class="sxs-lookup"><span data-stu-id="b3872-144">This payload is for a property change in a chat.</span></span>

```json
{
    "value": [{
        "subscriptionId": "352887e3-9be0-4b6f-a4e6-dec118d857db",
        "changeType": "Created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-06-03T09:50:37.719033+00:00",
        "resource": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')",
        "resourceData": {
            "id": "19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces",
            "@odata.type": "#microsoft.graph.chat",
            "@odata.id": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')"
        },
        "EncryptedContent": {
            "data": "<<--EncryptedContent-->>",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        }
            "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
        }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

<span data-ttu-id="b3872-145">Para obter detalhes sobre como validar tokens e descriptografar a carga útil, consulte [Definir notificações de alteração que incluem dados de recursos](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="b3872-145">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="b3872-146">A carga de notificação descriptografada parece com a seguinte.</span><span class="sxs-lookup"><span data-stu-id="b3872-146">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="b3872-147">O conteúdo está de acordo com o esquema de [chats](/graph/api/resources/chat?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="b3872-147">The payload conforms to the [chats](/graph/api/resources/chat?preserve-view=true) schema.</span></span> <span data-ttu-id="b3872-148">A carga é semelhante à devolvida pelas operações GET.</span><span class="sxs-lookup"><span data-stu-id="b3872-148">The payload is similar to that returned by GET operations.</span></span>

```json
{
  "id": "19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces",
  "topic": null,
  "createdDateTime": "2021-06-03T14:25:04+05:30",
  "lastUpdatedDateTime": "2021-06-03T14:25:04.387Z",
  "chatType": "oneOnOne",
  "members": [
    {
      "userId": "976f4b31-fd01-4e0b-9178-29cc40c14438",
      "email": null,
      "tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
      "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyM5NzZmNGIzMS1mZDAxLTRlMGItOTE3OC0yOWNjNDBjMTQ0Mzg=",
      "roles": [],
      "displayName": null,
      "visibleHistoryStartDateTime": "1970-01-01T00:00:00Z",
      "user": null
    },
    {
      "userId": "ee723d3d-22d0-4394-9c32-5764d68f4672",
      "email": null,
      "tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
      "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyNlZTcyM2QzZC0yMmQwLTQzOTQtOWMzMi01NzY0ZDY4ZjQ2NzI=",
      "roles": [],
      "displayName": null,
      "visibleHistoryStartDateTime": "1970-01-01T00:00:00Z",
      "user": null
    }
  ],
  "messages": [],
  "installedApps": [],
  "tabs": [],
  "permissionGrants": [],
  "operations": []
}
```

### <a name="notifications-without-resource-data"></a><span data-ttu-id="b3872-149">Notificações sem dados de recursos</span><span class="sxs-lookup"><span data-stu-id="b3872-149">Notifications without resource data</span></span>

<span data-ttu-id="b3872-150">O conteúdo a seguir descreve as informações enviadas na solicitação de notificações sem dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="b3872-150">The following payload describes the information sent in the request for notifications without resource data.</span></span> <span data-ttu-id="b3872-151">Este conteúdo específico significa que um novo chat foi criado.</span><span class="sxs-lookup"><span data-stu-id="b3872-151">This particular payload signifies that a new chat has been created.</span></span>

```json
{
    "subscriptionId": "8d85051d-779d-45bc-be92-e433f0a5d8ac",
    "changeType": "Created",
    "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
    "clientState": "<<--SpecifiedClientState-->>",
    "subscriptionExpirationDateTime": "2021-06-03T10:26:09.8959595+00:00",
    "resource": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')",
    "resourceData": {
        "id": "19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces",
        "@odata.type": "#microsoft.graph.chat",
        "@odata.id": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')"
    }
}
```

<span data-ttu-id="b3872-152">O **recurso** e a propriedades **@odata.id** pode ser usado para fazer chamadas para o Microsoft Graph para obter o conteúdo dos detalhes do chat.</span><span class="sxs-lookup"><span data-stu-id="b3872-152">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the chat details.</span></span> <span data-ttu-id="b3872-153">As chamadas GET sempre retornarão o estado atual dos detalhes do chat.</span><span class="sxs-lookup"><span data-stu-id="b3872-153">GET calls will always return the current state of the chat details.</span></span> <span data-ttu-id="b3872-154">Se os detalhes do bate-papo foram atualizados entre o momento em que a notificação é enviada e quando os detalhes do chat foram recuperados, a operação retornará os detalhes atualizados do chat.</span><span class="sxs-lookup"><span data-stu-id="b3872-154">If the chat details were updated between when the notification is sent and when the chat details were retrieved, the operation will return the updated chat details.</span></span>

## <a name="see-also"></a><span data-ttu-id="b3872-155">Confira também</span><span class="sxs-lookup"><span data-stu-id="b3872-155">See also</span></span>
- [<span data-ttu-id="b3872-156">Notificações de alteração do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b3872-156">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="b3872-157">Visão geral da API do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b3872-157">Microsoft Teams API overview</span></span>](teams-concept-overview.md)