---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Enviar um convite para acessar um item
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 37e2bc8a383f5078c413ccc37f369442f55b597c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272860"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="733f8-102">Enviar um convite de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="733f8-102">Send a sharing invitation</span></span>

<span data-ttu-id="733f8-103">Envia um convite de compartilhamento para um **DriveItem**.</span><span class="sxs-lookup"><span data-stu-id="733f8-103">Sends a sharing invitation for a **DriveItem**.</span></span>
<span data-ttu-id="733f8-104">Um convite de compartilhamento fornece permissões aos destinatários e, opcionalmente, os envia um email com um [link de compartilhamento][].</span><span class="sxs-lookup"><span data-stu-id="733f8-104">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="733f8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="733f8-105">Permissions</span></span>

<span data-ttu-id="733f8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="733f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="733f8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="733f8-108">Permission type</span></span>      | <span data-ttu-id="733f8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="733f8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="733f8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="733f8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="733f8-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="733f8-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="733f8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="733f8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="733f8-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="733f8-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="733f8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="733f8-114">Application</span></span> | <span data-ttu-id="733f8-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="733f8-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="733f8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="733f8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="733f8-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="733f8-117">Request body</span></span>

<span data-ttu-id="733f8-118">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="733f8-118">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="733f8-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="733f8-119">Parameter</span></span>        | <span data-ttu-id="733f8-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="733f8-120">Type</span></span>                           | <span data-ttu-id="733f8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="733f8-121">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="733f8-122">destinatários</span><span class="sxs-lookup"><span data-stu-id="733f8-122">recipients</span></span>       | <span data-ttu-id="733f8-123">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="733f8-123">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="733f8-124">Uma coleção dos destinatários que receberão o acesso e o convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="733f8-124">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="733f8-125">mensagem</span><span class="sxs-lookup"><span data-stu-id="733f8-125">message</span></span>          | <span data-ttu-id="733f8-126">String</span><span class="sxs-lookup"><span data-stu-id="733f8-126">String</span></span>                         | <span data-ttu-id="733f8-p103">Uma mensagem de texto sem formatação que está incluída no convite de compartilhamento. Comprimento máximo de 2000 caracteres.</span><span class="sxs-lookup"><span data-stu-id="733f8-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="733f8-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="733f8-129">requireSignIn</span></span>    | <span data-ttu-id="733f8-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="733f8-130">Boolean</span></span>                        | <span data-ttu-id="733f8-131">Especifica se o destinatário do convite deve entrar para exibir o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="733f8-131">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="733f8-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="733f8-132">sendInvitation</span></span>   | <span data-ttu-id="733f8-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="733f8-133">Boolean</span></span>                        | <span data-ttu-id="733f8-134">Se true, um [link de compartilhamento][] é enviado para o destinatário.</span><span class="sxs-lookup"><span data-stu-id="733f8-134">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="733f8-135">Caso contrário, uma permissão é concedida diretamente sem enviar uma notificação.</span><span class="sxs-lookup"><span data-stu-id="733f8-135">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="733f8-136">funções</span><span class="sxs-lookup"><span data-stu-id="733f8-136">roles</span></span>            | <span data-ttu-id="733f8-137">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="733f8-137">Collection(String)</span></span>             | <span data-ttu-id="733f8-138">Especifique as funções que devem ser concedidas aos destinatários do convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="733f8-138">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>

## <a name="example"></a><span data-ttu-id="733f8-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="733f8-139">Example</span></span>

<span data-ttu-id="733f8-140">Este exemplo envia um convite de compartilhamento para um usuário com o endereço de email "ryan@contoso.com" com uma mensagem sobre um arquivo que está sendo colaborado.</span><span class="sxs-lookup"><span data-stu-id="733f8-140">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="733f8-141">O convite concede acesso de leitura e gravação ao arquivo para Ryan.</span><span class="sxs-lookup"><span data-stu-id="733f8-141">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="733f8-142">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="733f8-142">HTTP Request</span></span>

<span data-ttu-id="733f8-143">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto de coleção [permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="733f8-143">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

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

### <a name="response"></a><span data-ttu-id="733f8-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="733f8-144">Response</span></span>

<span data-ttu-id="733f8-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="733f8-145">Here is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="733f8-146">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="733f8-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="733f8-147">C#</span><span class="sxs-lookup"><span data-stu-id="733f8-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/send-sharing-invite-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="733f8-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="733f8-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/send-sharing-invite-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="733f8-149">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="733f8-149">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/send-sharing-invite-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="733f8-150">Comentários</span><span class="sxs-lookup"><span data-stu-id="733f8-150">Remarks</span></span>

* <span data-ttu-id="733f8-151">[Drives](../resources/drive.md) com **driveType** de `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="733f8-151">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="733f8-152">Para obter uma lista das funções disponíveis, consulte [Funções de enumeração](../resources/permission.md#roles-enumeration).</span><span class="sxs-lookup"><span data-stu-id="733f8-152">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

## <a name="error-responses"></a><span data-ttu-id="733f8-153">Respostas de Erro</span><span class="sxs-lookup"><span data-stu-id="733f8-153">Error Responses</span></span>

<span data-ttu-id="733f8-154">Saiba mais sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="733f8-154">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


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
    "Error: /api-reference/v1.0/api/driveitem-invite.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/driveitem-invite.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-invite.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
