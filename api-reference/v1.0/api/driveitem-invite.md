---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Enviar um convite para acessar um item
localization_priority: Normal
ms.prod: sharepoint
description: Envia um convite de compartilhamento para um DriveItem.
doc_type: apiPageType
ms.openlocfilehash: 47aa7e49875d4d07ebc8b80a0f86c5939aea13ec
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375041"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="2492c-103">Enviar um convite de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="2492c-103">Send a sharing invitation</span></span>

<span data-ttu-id="2492c-104">Envia um convite de compartilhamento para um **DriveItem**.</span><span class="sxs-lookup"><span data-stu-id="2492c-104">Sends a sharing invitation for a **DriveItem**.</span></span>
<span data-ttu-id="2492c-105">Um convite de compartilhamento fornece permissões aos destinatários e, opcionalmente, os envia um email com um [link de compartilhamento][].</span><span class="sxs-lookup"><span data-stu-id="2492c-105">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="2492c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2492c-106">Permissions</span></span>

<span data-ttu-id="2492c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2492c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2492c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2492c-109">Permission type</span></span>      | <span data-ttu-id="2492c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2492c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2492c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2492c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2492c-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2492c-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2492c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2492c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2492c-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2492c-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2492c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2492c-115">Application</span></span> | <span data-ttu-id="2492c-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2492c-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2492c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2492c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="2492c-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2492c-118">Request body</span></span>

<span data-ttu-id="2492c-119">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2492c-119">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="2492c-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2492c-120">Parameter</span></span>        | <span data-ttu-id="2492c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2492c-121">Type</span></span>                           | <span data-ttu-id="2492c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2492c-122">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="2492c-123">destinatários</span><span class="sxs-lookup"><span data-stu-id="2492c-123">recipients</span></span>       | <span data-ttu-id="2492c-124">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="2492c-124">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="2492c-125">Uma coleção dos destinatários que receberão o acesso e o convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="2492c-125">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="2492c-126">mensagem</span><span class="sxs-lookup"><span data-stu-id="2492c-126">message</span></span>          | <span data-ttu-id="2492c-127">String</span><span class="sxs-lookup"><span data-stu-id="2492c-127">String</span></span>                         | <span data-ttu-id="2492c-p103">Uma mensagem de texto sem formatação que está incluída no convite de compartilhamento. Comprimento máximo de 2000 caracteres.</span><span class="sxs-lookup"><span data-stu-id="2492c-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="2492c-130">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="2492c-130">requireSignIn</span></span>    | <span data-ttu-id="2492c-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="2492c-131">Boolean</span></span>                        | <span data-ttu-id="2492c-132">Especifica se o destinatário do convite deve entrar para exibir o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="2492c-132">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="2492c-133">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="2492c-133">sendInvitation</span></span>   | <span data-ttu-id="2492c-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="2492c-134">Boolean</span></span>                        | <span data-ttu-id="2492c-135">Se true, um [link de compartilhamento][] é enviado para o destinatário.</span><span class="sxs-lookup"><span data-stu-id="2492c-135">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="2492c-136">Caso contrário, uma permissão é concedida diretamente sem enviar uma notificação.</span><span class="sxs-lookup"><span data-stu-id="2492c-136">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="2492c-137">funções</span><span class="sxs-lookup"><span data-stu-id="2492c-137">roles</span></span>            | <span data-ttu-id="2492c-138">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="2492c-138">Collection(String)</span></span>             | <span data-ttu-id="2492c-139">Especifique as funções que devem ser concedidas aos destinatários do convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="2492c-139">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>

## <a name="example"></a><span data-ttu-id="2492c-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2492c-140">Example</span></span>

<span data-ttu-id="2492c-141">Este exemplo envia um convite de compartilhamento para um usuário com o endereço de email "ryan@contoso.com" com uma mensagem sobre um arquivo que está sendo colaborado.</span><span class="sxs-lookup"><span data-stu-id="2492c-141">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="2492c-142">O convite concede acesso de leitura e gravação ao arquivo para Ryan.</span><span class="sxs-lookup"><span data-stu-id="2492c-142">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="2492c-143">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2492c-143">HTTP Request</span></span>

<span data-ttu-id="2492c-144">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto de coleção [permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2492c-144">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2492c-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="2492c-145">HTTP</span></span>](#tab/http)
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
  "roles": [ "write" ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2492c-146">C#</span><span class="sxs-lookup"><span data-stu-id="2492c-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2492c-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2492c-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2492c-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2492c-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2492c-149">Java</span><span class="sxs-lookup"><span data-stu-id="2492c-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2492c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="2492c-150">Response</span></span>

<span data-ttu-id="2492c-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2492c-151">Here is an example of the response.</span></span>

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
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="2492c-152">Comentários</span><span class="sxs-lookup"><span data-stu-id="2492c-152">Remarks</span></span>

* <span data-ttu-id="2492c-153">[Drives](../resources/drive.md) com **driveType** de `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="2492c-153">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="2492c-154">Para obter uma lista das funções disponíveis, consulte [Funções de enumeração](../resources/permission.md#roles-enumeration).</span><span class="sxs-lookup"><span data-stu-id="2492c-154">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

## <a name="error-responses"></a><span data-ttu-id="2492c-155">Respostas de Erro</span><span class="sxs-lookup"><span data-stu-id="2492c-155">Error Responses</span></span>

<span data-ttu-id="2492c-156">Saiba mais sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="2492c-156">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


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
