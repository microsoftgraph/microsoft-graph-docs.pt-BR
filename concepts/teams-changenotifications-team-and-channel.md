---
title: Obter notificações de alteração para equipes e canais usando o Microsoft Graph
description: Saiba como obter notificações de alterações (criar, atualizar e excluir) para equipes e canais usando as APIs do Microsoft Graph.
author: anandab
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 4d04333818fa57664664675feb4683465c4b63c6
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941547"
---
# <a name="get-change-notifications-for-teams-and-channels-using-microsoft-graph"></a><span data-ttu-id="828b7-103">Obter notificações de alteração para equipes e canais usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="828b7-103">Get change notifications for teams and channels using Microsoft Graph</span></span>

<span data-ttu-id="828b7-104">As notificações de alteração permitem que você se inscreva para alterações (criar, atualizar e excluir) de equipes e canais.</span><span class="sxs-lookup"><span data-stu-id="828b7-104">Change notifications enable you to subscribe to changes (create, update, and delete) to teams and channels.</span></span> <span data-ttu-id="828b7-105">Você será notificado sempre que uma equipe ou canal for criado, atualizado ou excluído.</span><span class="sxs-lookup"><span data-stu-id="828b7-105">You can get notified whenever a team or channel is created, updated, or deleted.</span></span> <span data-ttu-id="828b7-106">Você também receberá os dados de recursos nas notificações e, portanto, evitará chamar a API para obter a carga útil.</span><span class="sxs-lookup"><span data-stu-id="828b7-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

## <a name="subscribe-to-changes-in-any-team-at-tenant-level"></a><span data-ttu-id="828b7-107">Inscrever-se para alterações em qualquer equipe no nível de locatário</span><span class="sxs-lookup"><span data-stu-id="828b7-107">Subscribe to changes in any team at tenant level</span></span>

<span data-ttu-id="828b7-108">Para obter notificações de alteração para todas as alterações (criar, atualizar e excluir) relacionadas a qualquer equipe de um locatário, inscreva-se em `/teams`.</span><span class="sxs-lookup"><span data-stu-id="828b7-108">To get change notifications for all changes (create, update, and delete) related to any team in a tenant, subscribe to `/teams`.</span></span> <span data-ttu-id="828b7-109">Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.</span><span class="sxs-lookup"><span data-stu-id="828b7-109">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="828b7-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="828b7-110">Permissions</span></span>

|<span data-ttu-id="828b7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="828b7-111">Permission type</span></span>      | <span data-ttu-id="828b7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="828b7-112">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="828b7-113">Versões com suporte</span><span class="sxs-lookup"><span data-stu-id="828b7-113">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="828b7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="828b7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="828b7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828b7-115">Not supported.</span></span> | <span data-ttu-id="828b7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828b7-116">Not supported.</span></span> |
|<span data-ttu-id="828b7-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="828b7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="828b7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828b7-118">Not supported.</span></span>    | <span data-ttu-id="828b7-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828b7-119">Not supported.</span></span> |
|<span data-ttu-id="828b7-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="828b7-120">Application</span></span> | <span data-ttu-id="828b7-121">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="828b7-121">Team.ReadBasic.All, TeamSettings.Read.All</span></span>   | <span data-ttu-id="828b7-122">beta</span><span class="sxs-lookup"><span data-stu-id="828b7-122">beta</span></span>|

### <a name="example"></a><span data-ttu-id="828b7-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="828b7-123">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-a-particular-team"></a><span data-ttu-id="828b7-124">Inscrever-se para alterações em uma equipe em particular</span><span class="sxs-lookup"><span data-stu-id="828b7-124">Subscribe to changes in a particular team</span></span>


<span data-ttu-id="828b7-125">Para obter notificações de alteração para todas as alterações relacionadas a uma equipe em particular de um locatário, inscreva-se em `/teams/{id}`.</span><span class="sxs-lookup"><span data-stu-id="828b7-125">To get change notifications for all changes related to a particular team in a tenant, subscribe to `/teams/{id}`.</span></span> <span data-ttu-id="828b7-126">Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.</span><span class="sxs-lookup"><span data-stu-id="828b7-126">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="828b7-127">Permissões</span><span class="sxs-lookup"><span data-stu-id="828b7-127">Permissions</span></span>

