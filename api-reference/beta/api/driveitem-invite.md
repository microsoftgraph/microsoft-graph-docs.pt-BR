---
author: JeremyKelley
description: Envia um convite de compartilhamento para um DriveItem.
ms.date: 09/10/2017
title: Enviar um convite para acessar um item
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 0344a4b6b663aa5a2a0cc03a470907bb48f63f9f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416727"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="049fa-103">Enviar um convite de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="049fa-103">Send a sharing invitation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="049fa-p101">Envia um convite de compartilhamento para um **DriveItem**. Um convite de compartilhamento fornece permissões para os destinatários e, opcionalmente, envia um email aos destinatários para notificá-los de que o item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="049fa-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="049fa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="049fa-106">Permissions</span></span>

<span data-ttu-id="049fa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="049fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="049fa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="049fa-109">Permission type</span></span>      | <span data-ttu-id="049fa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="049fa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="049fa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="049fa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="049fa-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="049fa-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="049fa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="049fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="049fa-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="049fa-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="049fa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="049fa-115">Application</span></span> | <span data-ttu-id="049fa-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="049fa-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="049fa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="049fa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="049fa-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="049fa-118">Request body</span></span>

<span data-ttu-id="049fa-119">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="049fa-119">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="049fa-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="049fa-120">Parameter</span></span>        | <span data-ttu-id="049fa-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="049fa-121">Type</span></span>                                            | <span data-ttu-id="049fa-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="049fa-122">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="049fa-123">destinatários</span><span class="sxs-lookup"><span data-stu-id="049fa-123">recipients</span></span>       | <span data-ttu-id="049fa-124">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="049fa-124">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="049fa-125">Uma coleção dos destinatários que receberão o acesso e o convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="049fa-125">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="049fa-126">mensagem</span><span class="sxs-lookup"><span data-stu-id="049fa-126">message</span></span>          | <span data-ttu-id="049fa-127">String</span><span class="sxs-lookup"><span data-stu-id="049fa-127">String</span></span>                                          | <span data-ttu-id="049fa-p103">Uma mensagem de texto sem formatação que está incluída no convite de compartilhamento. Comprimento máximo de 2000 caracteres.</span><span class="sxs-lookup"><span data-stu-id="049fa-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="049fa-130">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="049fa-130">requireSignIn</span></span>    | <span data-ttu-id="049fa-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="049fa-131">Boolean</span></span>                                         | <span data-ttu-id="049fa-132">Especifica onde o destinatário do convite precisa entrar para exibir o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="049fa-132">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="049fa-133">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="049fa-133">sendInvitation</span></span>   | <span data-ttu-id="049fa-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="049fa-134">Boolean</span></span>                                         | <span data-ttu-id="049fa-135">Especifica se um email ou uma postagem é gerado (false) ou se a permissão é recém-criada (true).</span><span class="sxs-lookup"><span data-stu-id="049fa-135">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="049fa-136">funções</span><span class="sxs-lookup"><span data-stu-id="049fa-136">roles</span></span>            | <span data-ttu-id="049fa-137">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="049fa-137">Collection(String)</span></span>                              | <span data-ttu-id="049fa-138">Especifique as funções que são concedidas aos destinatários do convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="049fa-138">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |
| <span data-ttu-id="049fa-139">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="049fa-139">expirationDateTime</span></span> | <span data-ttu-id="049fa-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="049fa-140">DateTimeOffset</span></span>                       | <span data-ttu-id="049fa-141">Especifique o DateTime após o qual a permissão expira.</span><span class="sxs-lookup"><span data-stu-id="049fa-141">Specify the DateTime after which the permission expires.</span></span> <span data-ttu-id="049fa-142">Disponível em contas pessoais do OneDrive para o OneDrive for Business, SharePoint e Premium.</span><span class="sxs-lookup"><span data-stu-id="049fa-142">Available on OneDrive for Business, SharePoint, and premium personal OneDrive accounts.</span></span>
| <span data-ttu-id="049fa-143">password</span><span class="sxs-lookup"><span data-stu-id="049fa-143">password</span></span>           | <span data-ttu-id="049fa-144">String</span><span class="sxs-lookup"><span data-stu-id="049fa-144">String</span></span>                         | <span data-ttu-id="049fa-145">A senha definida no convite pelo criador.</span><span class="sxs-lookup"><span data-stu-id="049fa-145">The password set on the invite by the creator.</span></span> <span data-ttu-id="049fa-146">Opcional e o OneDrive somente pessoal</span><span class="sxs-lookup"><span data-stu-id="049fa-146">Optional and OneDrive Personal only</span></span>

## <a name="example"></a><span data-ttu-id="049fa-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="049fa-147">Example</span></span>

<span data-ttu-id="049fa-148">Este exemplo envia um convite de compartilhamento para um usuário com o endereço de email "ryan@contoso.org" com uma mensagem sobre um arquivo no qual ele está colaborando.</span><span class="sxs-lookup"><span data-stu-id="049fa-148">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="049fa-149">O convite concede acesso de leitura e gravação ao arquivo para Ryan.</span><span class="sxs-lookup"><span data-stu-id="049fa-149">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="049fa-150">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="049fa-150">HTTP request</span></span>

