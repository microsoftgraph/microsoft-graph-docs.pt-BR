---
title: Excluir foto
description: Exclua uma foto.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: f4e5a1650e2c75ec16c7625597fccd6111d94b83
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976254"
---
# <a name="delete-photo"></a><span data-ttu-id="0e948-103">Excluir foto</span><span class="sxs-lookup"><span data-stu-id="0e948-103">Delete photo</span></span>

<span data-ttu-id="0e948-104">Exclua uma foto.</span><span class="sxs-lookup"><span data-stu-id="0e948-104">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e948-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e948-105">Permissions</span></span>
<span data-ttu-id="0e948-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e948-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e948-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e948-108">Permission type</span></span>      | <span data-ttu-id="0e948-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e948-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e948-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e948-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0e948-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e948-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e948-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e948-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e948-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e948-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e948-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e948-114">Application</span></span> | <span data-ttu-id="0e948-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e948-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e948-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e948-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="0e948-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e948-117">Request headers</span></span>
| <span data-ttu-id="0e948-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0e948-118">Name</span></span>       | <span data-ttu-id="0e948-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e948-119">Type</span></span> | <span data-ttu-id="0e948-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e948-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0e948-121">if-match</span><span class="sxs-lookup"><span data-stu-id="0e948-121">if-match</span></span>  | <span data-ttu-id="0e948-122">string</span><span class="sxs-lookup"><span data-stu-id="0e948-122">string</span></span>  | <span data-ttu-id="0e948-123">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="0e948-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="0e948-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e948-124">Authorization</span></span>  | <span data-ttu-id="0e948-125">string</span><span class="sxs-lookup"><span data-stu-id="0e948-125">string</span></span>  | <span data-ttu-id="0e948-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e948-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e948-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e948-128">Request body</span></span>
<span data-ttu-id="0e948-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0e948-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e948-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e948-130">Response</span></span>

<span data-ttu-id="0e948-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e948-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e948-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e948-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e948-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e948-134">Request</span></span>
<span data-ttu-id="0e948-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e948-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0e948-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e948-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0e948-137">C#</span><span class="sxs-lookup"><span data-stu-id="0e948-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e948-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="0e948-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0e948-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0e948-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0e948-140">Java</span><span class="sxs-lookup"><span data-stu-id="0e948-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-photo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0e948-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e948-141">Response</span></span>
<span data-ttu-id="0e948-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e948-142">Here is an example of the response.</span></span>
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