|<span data-ttu-id="828b7-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="828b7-128">Permission type</span></span>      | <span data-ttu-id="828b7-129">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="828b7-129">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="828b7-130">Versões com suporte</span><span class="sxs-lookup"><span data-stu-id="828b7-130">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="828b7-131">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="828b7-131">Delegated (work or school account)</span></span> | <span data-ttu-id="828b7-132">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="828b7-132">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="828b7-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828b7-133">Not supported.</span></span> |
|<span data-ttu-id="828b7-134">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="828b7-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="828b7-135">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828b7-135">Not supported.</span></span>    | <span data-ttu-id="828b7-136">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828b7-136">Not supported.</span></span> |
|<span data-ttu-id="828b7-137">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="828b7-137">Application</span></span> | <span data-ttu-id="828b7-138">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="828b7-138">Team.ReadBasic.All, TeamSettings.Read.All</span></span>    | <span data-ttu-id="828b7-139">beta</span><span class="sxs-lookup"><span data-stu-id="828b7-139">beta</span></span> |

### <a name="example"></a><span data-ttu-id="828b7-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="828b7-140">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


## <a name="subscribe-to-changes-in-any-channel-at-tenant-level"></a><span data-ttu-id="828b7-141">Inscrever-se para alterações em qualquer canal no nível de locatário</span><span class="sxs-lookup"><span data-stu-id="828b7-141">Subscribe to changes in any channel at tenant level</span></span>

<span data-ttu-id="828b7-142">Para obter notificações de alteração para todas as alterações (criar, atualizar e excluir) relacionadas a qualquer canal de um locatário, inscreva-se em `/teams/getAllChannels`.</span><span class="sxs-lookup"><span data-stu-id="828b7-142">To get change notifications for all changes (create, update, and delete) related to any channel in a tenant, subscribe to `/teams/getAllChannels`.</span></span> <span data-ttu-id="828b7-143">Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.</span><span class="sxs-lookup"><span data-stu-id="828b7-143">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

><span data-ttu-id="828b7-144">**Observação:** Não há suporte para canais privados.</span><span class="sxs-lookup"><span data-stu-id="828b7-144">**Note:** Private channels aren't supported.</span></span>

### <a name="permissions"></a><span data-ttu-id="828b7-145">Permissões</span><span class="sxs-lookup"><span data-stu-id="828b7-145">Permissions</span></span>

|<span data-ttu-id="828b7-146">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="828b7-146">Permission type</span></span>      | <span data-ttu-id="828b7-147">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="828b7-147">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="828b7-148">Versões com suporte</span><span class="sxs-lookup"><span data-stu-id="828b7-148">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="828b7-149">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="828b7-149">Delegated (work or school account)</span></span> | <span data-ttu-id="828b7-150">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828b7-150">Not supported.</span></span> | <span data-ttu-id="828b7-151">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828b7-151">Not supported.</span></span> |
|<span data-ttu-id="828b7-152">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="828b7-152">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="828b7-153">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828b7-153">Not supported.</span></span>    | <span data-ttu-id="828b7-154">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828b7-154">Not supported.</span></span> |
|<span data-ttu-id="828b7-155">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="828b7-155">Application</span></span> | <span data-ttu-id="828b7-156">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="828b7-156">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> | <span data-ttu-id="828b7-157">beta</span><span class="sxs-lookup"><span data-stu-id="828b7-157">beta</span></span> |

### <a name="example"></a><span data-ttu-id="828b7-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="828b7-158">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/getAllChannels",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-any-channel-of-a-particular-team"></a><span data-ttu-id="828b7-159">Inscrever-se para alterações em qualquer canal em particular</span><span class="sxs-lookup"><span data-stu-id="828b7-159">Subscribe to changes in any channel of a particular team</span></span>


<span data-ttu-id="828b7-160">Para obter notificações de alteração para todas as alterações relacionadas a qualquer canal em particular, inscreva-se em `/teams/{id}/channels`.</span><span class="sxs-lookup"><span data-stu-id="828b7-160">To get change notifications for all changes related to any channel in a particular team, subscribe to `/teams/{id}/channels`.</span></span> <span data-ttu-id="828b7-161">Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.</span><span class="sxs-lookup"><span data-stu-id="828b7-161">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="828b7-162">Permissões</span><span class="sxs-lookup"><span data-stu-id="828b7-162">Permissions</span></span>

