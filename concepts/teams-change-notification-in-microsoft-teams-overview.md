---
title: Alterar notificações para os recursos do Microsoft Teams usando Microsoft Graph
description: Saiba como obter notificações de alterações (criar, atualizar e excluir) para recursos no Microsoft Teams usando as APIs do Microsoft Graph
author: anandab-msft
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 9433a4c5ee000fa34e125440168b865f1bb16172
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430879"
---
# <a name="change-notifications-for-microsoft-teams-resources-using-microsoft-graph"></a><span data-ttu-id="50699-103">Alterar notificações para os recursos do Microsoft Teams usando Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="50699-103">Change notifications for Microsoft Teams resources using Microsoft Graph</span></span>

<span data-ttu-id="50699-104">As notificações de alteração habilitam você a assinar para receber alterações (criar, atualizar e excluir) um recurso.</span><span class="sxs-lookup"><span data-stu-id="50699-104">Change notifications enable you to subscribe to changes (create, update, and delete) to a resource.</span></span> <span data-ttu-id="50699-105">As notificações de alteração fornecem um modelo de baixa latência, permitindo que você mantenha uma [assinatura](/graph/api/resources/webhooks?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="50699-105">Change notifications provide a low latency model by allowing you to maintain a [subscription](/graph/api/resources/webhooks?preserve-view=true).</span></span> <span data-ttu-id="50699-106">Você também pode obter os dados do recurso nas notificações e, portanto, evitar chamar a API para obter o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="50699-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

> <span data-ttu-id="50699-107">**Observação:** o tempo máximo que uma assinatura pode durar é 60 minutos; entretanto, as assinaturas podem ser renovadas até que o chamador tenha permissão para acessar o recurso.</span><span class="sxs-lookup"><span data-stu-id="50699-107">**Note:** The maximum time a subscription can last is 60 minutes; however, subscriptions can be renewed until the caller has permissions to access to resource.</span></span>

## <a name="change-notification-types"></a><span data-ttu-id="50699-108">Tipoos de notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="50699-108">Change notification types</span></span>
<span data-ttu-id="50699-109">O Microsoft Teams dá suporte a dois tipos de notificações de alteração:</span><span class="sxs-lookup"><span data-stu-id="50699-109">Microsoft Teams supports two types of change notifications:</span></span>
- <span data-ttu-id="50699-110">**Altere a notificação para controlar todas as alterações relacionadas a um recurso no locatário** – por exemplo, você pode assinar alterações em mensagens em qualquer canal no locatário e ser notificado sempre que uma mensagem for criada, atualizada ou excluída em qualquer canal no locatário.</span><span class="sxs-lookup"><span data-stu-id="50699-110">**Change notification to track all changes related to a resource across the tenant** - for example, you can subscribe to changes in messages in any channel across the tenant and get notified whenever a message is created, updated, or deleted in any channel in the tenant.</span></span>
- <span data-ttu-id="50699-111">**Altere a notificação para controlar todas as alterações de um recurso específico** - por exemplo, você pode assinar alterações em mensagens em um canal específico e ser notificado sempre que uma mensagem for criada, atualizada ou excluída nesse canal.</span><span class="sxs-lookup"><span data-stu-id="50699-111">**Change notification to track all changes for a specific resource** - for example, you can subscribe to changes in messages in a particular channel and get notified whenever a message is created, updated, or deleted in that channel.</span></span>

<span data-ttu-id="50699-112">Para obter detalhes sobre quais recursos dão suporte a quais tipos de notificações de alteração, consulte [Notificações de Alteração do Microsoft Graph](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="50699-112">For details about which resources support which types of change notifications, see [Microsoft Graph change notifications](webhooks.md).</span></span>
 

## <a name="notification-payloads"></a><span data-ttu-id="50699-113">Cargas de notificação</span><span class="sxs-lookup"><span data-stu-id="50699-113">Notification payloads</span></span>

<span data-ttu-id="50699-114">Dependendo da sua assinatura, você pode receber a notificação com dados de recursos ou sem ele.</span><span class="sxs-lookup"><span data-stu-id="50699-114">Depending on your subscription, you can either get the notification with resource data, or without resource data.</span></span> <span data-ttu-id="50699-115">Assinar com dados de recursos permite que você receba a carga da mensagem junto com a notificação, o que remove a necessidade de ligar de volta e obter o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="50699-115">Subscribing with resource data allows you to get the message payload along with the notification, which removes the need to call back and get the content.</span></span>

### <a name="notifications-with-resource-data"></a><span data-ttu-id="50699-116">Notificações com dados de recursos</span><span class="sxs-lookup"><span data-stu-id="50699-116">Notifications with resource data</span></span>

<span data-ttu-id="50699-117">Para notificações com dados de recursos, a carga se parece com a seguinte.</span><span class="sxs-lookup"><span data-stu-id="50699-117">For notifications with resource data, the payload looks like the following.</span></span>  <span data-ttu-id="50699-118">Essa carga é para uma notificação correspondente ao recurso de mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="50699-118">This payload is for a notification corresponding to the chat message resource.</span></span> <span data-ttu-id="50699-119">A notificação real inclui as propriedades **resource** e **resourceData**, que representam o recurso que disparou a notificação.</span><span class="sxs-lookup"><span data-stu-id="50699-119">The actual notification includes the **resource** and **resourceData** properties, which represent the resource that has triggered the notification.</span></span>

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')",
        "resourceData": {
            "id": "1612289765949",
            "@odata.type": "#Microsoft.Graph.chatMessage",
            "@odata.id": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')"
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

<span data-ttu-id="50699-120">Para obter detalhes sobre como validar tokens e descriptografar a carga útil, consulte [Definir notificações de alteração que incluem dados de recursos](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="50699-120">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="50699-121">A carga de notificação descriptografada parece com a seguinte.</span><span class="sxs-lookup"><span data-stu-id="50699-121">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="50699-122">A carga descriptografada para o exemplo anterior está em conformidade com o esquema [chatMessage](/graph/api/resources/chatMessage?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="50699-122">The decrypted payload for the previous example conforms to the [chatMessage](/graph/api/resources/chatMessage?preserve-view=true) schema.</span></span> <span data-ttu-id="50699-123">A carga é semelhante à devolvida pelas operações GET.</span><span class="sxs-lookup"><span data-stu-id="50699-123">The payload is similar to that returned by GET operations.</span></span>

```json
{
  "id": "1612289992105",
  "replyToId": null,
  "etag": "1612289992105",
  "messageType": "message",
  "createdDateTime": "2021-02-02T18:19:52Z",
  "lastModifiedDateTime": "2021-02-02T18:19:52.105Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
      "displayName": "Ramjot Singh",
      "userIdentityType": "aadUser"
    },
    "conversation": null
  },
  "body": {
    "contentType": "text",
    "content": "test"
  },
  "channelIdentity": null,
  "attachments": [],
  "mentions": [],
  "policyViolation": null,
  "reactions": [],
  "replies": [],
  "hostedContents": []
}
```

### <a name="notifications-without-resource-data"></a><span data-ttu-id="50699-124">Notificações sem dados de recursos</span><span class="sxs-lookup"><span data-stu-id="50699-124">Notifications without resource data</span></span>

<span data-ttu-id="50699-125">Notificações sem dados de recurso fornecem informações suficientes para fazer chamadas GET para obter o recurso.</span><span class="sxs-lookup"><span data-stu-id="50699-125">Notifications without resource data give you enough information to make GET calls to get the resource.</span></span> <span data-ttu-id="50699-126">As assinaturas para notificações sem dados de recursos não exigem um certificado de criptografia (porque os dados reais dos recursos não são enviados).</span><span class="sxs-lookup"><span data-stu-id="50699-126">Subscriptions for notifications without resource data don't require an encryption certificate (because actual resource data is not sent over).</span></span>

<span data-ttu-id="50699-127">A carga parece ser a seguinte.</span><span class="sxs-lookup"><span data-stu-id="50699-127">The payload looks like the following.</span></span> <span data-ttu-id="50699-128">Este conteúdo é para uma mensagem enviada em um canal.</span><span class="sxs-lookup"><span data-stu-id="50699-128">This payload is for a message sent in a channel.</span></span>

```json
{
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",  
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')",
  "resourceData": {
    "id": "1612293113399",
    "@odata.type": "#Microsoft.Graph.chatMessage",
    "@odata.id": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')"
  }
}
```
<span data-ttu-id="50699-129">O exemplo anterior acima mostra uma notificação que corresponde a um recurso de mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="50699-129">Previous example above shows a notification that corresponds to a chat message resource.</span></span> <span data-ttu-id="50699-130">A notificação real inclui as propriedades **resource** e **resourceData**, que representam o recurso que disparou a notificação.</span><span class="sxs-lookup"><span data-stu-id="50699-130">The actual notification includes the **resource** and **resourceData** properties, which represent the resource that has triggered the notification.</span></span> <span data-ttu-id="50699-131">As propriedades **recurso** e **@odata.id** podem ser usados para fazer chamadas para o Microsoft Graph para obter a carga do recurso.</span><span class="sxs-lookup"><span data-stu-id="50699-131">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload of the resource.</span></span>

> <span data-ttu-id="50699-132">**Observe** As chamadas GET sempre retornarão o estado atual do recurso.</span><span class="sxs-lookup"><span data-stu-id="50699-132">**Note** GET calls will always return the current state of the resource.</span></span> <span data-ttu-id="50699-133">Se o recurso for alterado entre quando a notificação for enviada e quando o recurso for recuperado, a operação retornará o recurso atualizado.</span><span class="sxs-lookup"><span data-stu-id="50699-133">If the resource is changed between when the notification is sent and when the resource is retrieved, the operation will return the updated resource.</span></span>

## <a name="see-also"></a><span data-ttu-id="50699-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="50699-134">See also</span></span>
- [<span data-ttu-id="50699-135">Notificações de alteração do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="50699-135">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="50699-136">Visão geral da API do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="50699-136">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
