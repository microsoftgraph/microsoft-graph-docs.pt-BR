---
author: JeremyKelley
description: Envia um convite de compartilhamento para um DriveItem.
ms.date: 09/10/2017
title: Enviar um convite para acessar um item
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 594df009c38ff1d7384207e7486392f24d7a8dbd
ms.sourcegitcommit: 6db0b7a473594653dda332ce7da45ea2ad90772b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/04/2020
ms.locfileid: "43146398"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="a830a-103">Enviar um convite de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="a830a-103">Send a sharing invitation</span></span>

<span data-ttu-id="a830a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a830a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a830a-p101">Envia um convite de compartilhamento para um **DriveItem**. Um convite de compartilhamento fornece permissões para os destinatários e, opcionalmente, envia um email aos destinatários para notificá-los de que o item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="a830a-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="a830a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a830a-107">Permissions</span></span>

<span data-ttu-id="a830a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a830a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a830a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a830a-110">Permission type</span></span>      | <span data-ttu-id="a830a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a830a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a830a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a830a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a830a-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a830a-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a830a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a830a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a830a-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a830a-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a830a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a830a-116">Application</span></span> | <span data-ttu-id="a830a-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a830a-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a830a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a830a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="a830a-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a830a-119">Request body</span></span>

<span data-ttu-id="a830a-120">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a830a-120">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite" } -->

```json
{
  "requireSignIn": false,
  "sendInvitation": false,
  "roles": [ "read | write"],
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" },
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "message": "string"
}
```

| <span data-ttu-id="a830a-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a830a-121">Parameter</span></span>        | <span data-ttu-id="a830a-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a830a-122">Type</span></span>                                            | <span data-ttu-id="a830a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a830a-123">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a830a-124">destinatários</span><span class="sxs-lookup"><span data-stu-id="a830a-124">recipients</span></span>       | <span data-ttu-id="a830a-125">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="a830a-125">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="a830a-126">Uma coleção dos destinatários que receberão o acesso e o convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="a830a-126">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="a830a-127">mensagem</span><span class="sxs-lookup"><span data-stu-id="a830a-127">message</span></span>          | <span data-ttu-id="a830a-128">String</span><span class="sxs-lookup"><span data-stu-id="a830a-128">String</span></span>                                          | <span data-ttu-id="a830a-p103">Uma mensagem de texto sem formatação que está incluída no convite de compartilhamento. Comprimento máximo de 2000 caracteres.</span><span class="sxs-lookup"><span data-stu-id="a830a-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="a830a-131">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="a830a-131">requireSignIn</span></span>    | <span data-ttu-id="a830a-132">Booleano</span><span class="sxs-lookup"><span data-stu-id="a830a-132">Boolean</span></span>                                         | <span data-ttu-id="a830a-133">Especifica onde o destinatário do convite precisa entrar para exibir o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="a830a-133">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="a830a-134">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="a830a-134">sendInvitation</span></span>   | <span data-ttu-id="a830a-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="a830a-135">Boolean</span></span>                                         | <span data-ttu-id="a830a-136">Especifica se um email ou uma postagem é gerado (false) ou se a permissão é recém-criada (true).</span><span class="sxs-lookup"><span data-stu-id="a830a-136">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="a830a-137">funções</span><span class="sxs-lookup"><span data-stu-id="a830a-137">roles</span></span>            | <span data-ttu-id="a830a-138">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="a830a-138">Collection(String)</span></span>                              | <span data-ttu-id="a830a-139">Especifique as funções que são concedidas aos destinatários do convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="a830a-139">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |
| <span data-ttu-id="a830a-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a830a-140">expirationDateTime</span></span> | <span data-ttu-id="a830a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a830a-141">DateTimeOffset</span></span>                       | <span data-ttu-id="a830a-142">Especifique o DateTime após o qual a permissão expira.</span><span class="sxs-lookup"><span data-stu-id="a830a-142">Specify the DateTime after which the permission expires.</span></span> <span data-ttu-id="a830a-143">Disponível em contas pessoais do OneDrive para o OneDrive for Business, SharePoint e Premium.</span><span class="sxs-lookup"><span data-stu-id="a830a-143">Available on OneDrive for Business, SharePoint, and premium personal OneDrive accounts.</span></span>
| <span data-ttu-id="a830a-144">password</span><span class="sxs-lookup"><span data-stu-id="a830a-144">password</span></span>           | <span data-ttu-id="a830a-145">String</span><span class="sxs-lookup"><span data-stu-id="a830a-145">String</span></span>                         | <span data-ttu-id="a830a-146">A senha definida no convite pelo criador.</span><span class="sxs-lookup"><span data-stu-id="a830a-146">The password set on the invite by the creator.</span></span> <span data-ttu-id="a830a-147">Opcional e o OneDrive somente pessoal</span><span class="sxs-lookup"><span data-stu-id="a830a-147">Optional and OneDrive Personal only</span></span>