|<span data-ttu-id="828b7-163">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="828b7-163">Permission type</span></span>      | <span data-ttu-id="828b7-164">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="828b7-164">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="828b7-165">Versões com suporte</span><span class="sxs-lookup"><span data-stu-id="828b7-165">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="828b7-166">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="828b7-166">Delegated (work or school account)</span></span> | <span data-ttu-id="828b7-167">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="828b7-167">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> | <span data-ttu-id="828b7-168">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828b7-168">Not supported.</span></span> |
|<span data-ttu-id="828b7-169">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="828b7-169">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="828b7-170">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828b7-170">Not supported.</span></span>    | <span data-ttu-id="828b7-171">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828b7-171">Not supported.</span></span> |
|<span data-ttu-id="828b7-172">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="828b7-172">Application</span></span> | <span data-ttu-id="828b7-173">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="828b7-173">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>   | <span data-ttu-id="828b7-174">beta</span><span class="sxs-lookup"><span data-stu-id="828b7-174">beta</span></span> |

### <a name="example"></a><span data-ttu-id="828b7-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="828b7-175">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


### <a name="notifications-with-resource-data"></a><span data-ttu-id="828b7-176">Notificações com dados de recursos</span><span class="sxs-lookup"><span data-stu-id="828b7-176">Notifications with resource data</span></span>

