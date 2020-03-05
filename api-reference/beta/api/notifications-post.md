---
title: Criar e enviar uma notificação
description: Criar e enviar uma notificação direcionada a um usuário por meio do Microsoft Graph.
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 1828f72bfcedb701597ce4b0d55e274a25fcf834
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456681"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="82da3-103">Criar e enviar uma notificação</span><span class="sxs-lookup"><span data-stu-id="82da3-103">Create and send a notification</span></span>

<span data-ttu-id="82da3-104">Namespace: Microsoft. Graph[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="82da3-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="82da3-105">Criar e enviar uma notificação direcionada a um usuário por meio do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="82da3-105">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="82da3-106">A notificação é armazenada no repositório de feeds de notificação do Microsoft Graph e é enviada a todos os clientes de aplicativos em todos os pontos de extremidade do dispositivo nos quais o usuário está conectado.</span><span class="sxs-lookup"><span data-stu-id="82da3-106">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  

## <a name="permissions"></a><span data-ttu-id="82da3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="82da3-107">Permissions</span></span>
<span data-ttu-id="82da3-108">O serviço de aplicativo não requer nenhuma permissão adicional para postar notificações para o usuário de destino.</span><span class="sxs-lookup"><span data-stu-id="82da3-108">Your application service does not require any additional permissions to post notifications to your targeted user.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="82da3-109">Se você optar por publicar notificações em nome de um usuário via permissões delegadas, uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="82da3-109">If you choose to post notifications on behalf of a user via delegated permissions instead, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="82da3-110">Não recomendamos esta opção para a criação de notificações.</span><span class="sxs-lookup"><span data-stu-id="82da3-110">We don't recommend this option for creating notifications.</span></span> <span data-ttu-id="82da3-111">Se quiser saber mais, incluindo como escolher permissões, consulte [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82da3-111">If you'd like to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82da3-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82da3-112">Permission type</span></span>      | <span data-ttu-id="82da3-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="82da3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82da3-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82da3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="82da3-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="82da3-115">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="82da3-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82da3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82da3-117">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="82da3-117">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="82da3-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82da3-118">Application</span></span> | <span data-ttu-id="82da3-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82da3-119">Not supported.</span></span>|



## <a name="http-request"></a><span data-ttu-id="82da3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82da3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="82da3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82da3-121">Request headers</span></span>
|<span data-ttu-id="82da3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="82da3-122">Name</span></span> | <span data-ttu-id="82da3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="82da3-123">Description</span></span>|
|:----|:-----------|
|<span data-ttu-id="82da3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="82da3-124">Authorization</span></span> | <span data-ttu-id="82da3-125">O cabeçalho de autorização é usado para passar as credenciais da parte de chamada.</span><span class="sxs-lookup"><span data-stu-id="82da3-125">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="82da3-126">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="82da3-126">Bearer {token}.</span></span> <span data-ttu-id="82da3-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82da3-127">Required.</span></span> |
|<span data-ttu-id="82da3-128">X-UNS-ID</span><span class="sxs-lookup"><span data-stu-id="82da3-128">X-UNS-ID</span></span> | <span data-ttu-id="82da3-129">O UserNotificationSubscriptionId retornado pelo serviço de notificação do Microsoft Graph após a criação de uma assinatura e é usado para direcionar o usuário específico.</span><span class="sxs-lookup"><span data-stu-id="82da3-129">The UserNotificationSubscriptionId that is returned by the Microsoft Graph notification service after creating a subscription and is used to target the specific user.</span></span> <span data-ttu-id="82da3-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82da3-130">Required.</span></span> |
|<span data-ttu-id="82da3-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="82da3-131">Content-type</span></span> | <span data-ttu-id="82da3-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82da3-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82da3-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82da3-134">Request body</span></span>
<span data-ttu-id="82da3-135">No corpo da solicitação, forneça uma representação JSON de um objeto [Notification](../resources/projectrome-notification.md) .</span><span class="sxs-lookup"><span data-stu-id="82da3-135">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="82da3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="82da3-136">Response</span></span>
<span data-ttu-id="82da3-137">Se tiver êxito, este método retornará `201 Created` um código de resposta que indica que a notificação foi criada e armazenada com êxito.</span><span class="sxs-lookup"><span data-stu-id="82da3-137">If successful, this method returns a `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> <span data-ttu-id="82da3-138">A notificação será subseqüentemente fanned a todos os pontos de extremidade especificados com uma assinatura válida.</span><span class="sxs-lookup"><span data-stu-id="82da3-138">The notification will be subsequently fanned-out to all specified endpoints with a valid subscription.</span></span> 

<span data-ttu-id="82da3-139">A tabela a seguir lista os possíveis códigos de erro e resposta que podem ser retornados.</span><span class="sxs-lookup"><span data-stu-id="82da3-139">The following table lists the possible error and response codes that can be returned.</span></span>

|<span data-ttu-id="82da3-140">Código de erro</span><span class="sxs-lookup"><span data-stu-id="82da3-140">Error code</span></span>             | <span data-ttu-id="82da3-141">Descrition</span><span class="sxs-lookup"><span data-stu-id="82da3-141">Descrition</span></span>                             |
|:-----------------------------------|:----------------------------------------------------------|
|<span data-ttu-id="82da3-142">HttpStatusCode. BadRequest</span><span class="sxs-lookup"><span data-stu-id="82da3-142">HttpStatusCode.BadRequest</span></span>           | <span data-ttu-id="82da3-143">O corpo é uma matriz (não há suporte para várias notificações).</span><span class="sxs-lookup"><span data-stu-id="82da3-143">Body is an array (multiple notifications is not supported).</span></span>|
|<span data-ttu-id="82da3-144">HttpStatusCode. BadRequest</span><span class="sxs-lookup"><span data-stu-id="82da3-144">HttpStatusCode.BadRequest</span></span>           | <span data-ttu-id="82da3-145">O corpo não corresponde ao contrato da API.</span><span class="sxs-lookup"><span data-stu-id="82da3-145">Body doesn't match the contract for the API.</span></span>               |
|<span data-ttu-id="82da3-146">HttpStatusCode. proibido</span><span class="sxs-lookup"><span data-stu-id="82da3-146">HttpStatusCode.Forbidden</span></span>            | <span data-ttu-id="82da3-147">O chamador está na lista de bloqueados.</span><span class="sxs-lookup"><span data-stu-id="82da3-147">Caller is on the blocked list.</span></span>                          |
|<span data-ttu-id="82da3-148">HttpStatusCode. MethodNotAllowed</span><span class="sxs-lookup"><span data-stu-id="82da3-148">HttpStatusCode.MethodNotAllowed</span></span>     | <span data-ttu-id="82da3-149">Não há suporte para o método HTTP usado.</span><span class="sxs-lookup"><span data-stu-id="82da3-149">The HTTP method used is not supported.</span></span>                     |
|<span data-ttu-id="82da3-150">HttpStatusCode. BadRequest</span><span class="sxs-lookup"><span data-stu-id="82da3-150">HttpStatusCode.BadRequest</span></span>           | <span data-ttu-id="82da3-151">Cabeçalhos sem suporte estão presentes na solicitação.</span><span class="sxs-lookup"><span data-stu-id="82da3-151">Unsupported headers are present in the request.</span></span> <span data-ttu-id="82da3-152">Não há suporte para dois cabeçalhos:</span><span class="sxs-lookup"><span data-stu-id="82da3-152">Two headers are not supported:</span></span><br/><br/><span data-ttu-id="82da3-153">If-Modified-Since</span><span class="sxs-lookup"><span data-stu-id="82da3-153">If-Modified-Since</span></span><br/><span data-ttu-id="82da3-154">If-Range</span><span class="sxs-lookup"><span data-stu-id="82da3-154">If-Range</span></span> |                    
|<span data-ttu-id="82da3-155">HttpStatusCode. UnsupportedMediaType</span><span class="sxs-lookup"><span data-stu-id="82da3-155">HttpStatusCode.UnsupportedMediaType</span></span> | <span data-ttu-id="82da3-156">O cabeçalho Content-Encoding está presente e tem valores de algoritmo de compactação diferentes de `Deflate` ou `Gzip`.</span><span class="sxs-lookup"><span data-stu-id="82da3-156">The header Content-Encoding is present and has compression algorithm values other than `Deflate` or `Gzip`.</span></span>  |
|<span data-ttu-id="82da3-157">HttpStatusCode. BadRequest</span><span class="sxs-lookup"><span data-stu-id="82da3-157">HttpStatusCode.BadRequest</span></span>           | <span data-ttu-id="82da3-158">Carga inválida.</span><span class="sxs-lookup"><span data-stu-id="82da3-158">Invalid payload.</span></span>                                           |
|<span data-ttu-id="82da3-159">HttpStatusCode. proibido</span><span class="sxs-lookup"><span data-stu-id="82da3-159">HttpStatusCode.Forbidden</span></span>            | <span data-ttu-id="82da3-160">O chamador não está autorizado a atuar em nome do usuário ou enviar notificação para o usuário.</span><span class="sxs-lookup"><span data-stu-id="82da3-160">Caller is not authorized to act on behalf of the user or send notification to the user.</span></span>                         |
|<span data-ttu-id="82da3-161">HttpStatusCode. não autorizado</span><span class="sxs-lookup"><span data-stu-id="82da3-161">HttpStatusCode.Unauthorized</span></span>         |  <span data-ttu-id="82da3-162">O corpo da solicitação contém tipos de dados de atividade inválidos.</span><span class="sxs-lookup"><span data-stu-id="82da3-162">Request body contains invalid activity data types.</span></span>        |
|<span data-ttu-id="82da3-163">HttpStatusCode. OK</span><span class="sxs-lookup"><span data-stu-id="82da3-163">HttpStatusCode.OK</span></span>                   |  <span data-ttu-id="82da3-164">Atividade criada com êxito.</span><span class="sxs-lookup"><span data-stu-id="82da3-164">Activity successfully created.</span></span>                            |
|<span data-ttu-id="82da3-165">HttpStatusCode. não aceito</span><span class="sxs-lookup"><span data-stu-id="82da3-165">HttpStatusCode.NotAcceptable</span></span>        |  <span data-ttu-id="82da3-166">A solicitação foi limitada ou o servidor está ocupado.</span><span class="sxs-lookup"><span data-stu-id="82da3-166">Request has been throttled or the server is busy.</span></span>    |


## <a name="example"></a><span data-ttu-id="82da3-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82da3-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="82da3-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82da3-168">Request</span></span>
<span data-ttu-id="82da3-169">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="82da3-169">The following is an example of a request.</span></span>

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

### <a name="response"></a><span data-ttu-id="82da3-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="82da3-170">Response</span></span>
<span data-ttu-id="82da3-171">Veja a seguir um exemplo da resposta correspondente.</span><span class="sxs-lookup"><span data-stu-id="82da3-171">The following is an example of the corresponding response.</span></span>

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

