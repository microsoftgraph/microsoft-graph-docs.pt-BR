---
title: Criar e enviar uma notificação
description: Criar e enviar uma notificação direcionada a um usuário por meio do Microsoft Graph.
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 8eb35ea0ade2e7d471674d8d064ba0ac38b361cc
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996260"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="6bbf7-103">Criar e enviar uma notificação</span><span class="sxs-lookup"><span data-stu-id="6bbf7-103">Create and send a notification</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bbf7-104">Criar e enviar uma notificação direcionada a um usuário por meio do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6bbf7-104">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="6bbf7-105">A notificação é armazenada no repositório de feeds de notificação do Microsoft Graph e é enviada a todos os clientes de aplicativos em todos os pontos de extremidade do dispositivo nos quais o usuário está conectado.</span><span class="sxs-lookup"><span data-stu-id="6bbf7-105">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  

## <a name="permissions"></a><span data-ttu-id="6bbf7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6bbf7-106">Permissions</span></span>
<span data-ttu-id="6bbf7-107">O serviço de aplicativo não requer nenhuma permissão adicional para postar notificações para o usuário de destino.</span><span class="sxs-lookup"><span data-stu-id="6bbf7-107">Your application service does not require any additional permissions to post notifications to your targeted user.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="6bbf7-108">Se você optar por publicar notificações em nome de um usuário via permissões delegadas, uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="6bbf7-108">If you choose to post notifications on behalf of a user via delegated permissions instead, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="6bbf7-109">Não recomendamos esta opção para postar notificações, mas se você quiser saber mais, incluindo como escolher permissões, consulte [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bbf7-109">We don't recommend this option for posting notifications but if you'd like to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bbf7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bbf7-110">Permission type</span></span>      | <span data-ttu-id="6bbf7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6bbf7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6bbf7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bbf7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6bbf7-113">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="6bbf7-113">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="6bbf7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bbf7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bbf7-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="6bbf7-115">Notifications.ReadWrite.CreatedByApp</span></span>    |
| <span data-ttu-id="6bbf7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bbf7-116">Application</span></span>                           | <span data-ttu-id="6bbf7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bbf7-117">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="6bbf7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bbf7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="6bbf7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bbf7-119">Request headers</span></span>
|<span data-ttu-id="6bbf7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6bbf7-120">Name</span></span> | <span data-ttu-id="6bbf7-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bbf7-121">Type</span></span> | <span data-ttu-id="6bbf7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bbf7-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="6bbf7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bbf7-123">Authorization</span></span> | <span data-ttu-id="6bbf7-124">string</span><span class="sxs-lookup"><span data-stu-id="6bbf7-124">string</span></span> |<span data-ttu-id="6bbf7-125">O cabeçalho de autorização é usado para passar as credenciais da parte de chamada.</span><span class="sxs-lookup"><span data-stu-id="6bbf7-125">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="6bbf7-126">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="6bbf7-126">Bearer {token}.</span></span> <span data-ttu-id="6bbf7-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bbf7-127">Required.</span></span> |
|<span data-ttu-id="6bbf7-128">X-UNS-ID</span><span class="sxs-lookup"><span data-stu-id="6bbf7-128">X-UNS-ID</span></span> | <span data-ttu-id="6bbf7-129">string</span><span class="sxs-lookup"><span data-stu-id="6bbf7-129">string</span></span> |<span data-ttu-id="6bbf7-130">O UserNotificationSubscriptionId retornado pelo serviço de notificação do Microsoft Graph após a criação de uma assinatura no lado do cliente e é usado para direcionar o usuário específico.</span><span class="sxs-lookup"><span data-stu-id="6bbf7-130">The UserNotificationSubscriptionId that is returned by the Microsoft Graph notification service after creating a subscription on the client-side, and is used to target the specific user.</span></span> <span data-ttu-id="6bbf7-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bbf7-131">Required.</span></span> |
|<span data-ttu-id="6bbf7-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="6bbf7-132">Content-type</span></span>| <span data-ttu-id="6bbf7-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bbf7-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bbf7-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bbf7-135">Request body</span></span>
<span data-ttu-id="6bbf7-136">No corpo da solicitação, forneça uma representação JSON de um objeto [Notification](../resources/projectrome-notification.md) .</span><span class="sxs-lookup"><span data-stu-id="6bbf7-136">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6bbf7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bbf7-137">Response</span></span>
<span data-ttu-id="6bbf7-138">Se tiver êxito, este método retornará `201 Created` um código de resposta que indica que a notificação foi criada e armazenada com êxito.</span><span class="sxs-lookup"><span data-stu-id="6bbf7-138">If successful, this method returns a `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> <span data-ttu-id="6bbf7-139">A notificação será subseqüentemente fanned a todos os pontos de extremidade especificados com uma assinatura válida.</span><span class="sxs-lookup"><span data-stu-id="6bbf7-139">The notification will be subsequently fanned-out to all specified endpoints with a valid subscription.</span></span> 

## <a name="example"></a><span data-ttu-id="6bbf7-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6bbf7-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="6bbf7-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bbf7-141">Request</span></span>
<span data-ttu-id="6bbf7-142">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bbf7-142">The following is an example of a request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6bbf7-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="6bbf7-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_notification_from_user"
}-->

```http
POST https://graph.microsoft.com/beta/me/notifications
Content-type: application/json

{
  "notification": {
    "targetHostName": "targetHostName-value",
    "appNotificationId": "appNotificationID-value",
    "expirationDateTime": "datetime-value",
    "targetPolicy": {
      "platformTypes": [
        "platformTypes-value"
        ]
      }, 
    "payload": {
      "rawContent": "rawContent-value",
      "visualContent": {
        "title": "title-value",
        "body": "body-value"
      }
    },
    "displayTimeToLive": 99,
    "priority": "priority-value",
    "groupName": "groupName-value"
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6bbf7-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6bbf7-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-notification-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6bbf7-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bbf7-145">Response</span></span>
<span data-ttu-id="6bbf7-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6bbf7-146">The following is an example of the response.</span></span>

> <span data-ttu-id="6bbf7-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6bbf7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notification"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "notification": {
    "targetHostName": "targetHostName-value",
    "expirationDateTime": "datetime-value",
    "payload": {
      "rawContent": "rawContent-value",
      "visualContent": {
        "title": "title-value",
        "body": "body-value"
      }
    },
    "displayTimeToLive": 99,
    "priority": "priority-value",
    "groupName": "groupName-value"
  }
}
```
