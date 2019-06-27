---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Enviar um convite para acessar um item
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: df1b179539847b8e75bbab47439c5713310922fc
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260127"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="ce208-102">Enviar um convite de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="ce208-102">Send a sharing invitation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce208-p101">Envia um convite de compartilhamento para um **DriveItem**. Um convite de compartilhamento fornece permissões para os destinatários e, opcionalmente, envia um email aos destinatários para notificá-los de que o item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="ce208-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce208-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce208-105">Permissions</span></span>

<span data-ttu-id="ce208-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce208-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce208-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce208-108">Permission type</span></span>      | <span data-ttu-id="ce208-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce208-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce208-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce208-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce208-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce208-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce208-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce208-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce208-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce208-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce208-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce208-114">Application</span></span> | <span data-ttu-id="ce208-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce208-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce208-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce208-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="ce208-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce208-117">Request body</span></span>

<span data-ttu-id="ce208-118">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce208-118">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="ce208-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ce208-119">Parameter</span></span>        | <span data-ttu-id="ce208-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce208-120">Type</span></span>                                            | <span data-ttu-id="ce208-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce208-121">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ce208-122">destinatários</span><span class="sxs-lookup"><span data-stu-id="ce208-122">recipients</span></span>       | <span data-ttu-id="ce208-123">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="ce208-123">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="ce208-124">Uma coleção dos destinatários que receberão o acesso e o convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="ce208-124">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="ce208-125">mensagem</span><span class="sxs-lookup"><span data-stu-id="ce208-125">message</span></span>          | <span data-ttu-id="ce208-126">String</span><span class="sxs-lookup"><span data-stu-id="ce208-126">String</span></span>                                          | <span data-ttu-id="ce208-p103">Uma mensagem de texto sem formatação que está incluída no convite de compartilhamento. Comprimento máximo de 2000 caracteres.</span><span class="sxs-lookup"><span data-stu-id="ce208-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="ce208-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="ce208-129">requireSignIn</span></span>    | <span data-ttu-id="ce208-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce208-130">Boolean</span></span>                                         | <span data-ttu-id="ce208-131">Especifica onde o destinatário do convite precisa entrar para exibir o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="ce208-131">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="ce208-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="ce208-132">sendInvitation</span></span>   | <span data-ttu-id="ce208-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce208-133">Boolean</span></span>                                         | <span data-ttu-id="ce208-134">Especifica se um email ou uma postagem é gerado (false) ou se a permissão é recém-criada (true).</span><span class="sxs-lookup"><span data-stu-id="ce208-134">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="ce208-135">funções</span><span class="sxs-lookup"><span data-stu-id="ce208-135">roles</span></span>            | <span data-ttu-id="ce208-136">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="ce208-136">Collection(String)</span></span>                              | <span data-ttu-id="ce208-137">Especifique as funções que são concedidas aos destinatários do convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="ce208-137">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |
| <span data-ttu-id="ce208-138">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ce208-138">expirationDateTime</span></span> | <span data-ttu-id="ce208-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce208-139">DateTimeOffset</span></span>                       | <span data-ttu-id="ce208-140">Especifique o DateTime após o qual a permissão expira.</span><span class="sxs-lookup"><span data-stu-id="ce208-140">Specify the DateTime after which the permission expires.</span></span> <span data-ttu-id="ce208-141">Disponível em contas pessoais do OneDrive para o OneDrive for Business, SharePoint e Premium.</span><span class="sxs-lookup"><span data-stu-id="ce208-141">Available on OneDrive for Business, SharePoint, and premium personal OneDrive accounts.</span></span>
| <span data-ttu-id="ce208-142">password</span><span class="sxs-lookup"><span data-stu-id="ce208-142">password</span></span>           | <span data-ttu-id="ce208-143">String</span><span class="sxs-lookup"><span data-stu-id="ce208-143">String</span></span>                         | <span data-ttu-id="ce208-144">A senha definida no convite pelo criador.</span><span class="sxs-lookup"><span data-stu-id="ce208-144">The password set on the invite by the creator.</span></span> <span data-ttu-id="ce208-145">Opcional e o OneDrive somente pessoal</span><span class="sxs-lookup"><span data-stu-id="ce208-145">Optional and OneDrive Personal only</span></span>

## <a name="example"></a><span data-ttu-id="ce208-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce208-146">Example</span></span>

<span data-ttu-id="ce208-147">Este exemplo envia um convite de compartilhamento para um usuário com o endereço de email "ryan@contoso.org" com uma mensagem sobre um arquivo no qual ele está colaborando.</span><span class="sxs-lookup"><span data-stu-id="ce208-147">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="ce208-148">O convite concede acesso de leitura e gravação ao arquivo para Ryan.</span><span class="sxs-lookup"><span data-stu-id="ce208-148">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="ce208-149">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce208-149">HTTP request</span></span>

