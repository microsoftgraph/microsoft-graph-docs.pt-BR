---
title: Criar e enviar uma notificação
description: 'Criar e enviar uma notificação direcionada a um usuário por meio do Microsoft Graph. A notificação é armazenada no repositório de feeds de notificação do Microsoft Graph e é enviada a todos os clientes de aplicativos em todos os pontos de extremidade do dispositivo nos quais o usuário está conectado.  '
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ''
ms.openlocfilehash: a5ed743e93a5cafcb7ee919acbbcee5f2734a5de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992644"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="d0ede-104">Criar e enviar uma notificação</span><span class="sxs-lookup"><span data-stu-id="d0ede-104">Create and send a notification</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0ede-105">Criar e enviar uma notificação direcionada a um usuário por meio do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d0ede-105">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="d0ede-106">A notificação é armazenada no repositório de feeds de notificação do Microsoft Graph e é enviada a todos os clientes de aplicativos em todos os pontos de extremidade do dispositivo nos quais o usuário está conectado.</span><span class="sxs-lookup"><span data-stu-id="d0ede-106">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  
## <a name="permissions"></a><span data-ttu-id="d0ede-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0ede-107">Permissions</span></span>
<span data-ttu-id="d0ede-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0ede-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0ede-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0ede-110">Permission type</span></span>      | <span data-ttu-id="d0ede-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0ede-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0ede-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0ede-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d0ede-113">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d0ede-113">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="d0ede-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0ede-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0ede-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d0ede-115">Notifications.ReadWrite.CreatedByApp</span></span>    |

## <a name="http-request"></a><span data-ttu-id="d0ede-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0ede-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="d0ede-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0ede-117">Request headers</span></span>
|<span data-ttu-id="d0ede-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d0ede-118">Name</span></span> | <span data-ttu-id="d0ede-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0ede-119">Type</span></span> | <span data-ttu-id="d0ede-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0ede-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="d0ede-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0ede-121">Authorization</span></span> | <span data-ttu-id="d0ede-122">string</span><span class="sxs-lookup"><span data-stu-id="d0ede-122">string</span></span> |<span data-ttu-id="d0ede-123">O cabeçalho de autorização é usado para passar as credenciais da parte de chamada.</span><span class="sxs-lookup"><span data-stu-id="d0ede-123">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="d0ede-124">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="d0ede-124">Bearer {token}.</span></span> <span data-ttu-id="d0ede-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0ede-125">Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="d0ede-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0ede-126">Request body</span></span>
<span data-ttu-id="d0ede-127">No corpo da solicitação, forneça uma representação JSON de um objeto [Notification](../resources/projectrome-notification.md) .</span><span class="sxs-lookup"><span data-stu-id="d0ede-127">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d0ede-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0ede-128">Response</span></span>
<span data-ttu-id="d0ede-129">Se tiver êxito, este método retornará `201 Created` o código de resposta que indica que a notificação foi criada e armazenada com êxito.</span><span class="sxs-lookup"><span data-stu-id="d0ede-129">If successful, this method returns the `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> 
## <a name="example"></a><span data-ttu-id="d0ede-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0ede-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d0ede-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0ede-131">Request</span></span>
<span data-ttu-id="d0ede-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0ede-132">The following is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/me/notifications/
Content-type: application/json

{
    "targetHostName": "graphnotifications.sample.windows.com",
    "appNotificationId": "testDirectToastNotification",
    "expirationDateTime": "2018-08-29T23:51:33.000Z",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    },
    "targetPolicy": {
        "platformTypes": [
        "windows",
        "android"
        ]
    },
    "priority": "High",
    "groupName": "TestGroup",
    "displayTimeToLive": "23"
}
```

#### <a name="response"></a><span data-ttu-id="d0ede-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0ede-133">Response</span></span>
<span data-ttu-id="d0ede-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d0ede-134">The following is an example of the response.</span></span>

```http
HTTP/1.1 201
Content-Type: application/json
location: https://graph.microsoft.com/beta/me/notifications/518c4fb1-c565-4d67-95c4-bcc3eb8eda1b

{
    "@odata.context": "https://graph.microsoft.com/test872018/$metadata#users('graphNotificationsUser%40contoso.com')/notifications/$entity",
    "appNotificationId": "testDirectToastNotification",
    "displayTimeToLive": 23,
    "expirationDateTime": "2018-08-24T12:31:53.858Z",
    "groupName": "TestGroup",
    "id": "cd5c5e6a-99ce-470a-9982-c47635e73620",
    "priority": "1",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    }
}
```