<span data-ttu-id="049fa-151">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto de coleção [permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="049fa-151">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="049fa-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="049fa-152">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="049fa-153">C#</span><span class="sxs-lookup"><span data-stu-id="049fa-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="049fa-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="049fa-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="049fa-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="049fa-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="049fa-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="049fa-156">Response</span></span>

<span data-ttu-id="049fa-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="049fa-157">Here is an example of the response.</span></span>

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
### <a name="partial-success-response"></a><span data-ttu-id="049fa-158">Resposta parcial com êxito</span><span class="sxs-lookup"><span data-stu-id="049fa-158">Partial success response</span></span>

<span data-ttu-id="049fa-159">Ao convidar vários destinatários, é possível que a notificação tenha êxito em alguns e falha para outras pessoas.</span><span class="sxs-lookup"><span data-stu-id="049fa-159">When inviting multiple recipients, it's possible for the notification to succeed for some and fail for others.</span></span>
<span data-ttu-id="049fa-160">Nesse caso, o serviço retorna uma resposta de êxito parcial com um código de status HTTP 207.</span><span class="sxs-lookup"><span data-stu-id="049fa-160">In this case, the service returns a partial success response with an HTTP status code of 207.</span></span>
<span data-ttu-id="049fa-161">Quando o sucesso parcial for retornado, a resposta para cada destinatário com falha conterá um `error` objeto com informações sobre o que deu errado e como corrigi-lo.</span><span class="sxs-lookup"><span data-stu-id="049fa-161">When partial success is returned, the response for each failed recipient will contain an `error` object with information about what went wrong and how to fix it.</span></span>

<span data-ttu-id="049fa-162">Veja um exemplo da resposta parcial.</span><span class="sxs-lookup"><span data-stu-id="049fa-162">Here is an example of the partial response.</span></span>  

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
### <a name="sendnotification-errors"></a><span data-ttu-id="049fa-163">Erros do SendNotification</span><span class="sxs-lookup"><span data-stu-id="049fa-163">SendNotification errors</span></span>
<span data-ttu-id="049fa-164">A seguir estão alguns erros adicionais que seu aplicativo pode encontrar nos objetos aninhados `innererror` ao enviar uma notificação falha.</span><span class="sxs-lookup"><span data-stu-id="049fa-164">The following are some additional errors that your app might encounter within the nested `innererror` objects when sending notification fails.</span></span> <span data-ttu-id="049fa-165">Os aplicativos não são necessários para lidar com eles.</span><span class="sxs-lookup"><span data-stu-id="049fa-165">Apps are not required to handle these.</span></span>

| <span data-ttu-id="049fa-166">Código</span><span class="sxs-lookup"><span data-stu-id="049fa-166">Code</span></span>                           | <span data-ttu-id="049fa-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="049fa-167">Description</span></span>
|:-------------------------------|:--------------------------------------------------------------------------------------
| <span data-ttu-id="049fa-168">accountVerificationRequired</span><span class="sxs-lookup"><span data-stu-id="049fa-168">accountVerificationRequired</span></span>    | <span data-ttu-id="049fa-169">A verificação da conta é necessária para desbloquear o envio de notificações.</span><span class="sxs-lookup"><span data-stu-id="049fa-169">Account verification is required to unblock sending notifications.</span></span>
| <span data-ttu-id="049fa-170">hipCheckRequired</span><span class="sxs-lookup"><span data-stu-id="049fa-170">hipCheckRequired</span></span>               | <span data-ttu-id="049fa-171">É necessário resolver a verificação HIP (Host Intrusion Prevention) para desbloquear o envio de notificações.</span><span class="sxs-lookup"><span data-stu-id="049fa-171">Need to solve HIP (Host Intrusion Prevention) check to unblock sending notifications.</span></span>
| <span data-ttu-id="049fa-172">exchangeInvalidUser</span><span class="sxs-lookup"><span data-stu-id="049fa-172">exchangeInvalidUser</span></span>            | <span data-ttu-id="049fa-173">A caixa de correio do usuário atual não foi encontrada.</span><span class="sxs-lookup"><span data-stu-id="049fa-173">Current user's mailbox was not found.</span></span>
| <span data-ttu-id="049fa-174">exchangeOutOfMailboxQuota</span><span class="sxs-lookup"><span data-stu-id="049fa-174">exchangeOutOfMailboxQuota</span></span>      | <span data-ttu-id="049fa-175">Fora da cota.</span><span class="sxs-lookup"><span data-stu-id="049fa-175">Out of quota.</span></span>
| <span data-ttu-id="049fa-176">exchangeMaxRecipients</span><span class="sxs-lookup"><span data-stu-id="049fa-176">exchangeMaxRecipients</span></span>          | <span data-ttu-id="049fa-177">Foi excedido o número máximo de destinatários que podem receber notificações ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="049fa-177">Exceeded maximum number of recipients that can be sent notifications at the same time.</span></span>

><span data-ttu-id="049fa-178">**Observação:** O serviço pode adicionar novos códigos de erro ou parar de retornar os antigos a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="049fa-178">**Note:** The service can add new error codes or stop returning old ones at any time.</span></span>

## <a name="remarks"></a><span data-ttu-id="049fa-179">Comentários</span><span class="sxs-lookup"><span data-stu-id="049fa-179">Remarks</span></span>

* <span data-ttu-id="049fa-180">[Drives](../resources/drive.md) com **driveType** de `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="049fa-180">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="049fa-181">Para obter uma lista das funções disponíveis, consulte [Funções de enumeração](../resources/permission.md#roles-enumeration-values).</span><span class="sxs-lookup"><span data-stu-id="049fa-181">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="049fa-182">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="049fa-182">Error responses</span></span>

<span data-ttu-id="049fa-183">Saiba mais sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="049fa-183">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


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