<span data-ttu-id="ce208-150">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto de coleção [permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce208-150">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

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

### <a name="response"></a><span data-ttu-id="ce208-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce208-151">Response</span></span>

<span data-ttu-id="ce208-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce208-152">Here is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ce208-153">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="ce208-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ce208-154">C#</span><span class="sxs-lookup"><span data-stu-id="ce208-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/send-sharing-invite-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce208-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce208-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/send-sharing-invite-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ce208-156">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ce208-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/send-sharing-invite-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
### <a name="partial-success-response"></a><span data-ttu-id="ce208-157">Resposta parcial com êxito</span><span class="sxs-lookup"><span data-stu-id="ce208-157">Partial success response</span></span>

<span data-ttu-id="ce208-158">Ao convidar vários destinatários, é possível que a notificação tenha êxito em alguns e falha para outras pessoas.</span><span class="sxs-lookup"><span data-stu-id="ce208-158">When inviting multiple recipients, it's possible for the notification to succeed for some and fail for others.</span></span>
<span data-ttu-id="ce208-159">Nesse caso, o serviço retorna uma resposta de êxito parcial com um código de status HTTP 207.</span><span class="sxs-lookup"><span data-stu-id="ce208-159">In this case, the service returns a partial success response with an HTTP status code of 207.</span></span>
<span data-ttu-id="ce208-160">Quando o sucesso parcial for retornado, a resposta para cada destinatário com falha conterá um `error` objeto com informações sobre o que deu errado e como corrigi-lo.</span><span class="sxs-lookup"><span data-stu-id="ce208-160">When partial success is returned, the response for each failed recipient will contain an `error` object with information about what went wrong and how to fix it.</span></span>

<span data-ttu-id="ce208-161">Veja um exemplo da resposta parcial.</span><span class="sxs-lookup"><span data-stu-id="ce208-161">Here is an example of the partial response.</span></span>  

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
### <a name="sendnotification-errors"></a><span data-ttu-id="ce208-162">Erros do SendNotification</span><span class="sxs-lookup"><span data-stu-id="ce208-162">SendNotification errors</span></span>
<span data-ttu-id="ce208-163">A seguir estão alguns erros adicionais que seu aplicativo pode encontrar nos objetos aninhados `innererror` ao enviar uma notificação falha.</span><span class="sxs-lookup"><span data-stu-id="ce208-163">The following are some additional errors that your app might encounter within the nested `innererror` objects when sending notification fails.</span></span> <span data-ttu-id="ce208-164">Os aplicativos não são necessários para lidar com eles.</span><span class="sxs-lookup"><span data-stu-id="ce208-164">Apps are not required to handle these.</span></span>

| <span data-ttu-id="ce208-165">Código</span><span class="sxs-lookup"><span data-stu-id="ce208-165">Code</span></span>                           | <span data-ttu-id="ce208-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce208-166">Description</span></span>
|:-------------------------------|:--------------------------------------------------------------------------------------
| <span data-ttu-id="ce208-167">accountVerificationRequired</span><span class="sxs-lookup"><span data-stu-id="ce208-167">accountVerificationRequired</span></span>    | <span data-ttu-id="ce208-168">A verificação da conta é necessária para desbloquear o envio de notificações.</span><span class="sxs-lookup"><span data-stu-id="ce208-168">Account verification is required to unblock sending notifications.</span></span>
| <span data-ttu-id="ce208-169">hipCheckRequired</span><span class="sxs-lookup"><span data-stu-id="ce208-169">hipCheckRequired</span></span>               | <span data-ttu-id="ce208-170">É necessário resolver a verificação HIP (Host Intrusion Prevention) para desbloquear o envio de notificações.</span><span class="sxs-lookup"><span data-stu-id="ce208-170">Need to solve HIP (Host Intrusion Prevention) check to unblock sending notifications.</span></span>
| <span data-ttu-id="ce208-171">exchangeInvalidUser</span><span class="sxs-lookup"><span data-stu-id="ce208-171">exchangeInvalidUser</span></span>            | <span data-ttu-id="ce208-172">A caixa de correio do usuário atual não foi encontrada.</span><span class="sxs-lookup"><span data-stu-id="ce208-172">Current user's mailbox was not found.</span></span>
| <span data-ttu-id="ce208-173">exchangeOutOfMailboxQuota</span><span class="sxs-lookup"><span data-stu-id="ce208-173">exchangeOutOfMailboxQuota</span></span>      | <span data-ttu-id="ce208-174">Fora da cota.</span><span class="sxs-lookup"><span data-stu-id="ce208-174">Out of quota.</span></span>
| <span data-ttu-id="ce208-175">exchangeMaxRecipients</span><span class="sxs-lookup"><span data-stu-id="ce208-175">exchangeMaxRecipients</span></span>          | <span data-ttu-id="ce208-176">Foi excedido o número máximo de destinatários que podem receber notificações ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="ce208-176">Exceeded maximum number of recipients that can be sent notifications at the same time.</span></span>

><span data-ttu-id="ce208-177">**Observação:** O serviço pode adicionar novos códigos de erro ou parar de retornar os antigos a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="ce208-177">**Note:** The service can add new error codes or stop returning old ones at any time.</span></span>

## <a name="remarks"></a><span data-ttu-id="ce208-178">Comentários</span><span class="sxs-lookup"><span data-stu-id="ce208-178">Remarks</span></span>

* <span data-ttu-id="ce208-179">[Drives](../resources/drive.md) com **driveType** de `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="ce208-179">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="ce208-180">Para obter uma lista das funções disponíveis, consulte [Funções de enumeração](../resources/permission.md#roles-enumeration-values).</span><span class="sxs-lookup"><span data-stu-id="ce208-180">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="ce208-181">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="ce208-181">Error responses</span></span>

<span data-ttu-id="ce208-182">Saiba mais sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="ce208-182">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-invite.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitem-invite.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-invite.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
