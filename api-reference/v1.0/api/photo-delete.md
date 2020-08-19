---
title: Excluir foto
description: Exclua uma foto.
localization_priority: Normal
author: kevinbellinger
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 57cc725d5b668d4db72ec9b96c3be0cbdf20db46
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808743"
---
# <a name="delete-photo"></a><span data-ttu-id="c0dd7-103">Excluir foto</span><span class="sxs-lookup"><span data-stu-id="c0dd7-103">Delete photo</span></span>

<span data-ttu-id="c0dd7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0dd7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0dd7-105">Exclua uma foto.</span><span class="sxs-lookup"><span data-stu-id="c0dd7-105">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="c0dd7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0dd7-106">Permissions</span></span>
<span data-ttu-id="c0dd7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0dd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0dd7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0dd7-109">Permission type</span></span>      | <span data-ttu-id="c0dd7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0dd7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0dd7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0dd7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c0dd7-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0dd7-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0dd7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0dd7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0dd7-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0dd7-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0dd7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0dd7-115">Application</span></span> | <span data-ttu-id="c0dd7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0dd7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0dd7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0dd7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="c0dd7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0dd7-118">Request headers</span></span>
| <span data-ttu-id="c0dd7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c0dd7-119">Name</span></span>       | <span data-ttu-id="c0dd7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0dd7-120">Type</span></span> | <span data-ttu-id="c0dd7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0dd7-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c0dd7-122">if-match</span><span class="sxs-lookup"><span data-stu-id="c0dd7-122">if-match</span></span>  | <span data-ttu-id="c0dd7-123">string</span><span class="sxs-lookup"><span data-stu-id="c0dd7-123">string</span></span>  | <span data-ttu-id="c0dd7-124">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="c0dd7-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="c0dd7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0dd7-125">Authorization</span></span>  | <span data-ttu-id="c0dd7-126">string</span><span class="sxs-lookup"><span data-stu-id="c0dd7-126">string</span></span>  | <span data-ttu-id="c0dd7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0dd7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0dd7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0dd7-129">Request body</span></span>
<span data-ttu-id="c0dd7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0dd7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0dd7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0dd7-131">Response</span></span>

<span data-ttu-id="c0dd7-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0dd7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0dd7-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0dd7-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0dd7-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0dd7-135">Request</span></span>
<span data-ttu-id="c0dd7-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0dd7-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0dd7-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0dd7-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
# <a name="c"></a>[<span data-ttu-id="c0dd7-138">C#</span><span class="sxs-lookup"><span data-stu-id="c0dd7-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0dd7-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0dd7-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0dd7-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0dd7-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0dd7-141">Java</span><span class="sxs-lookup"><span data-stu-id="c0dd7-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-photo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c0dd7-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0dd7-142">Response</span></span>
<span data-ttu-id="c0dd7-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0dd7-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
