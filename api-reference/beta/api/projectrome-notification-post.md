---
title: Criar e enviar uma notificação
description: 'Criar e enviar uma notificação de direcionamento de um usuário por meio do Microsoft Graph. A notificação é armazenada na notificação Microsoft Graph feed repositório e é enviada a todos os clientes de aplicativo em todos os pontos de extremidade do dispositivo que o usuário está conectado ao.  '
ms.openlocfilehash: 7855d8b369a2efc6dada33c66c12ae76384a2760
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038498"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="a8a2e-104">Criar e enviar uma notificação</span><span class="sxs-lookup"><span data-stu-id="a8a2e-104">Create and send a notification</span></span>
> <span data-ttu-id="a8a2e-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8a2e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8a2e-107">Criar e enviar uma notificação de direcionamento de um usuário por meio do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-107">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="a8a2e-108">A notificação é armazenada na notificação Microsoft Graph feed repositório e é enviada a todos os clientes de aplicativo em todos os pontos de extremidade do dispositivo que o usuário está conectado ao.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-108">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  
## <a name="permissions"></a><span data-ttu-id="a8a2e-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="a8a2e-109">Permissions</span></span>
<span data-ttu-id="a8a2e-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8a2e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8a2e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8a2e-112">Permission type</span></span>      | <span data-ttu-id="a8a2e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8a2e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8a2e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8a2e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a8a2e-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a8a2e-115">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="a8a2e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8a2e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8a2e-117">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a8a2e-117">Notifications.ReadWrite.CreatedByApp</span></span>    |

## <a name="http-request"></a><span data-ttu-id="a8a2e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8a2e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="a8a2e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8a2e-119">Request headers</span></span>
|<span data-ttu-id="a8a2e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a8a2e-120">Name</span></span> | <span data-ttu-id="a8a2e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8a2e-121">Type</span></span> | <span data-ttu-id="a8a2e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8a2e-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="a8a2e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8a2e-123">Authorization</span></span> | <span data-ttu-id="a8a2e-124">string</span><span class="sxs-lookup"><span data-stu-id="a8a2e-124">string</span></span> |<span data-ttu-id="a8a2e-125">O cabeçalho de autorização é usado para passar as credenciais do chamador.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-125">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="a8a2e-126">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-126">Bearer {token}.</span></span> <span data-ttu-id="a8a2e-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-127">Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="a8a2e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8a2e-128">Request body</span></span>
<span data-ttu-id="a8a2e-129">No corpo da solicitação, fornece uma representação JSON de um objeto de [notificação](../resources/projectrome-notification.md) .</span><span class="sxs-lookup"><span data-stu-id="a8a2e-129">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a8a2e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8a2e-130">Response</span></span>
<span data-ttu-id="a8a2e-131">Se tiver êxito, este método retornará o `201 Created` código de resposta que indica que a notificação foi criada com êxito e armazenada.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-131">If successful, this method returns the `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> 
## <a name="example"></a><span data-ttu-id="a8a2e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8a2e-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a8a2e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8a2e-133">Request</span></span>
<span data-ttu-id="a8a2e-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-134">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="a8a2e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8a2e-135">Response</span></span>
<span data-ttu-id="a8a2e-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-136">The following is an example of the response.</span></span>

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