<span data-ttu-id="828b7-177">Para notificações com dados de recursos, a carga se parece com a seguinte.</span><span class="sxs-lookup"><span data-stu-id="828b7-177">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="828b7-178">Essa carga é para uma alteração de propriedade em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="828b7-178">This payload is for a property change in a team.</span></span>

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')",
        "resourceData": {
            "id": "1612289765949",
            "@odata.type": "#Microsoft.Graph.Team",
            "@odata.id": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')"
        },
        "encryptedContent": {
            "data": "<<--EncryptedContent-->",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
    }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```



<span data-ttu-id="828b7-179">A carga de notificação descriptografada parece com o seguinte.</span><span class="sxs-lookup"><span data-stu-id="828b7-179">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="828b7-180">A carga está de acordo com o esquema de [equipes](/graph/api/resources/team?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="828b7-180">The payload conforms to the [teams](/graph/api/resources/team?preserve-view=true) schema.</span></span> <span data-ttu-id="828b7-181">A carga é semelhante à devolvida pelas operações GET.</span><span class="sxs-lookup"><span data-stu-id="828b7-181">The payload is similar to that returned by GET operations.</span></span>

><span data-ttu-id="828b7-182">**Observação:** [discoverySettings](/graph/api/resources/teamdiscoverysettings?preserve-view=true) [classSettings](/graph/api/resources/teamclasssettings?preserve-view=true) não são expostos em dados de carga.</span><span class="sxs-lookup"><span data-stu-id="828b7-182">**Note:** [discoverySettings](/graph/api/resources/teamdiscoverysettings?preserve-view=true) and [classSettings](/graph/api/resources/teamclasssettings?preserve-view=true) aren't exposed in payload data.</span></span>

```json
{
  "id": "4c533ad3-e1dd-4277-a672-92ab64ed225c",
  "createdDateTime": "2021-03-18T10:31:14.597Z",
  "displayName": "Sample name",
  "description": "Sample description",
  "internalId": "19:2077546f765a42c1ba71236f4df70aa2@thread.tacv2",
  "specialization": "none",
  "visibility": "public",
  "webUrl": "https://teams.microsoft.com/l/team/19:2077546f724a42c1ba71236f4df79aa2%40thread.tacv2/conversations?groupId=4c533ad3-e1dd-4277-a672-92ab64ed225c&tenantId=0f2e8f59-862a-483b-9ca8-82a10665e17d",
  "isArchived": false,
  "isMembershipLimitedToOwners": false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowCreatePrivateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true
  },
  "guestSettings": {
    "allowCreateUpdateChannels": false,
    "allowDeleteChannels": false
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "moderate",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```


<span data-ttu-id="828b7-183">Para notificações com dados de recursos, a carga se parece com o seguinte.</span><span class="sxs-lookup"><span data-stu-id="828b7-183">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="828b7-184">Esta carga é para uma alteração de propriedade em um canal.</span><span class="sxs-lookup"><span data-stu-id="828b7-184">This payload is for a property change in a channel.</span></span>

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')/channels('19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2')",
        "resourceData": {
            "id": "19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2",
            "@odata.type": "#Microsoft.Graph.Channel",
            "@odata.id": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')/channels('19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2')"
        },
        "encryptedContent": {
            "data": "<<--EncryptedContent-->",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
    }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```
  

<span data-ttu-id="828b7-185">A carga de notificação descriptografada parece com o seguinte.</span><span class="sxs-lookup"><span data-stu-id="828b7-185">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="828b7-186">A carga está de acordo com o esquema de [canais](/graph/api/resources/channel?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="828b7-186">The payload conforms to the [channel](/graph/api/resources/channel?preserve-view=true) schema.</span></span> <span data-ttu-id="828b7-187">A carga é semelhante à devolvida pelas operações GET.</span><span class="sxs-lookup"><span data-stu-id="828b7-187">The payload is similar to that returned by GET operations.</span></span>

```json
{
  "id": "19:a3f841d969cd4ae0a7cbe847fc10b371@thread.tacv2",
  "createdDateTime": "2020-02-14T01:10:03.592Z",
  "displayName": "General",
  "description": "Sample Channel description",
  "isFavoriteByDefault": true,
  "email": "",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3Aa3f841d969cd4ae0a7cbe847fc10b371%40thread.tacv2/General?groupId=7ed9bdab-9c7d-4c10-a25d-3f4ff0e34577&tenantId=0f2d8f49-862a-493b-9ca8-82a10637e17d",
  "membershipType": "standard",
  "moderationSettings": null
}
```


### <a name="notifications-without-resource-data"></a><span data-ttu-id="828b7-188">Notificações sem dados de recursos</span><span class="sxs-lookup"><span data-stu-id="828b7-188">Notifications without resource data</span></span>

<span data-ttu-id="828b7-189">Notificações sem dados de recursos dão informações suficientes para fazer chamadas GET para obter o conteúdo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="828b7-189">Notifications without resource data give you enough information to make GET calls to get the message content.</span></span> <span data-ttu-id="828b7-190">As assinaturas para notificações sem dados de recursos não exigem um certificado de criptografia (porque os dados reais dos recursos não são enviados).</span><span class="sxs-lookup"><span data-stu-id="828b7-190">Subscriptions for notifications without resource data don't require an encryption certificate (because actual resource data is not sent over).</span></span>

<span data-ttu-id="828b7-191">Para notificações sem dados de recursos, a carga se parecerá com o seguinte.</span><span class="sxs-lookup"><span data-stu-id="828b7-191">For notifications without resource data, the payload looks like the following.</span></span> <span data-ttu-id="828b7-192">Essa carga é para uma alteração de propriedade em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="828b7-192">This payload is for a property change in a team.</span></span>

```json
{
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')",
  "resourceData": {
    "id": "1612293113399",
    "@odata.type": "#Microsoft.Graph.Teams",
    "@odata.id": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')"
  }
}
```

<span data-ttu-id="828b7-193">As propriedades **recurso** e **@odata.id** podem ser usados para fazer chamadas para o Microsoft Graph para obter o conteúdo para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="828b7-193">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the message.</span></span> <span data-ttu-id="828b7-194">As chamadas GET sempre retornarão o estado atual da mensagem.</span><span class="sxs-lookup"><span data-stu-id="828b7-194">GET calls will always return the current state of the message.</span></span> <span data-ttu-id="828b7-195">Se a mensagem for alterada entre quando a notificação for enviada e quando a mensagem for recuperada, a operação retornará a mensagem atualizada.</span><span class="sxs-lookup"><span data-stu-id="828b7-195">If the message is changed between when the notification is sent and when the message is retrieved, the operation will return the updated message.</span></span>


><span data-ttu-id="828b7-196">**Observação:** o endereço de email do canal não retorna na carga.</span><span class="sxs-lookup"><span data-stu-id="828b7-196">**Note:** Channel email address isn't returned in the payload.</span></span>

<span data-ttu-id="828b7-197">Para notificações sem dados de recursos, a carga se parecerá com o seguinte.</span><span class="sxs-lookup"><span data-stu-id="828b7-197">For notifications without resource data, the payload looks like the following.</span></span> <span data-ttu-id="828b7-198">Essa carga é para uma alteração de propriedade em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="828b7-198">This payload is for a property change in a team.</span></span>

```json
{
  "id": "19:a3f841d969cd4ae0a7cbe847fc10b371@thread.tacv2",
  "createdDateTime": "2020-02-14T01:10:03.592Z",
  "displayName": "General",
  "description": "Sample Channel description",
  "isFavoriteByDefault": true,
  "email": "",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3Aa3f841d969cd4ae0a7cbe847fc10b371%40thread.tacv2/General?groupId=7ed9bdab-9c7d-4c10-a25d-3f4ff0e34577&tenantId=0f2d8f49-862a-493b-9ca8-82a10637e17d",
  "membershipType": "standard",
  "moderationSettings": null
}
```


## <a name="see-also"></a><span data-ttu-id="828b7-199">Confira também</span><span class="sxs-lookup"><span data-stu-id="828b7-199">See also</span></span>
- [<span data-ttu-id="828b7-200">Notificações de alteração do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="828b7-200">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="828b7-201">Visão geral da API do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="828b7-201">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
