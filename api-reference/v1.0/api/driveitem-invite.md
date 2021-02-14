---
author: JeremyKelley
ms.date: 09/10/2017
title: Enviar um convite para acessar um item
localization_priority: Normal
ms.prod: sharepoint
description: Envia um convite de compartilhamento para um driveItem.
doc_type: apiPageType
ms.openlocfilehash: e514fbd3b8f79d3696f894a6b15ad55055137b70
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240287"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="ab0e8-103">Enviar um convite de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="ab0e8-103">Send a sharing invitation</span></span>

<span data-ttu-id="ab0e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab0e8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab0e8-105">Envia um convite de compartilhamento para **um driveItem**.</span><span class="sxs-lookup"><span data-stu-id="ab0e8-105">Sends a sharing invitation for a **driveItem**.</span></span>
<span data-ttu-id="ab0e8-106">Um convite de compartilhamento fornece permissões para os destinatários e, opcionalmente, envia um email com um [link de compartilhamento][].</span><span class="sxs-lookup"><span data-stu-id="ab0e8-106">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="ab0e8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab0e8-107">Permissions</span></span>

<span data-ttu-id="ab0e8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab0e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab0e8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab0e8-110">Permission type</span></span>      | <span data-ttu-id="ab0e8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab0e8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab0e8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab0e8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ab0e8-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab0e8-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab0e8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab0e8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab0e8-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab0e8-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab0e8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab0e8-116">Application</span></span> | <span data-ttu-id="ab0e8-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab0e8-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab0e8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab0e8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="ab0e8-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab0e8-119">Request body</span></span>

<span data-ttu-id="ab0e8-120">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab0e8-120">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

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

| <span data-ttu-id="ab0e8-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ab0e8-121">Parameter</span></span>        | <span data-ttu-id="ab0e8-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab0e8-122">Type</span></span>                           | <span data-ttu-id="ab0e8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab0e8-123">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="ab0e8-124">destinatários</span><span class="sxs-lookup"><span data-stu-id="ab0e8-124">recipients</span></span>       | <span data-ttu-id="ab0e8-125">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="ab0e8-125">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="ab0e8-126">Uma coleção dos destinatários que receberão o acesso e o convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="ab0e8-126">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="ab0e8-127">mensagem</span><span class="sxs-lookup"><span data-stu-id="ab0e8-127">message</span></span>          | <span data-ttu-id="ab0e8-128">String</span><span class="sxs-lookup"><span data-stu-id="ab0e8-128">String</span></span>                         | <span data-ttu-id="ab0e8-p103">Uma mensagem de texto sem formatação que está incluída no convite de compartilhamento. Comprimento máximo de 2000 caracteres.</span><span class="sxs-lookup"><span data-stu-id="ab0e8-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="ab0e8-131">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="ab0e8-131">requireSignIn</span></span>    | <span data-ttu-id="ab0e8-132">Booleano</span><span class="sxs-lookup"><span data-stu-id="ab0e8-132">Boolean</span></span>                        | <span data-ttu-id="ab0e8-133">Especifica se o destinatário do convite precisa fazer logon para visualizar o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="ab0e8-133">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="ab0e8-134">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="ab0e8-134">sendInvitation</span></span>   | <span data-ttu-id="ab0e8-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="ab0e8-135">Boolean</span></span>                        | <span data-ttu-id="ab0e8-136">Se verdadeiro, um [link de compartilhamento][] será enviado ao destinatário.</span><span class="sxs-lookup"><span data-stu-id="ab0e8-136">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="ab0e8-137">Caso contrário, uma permissão é concedida diretamente sem enviar uma notificação.</span><span class="sxs-lookup"><span data-stu-id="ab0e8-137">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="ab0e8-138">funções</span><span class="sxs-lookup"><span data-stu-id="ab0e8-138">roles</span></span>            | <span data-ttu-id="ab0e8-139">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="ab0e8-139">Collection(String)</span></span>             | <span data-ttu-id="ab0e8-140">Especifique as funções que devem ser concedidas aos destinatários do convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="ab0e8-140">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>
| <span data-ttu-id="ab0e8-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ab0e8-141">expirationDateTime</span></span> | <span data-ttu-id="ab0e8-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab0e8-142">DateTimeOffset</span></span>                       | <span data-ttu-id="ab0e8-143">Especifique a Data e Hora após a qual a permissão expira.</span><span class="sxs-lookup"><span data-stu-id="ab0e8-143">Specify the DateTime after which the permission expires.</span></span> <span data-ttu-id="ab0e8-144">Disponível nas contas do OneDrive for Business, SharePoint e premium personal do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ab0e8-144">Available on OneDrive for Business, SharePoint, and premium personal OneDrive accounts.</span></span>
| <span data-ttu-id="ab0e8-145">password</span><span class="sxs-lookup"><span data-stu-id="ab0e8-145">password</span></span>           | <span data-ttu-id="ab0e8-146">String</span><span class="sxs-lookup"><span data-stu-id="ab0e8-146">String</span></span>                         | <span data-ttu-id="ab0e8-147">A senha definida no convite pelo criador.</span><span class="sxs-lookup"><span data-stu-id="ab0e8-147">The password set on the invite by the creator.</span></span> <span data-ttu-id="ab0e8-148">Opcional e somente OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="ab0e8-148">Optional and OneDrive Personal only.</span></span>

## <a name="example"></a><span data-ttu-id="ab0e8-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab0e8-149">Example</span></span>

<span data-ttu-id="ab0e8-150">Este exemplo envia um convite de compartilhamento para um usuário com o endereço de email "ryan@contoso.com" com uma mensagem sobre um arquivo recebendo colaborações.</span><span class="sxs-lookup"><span data-stu-id="ab0e8-150">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="ab0e8-151">O convite concede acesso de leitura e gravação ao arquivo para Ryan.</span><span class="sxs-lookup"><span data-stu-id="ab0e8-151">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="ab0e8-152">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab0e8-152">HTTP request</span></span>

<span data-ttu-id="ab0e8-153">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto de coleção [permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab0e8-153">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="http"></a>[<span data-ttu-id="ab0e8-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab0e8-154">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```json
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.com"
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
# <a name="c"></a>[<span data-ttu-id="ab0e8-155">C#</span><span class="sxs-lookup"><span data-stu-id="ab0e8-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab0e8-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab0e8-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab0e8-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab0e8-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab0e8-158">Java</span><span class="sxs-lookup"><span data-stu-id="ab0e8-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ab0e8-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab0e8-159">Response</span></span>

<span data-ttu-id="ab0e8-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab0e8-160">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="ab0e8-161">Comentários</span><span class="sxs-lookup"><span data-stu-id="ab0e8-161">Remarks</span></span>

* <span data-ttu-id="ab0e8-162">[Drives](../resources/drive.md) com **driveType** de `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="ab0e8-162">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="ab0e8-163">Para uma lista de funções disponíveis, consulte valores [de propriedade de funções.](../resources/permission.md#roles-property-values)</span><span class="sxs-lookup"><span data-stu-id="ab0e8-163">For a list of available roles, see [roles property values](../resources/permission.md#roles-property-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="ab0e8-164">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="ab0e8-164">Error responses</span></span>

<span data-ttu-id="ab0e8-165">Veja mais informações sobre como os erros são retornados no tópico [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="ab0e8-165">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[link de compartilhamento]: ../resources/permission.md#sharing-links
[sharing link]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
  ]
} -->

