---
title: Criar e enviar uma notificação
description: Criar e enviar uma notificação direcionada a um usuário por meio do Microsoft Graph.
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 6062153c1eaff68a19cd5b27ac10efa9bacafb93
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937921"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="f0046-103">Criar e enviar uma notificação</span><span class="sxs-lookup"><span data-stu-id="f0046-103">Create and send a notification</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0046-104">Criar e enviar uma notificação direcionada a um usuário por meio do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f0046-104">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="f0046-105">A notificação é armazenada no repositório de feeds de notificação do Microsoft Graph e é enviada a todos os clientes de aplicativos em todos os pontos de extremidade do dispositivo nos quais o usuário está conectado.</span><span class="sxs-lookup"><span data-stu-id="f0046-105">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  

## <a name="permissions"></a><span data-ttu-id="f0046-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f0046-106">Permissions</span></span>
<span data-ttu-id="f0046-107">O serviço de aplicativo não requer nenhuma permissão adicional para postar notificações para o usuário de destino.</span><span class="sxs-lookup"><span data-stu-id="f0046-107">Your application service does not require any additional permissions to post notifications to your targeted user.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="f0046-108">Se você optar por publicar notificações em nome de um usuário via permissões delegadas, uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f0046-108">If you choose to post notifications on behalf of a user via delegated permissions instead, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="f0046-109">Não recomendamos esta opção para a criação de notificações.</span><span class="sxs-lookup"><span data-stu-id="f0046-109">We don't recommend this option for creating notifications.</span></span> <span data-ttu-id="f0046-110">Se quiser saber mais, incluindo como escolher permissões, consulte [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0046-110">If you'd like to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0046-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0046-111">Permission type</span></span>      | <span data-ttu-id="f0046-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0046-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0046-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0046-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f0046-114">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="f0046-114">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="f0046-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0046-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0046-116">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="f0046-116">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="f0046-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0046-117">Application</span></span> | <span data-ttu-id="f0046-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0046-118">Not supported.</span></span>|



## <a name="http-request"></a><span data-ttu-id="f0046-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0046-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="f0046-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0046-120">Request headers</span></span>
|<span data-ttu-id="f0046-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f0046-121">Name</span></span> | <span data-ttu-id="f0046-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0046-122">Type</span></span> | <span data-ttu-id="f0046-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0046-123">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="f0046-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0046-124">Authorization</span></span> | <span data-ttu-id="f0046-125">string</span><span class="sxs-lookup"><span data-stu-id="f0046-125">string</span></span> |<span data-ttu-id="f0046-126">O cabeçalho de autorização é usado para passar as credenciais da parte de chamada.</span><span class="sxs-lookup"><span data-stu-id="f0046-126">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="f0046-127">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="f0046-127">Bearer {token}.</span></span> <span data-ttu-id="f0046-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0046-128">Required.</span></span> |
|<span data-ttu-id="f0046-129">X-UNS-ID</span><span class="sxs-lookup"><span data-stu-id="f0046-129">X-UNS-ID</span></span> | <span data-ttu-id="f0046-130">string</span><span class="sxs-lookup"><span data-stu-id="f0046-130">string</span></span> |<span data-ttu-id="f0046-131">O UserNotificationSubscriptionId retornado pelo serviço de notificação do Microsoft Graph após a criação de uma assinatura e é usado para direcionar o usuário específico.</span><span class="sxs-lookup"><span data-stu-id="f0046-131">The UserNotificationSubscriptionId that is returned by the Microsoft Graph notification service after creating a subscription and is used to target the specific user.</span></span> <span data-ttu-id="f0046-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0046-132">Required.</span></span> |
|<span data-ttu-id="f0046-133">Content-type</span><span class="sxs-lookup"><span data-stu-id="f0046-133">Content-type</span></span> | <span data-ttu-id="f0046-134">aplicado/JSON.</span><span class="sxs-lookup"><span data-stu-id="f0046-134">appliation/json.</span></span> <span data-ttu-id="f0046-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0046-135">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0046-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0046-136">Request body</span></span>
<span data-ttu-id="f0046-137">No corpo da solicitação, forneça uma representação JSON de um objeto [Notification](../resources/projectrome-notification.md) .</span><span class="sxs-lookup"><span data-stu-id="f0046-137">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f0046-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0046-138">Response</span></span>
<span data-ttu-id="f0046-139">Se tiver êxito, este método retornará `201 Created` um código de resposta que indica que a notificação foi criada e armazenada com êxito.</span><span class="sxs-lookup"><span data-stu-id="f0046-139">If successful, this method returns a `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> <span data-ttu-id="f0046-140">A notificação será subseqüentemente fanned a todos os pontos de extremidade especificados com uma assinatura válida.</span><span class="sxs-lookup"><span data-stu-id="f0046-140">The notification will be subsequently fanned-out to all specified endpoints with a valid subscription.</span></span> 

## <a name="example"></a><span data-ttu-id="f0046-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0046-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0046-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0046-142">Request</span></span>
<span data-ttu-id="f0046-143">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0046-143">The following is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/me/notifications/
Content-type: application/json

{
    "targetHostName": "graphnotifications.sample.windows.com",
    "appNotificationId": "testDirectToastNotification",
    "expirationDateTime": "2019-10-30T23:59:00.000Z",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    },
    "targetPolicy": {
        "platformTypes": [
    "windows",
    "ios",
    "android"
        ]
    },
    "priority": "High",
    "groupName": "TestGroup",
    "displayTimeToLive": "60"
}
```

### <a name="response"></a><span data-ttu-id="f0046-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0046-144">Response</span></span>
<span data-ttu-id="f0046-145">Veja a seguir um exemplo da resposta correspondente.</span><span class="sxs-lookup"><span data-stu-id="f0046-145">The following is an example of the corresponding response.</span></span>

```http
HTTP/1.1 201
client-request-id: 71e62feb-8d72-4912-8b2c-4cee9d89e781
content-length: 356
content-type: application/json
location: https://graph.microsoft.com/beta/me/activities/119081f2-f19d-4fa8-817c-7e01092c0f7d
request-id: 71e62feb-8d72-4912-8b2c-4cee9d89e781

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('graphnotify%40contoso.com')/notifications/$entity",
    "displayTimeToLive": 59,
    "expirationDateTime": "2019-10-28T22:05:36.25Z",
    "groupName": "TestGroup",
    "id": "119081f2-f19d-4fa8-817c-7e01092c0f7d",
    "priority": "High",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    }
}
```