## <a name="example"></a><span data-ttu-id="a830a-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a830a-148">Example</span></span>

<span data-ttu-id="a830a-149">Este exemplo envia um convite de compartilhamento para um usuário com o endereço de email "ryan@contoso.org" com uma mensagem sobre um arquivo no qual ele está colaborando.</span><span class="sxs-lookup"><span data-stu-id="a830a-149">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="a830a-150">O convite concede acesso de leitura e gravação ao arquivo para Ryan.</span><span class="sxs-lookup"><span data-stu-id="a830a-150">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="a830a-151">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a830a-151">HTTP request</span></span>

<span data-ttu-id="a830a-152">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto de coleção [permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a830a-152">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="http"></a>[<span data-ttu-id="a830a-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="a830a-153">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "send-sharing-invite", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ],
  "password": "password123",
  "expirationDateTime": "2018-07-15T14:00:00.000Z"
}
```
# <a name="c"></a>[<span data-ttu-id="a830a-154">C#</span><span class="sxs-lookup"><span data-stu-id="a830a-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a830a-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a830a-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a830a-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a830a-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a830a-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="a830a-157">Response</span></span>

<span data-ttu-id="a830a-158">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a830a-158">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "hasPassword": true,
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```
### <a name="partial-success-response"></a><span data-ttu-id="a830a-159">Resposta parcial com êxito</span><span class="sxs-lookup"><span data-stu-id="a830a-159">Partial success response</span></span>

<span data-ttu-id="a830a-160">Ao convidar vários destinatários, é possível que a notificação tenha êxito em alguns e falha para outras pessoas.</span><span class="sxs-lookup"><span data-stu-id="a830a-160">When inviting multiple recipients, it's possible for the notification to succeed for some and fail for others.</span></span>
<span data-ttu-id="a830a-161">Nesse caso, o serviço retorna uma resposta de êxito parcial com um código de status HTTP 207.</span><span class="sxs-lookup"><span data-stu-id="a830a-161">In this case, the service returns a partial success response with an HTTP status code of 207.</span></span>
<span data-ttu-id="a830a-162">Quando o sucesso parcial for retornado, a resposta para cada destinatário com falha conterá um `error` objeto com informações sobre o que deu errado e como corrigi-lo.</span><span class="sxs-lookup"><span data-stu-id="a830a-162">When partial success is returned, the response for each failed recipient will contain an `error` object with information about what went wrong and how to fix it.</span></span>

<span data-ttu-id="a830a-163">Veja um exemplo da resposta parcial.</span><span class="sxs-lookup"><span data-stu-id="a830a-163">Here is an example of the partial response.</span></span>  

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 207 Multi-Status
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "John Adams",
          "id": "5D8CA5D0-FFF8-4A97-B0A6-8F5AEA339681"
        }
      },
      "id": "1EFG7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "adams@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "error": {
        "code":"notAllowed",
        "message":"Account verification needed to unblock sending emails.",
        "localizedMessage": "Kontobestätigung erforderlich, um das Senden von E-Mails zu entsperren.",
        "fixItUrl":"http://g.live.com/8SESkydrive/VerifyAccount",
        "innererror":{  
          "code":"accountVerificationRequired" 
        }
      }
    },
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```
### <a name="sendnotification-errors"></a><span data-ttu-id="a830a-164">Erros do SendNotification</span><span class="sxs-lookup"><span data-stu-id="a830a-164">SendNotification errors</span></span>
<span data-ttu-id="a830a-165">A seguir estão alguns erros adicionais que seu aplicativo pode encontrar nos objetos aninhados `innererror` ao enviar uma notificação falha.</span><span class="sxs-lookup"><span data-stu-id="a830a-165">The following are some additional errors that your app might encounter within the nested `innererror` objects when sending notification fails.</span></span> <span data-ttu-id="a830a-166">Os aplicativos não são necessários para lidar com eles.</span><span class="sxs-lookup"><span data-stu-id="a830a-166">Apps are not required to handle these.</span></span>

| <span data-ttu-id="a830a-167">Código</span><span class="sxs-lookup"><span data-stu-id="a830a-167">Code</span></span>                           | <span data-ttu-id="a830a-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="a830a-168">Description</span></span>
|:-------------------------------|:--------------------------------------------------------------------------------------
| <span data-ttu-id="a830a-169">accountVerificationRequired</span><span class="sxs-lookup"><span data-stu-id="a830a-169">accountVerificationRequired</span></span>    | <span data-ttu-id="a830a-170">A verificação da conta é necessária para desbloquear o envio de notificações.</span><span class="sxs-lookup"><span data-stu-id="a830a-170">Account verification is required to unblock sending notifications.</span></span>
| <span data-ttu-id="a830a-171">hipCheckRequired</span><span class="sxs-lookup"><span data-stu-id="a830a-171">hipCheckRequired</span></span>               | <span data-ttu-id="a830a-172">É necessário resolver a verificação HIP (Host Intrusion Prevention) para desbloquear o envio de notificações.</span><span class="sxs-lookup"><span data-stu-id="a830a-172">Need to solve HIP (Host Intrusion Prevention) check to unblock sending notifications.</span></span>
| <span data-ttu-id="a830a-173">exchangeInvalidUser</span><span class="sxs-lookup"><span data-stu-id="a830a-173">exchangeInvalidUser</span></span>            | <span data-ttu-id="a830a-174">A caixa de correio do usuário atual não foi encontrada.</span><span class="sxs-lookup"><span data-stu-id="a830a-174">Current user's mailbox was not found.</span></span>
| <span data-ttu-id="a830a-175">exchangeOutOfMailboxQuota</span><span class="sxs-lookup"><span data-stu-id="a830a-175">exchangeOutOfMailboxQuota</span></span>      | <span data-ttu-id="a830a-176">Fora da cota.</span><span class="sxs-lookup"><span data-stu-id="a830a-176">Out of quota.</span></span>
| <span data-ttu-id="a830a-177">exchangeMaxRecipients</span><span class="sxs-lookup"><span data-stu-id="a830a-177">exchangeMaxRecipients</span></span>          | <span data-ttu-id="a830a-178">Foi excedido o número máximo de destinatários que podem receber notificações ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="a830a-178">Exceeded maximum number of recipients that can be sent notifications at the same time.</span></span>

><span data-ttu-id="a830a-179">**Observação:** O serviço pode adicionar novos códigos de erro ou parar de retornar os antigos a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="a830a-179">**Note:** The service can add new error codes or stop returning old ones at any time.</span></span>

## <a name="remarks"></a><span data-ttu-id="a830a-180">Comentários</span><span class="sxs-lookup"><span data-stu-id="a830a-180">Remarks</span></span>

* <span data-ttu-id="a830a-181">[Drives](../resources/drive.md) com **driveType** de `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="a830a-181">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="a830a-182">Para obter uma lista de funções disponíveis, consulte [funções valores de propriedade](../resources/permission.md#roles-property-values).</span><span class="sxs-lookup"><span data-stu-id="a830a-182">For a list of available roles, see [roles property values](../resources/permission.md#roles-property-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="a830a-183">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="a830a-183">Error responses</span></span>

<span data-ttu-id="a830a-184">Veja mais informações sobre como os erros são retornados no tópico [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="a830a-184">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
  ]
}
-->
