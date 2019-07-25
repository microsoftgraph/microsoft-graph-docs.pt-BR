---
title: Excluir contactFolder
description: Exclui uma contactFolder que não a padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b742688b694f82eb60a5c6f8b9e4e8fe6cb8cdef
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884014"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="b4ee6-103">Excluir contactFolder</span><span class="sxs-lookup"><span data-stu-id="b4ee6-103">Delete contactFolder</span></span>

<span data-ttu-id="b4ee6-104">Exclui uma contactFolder que não a padrão.</span><span class="sxs-lookup"><span data-stu-id="b4ee6-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="b4ee6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b4ee6-105">Permissions</span></span>
<span data-ttu-id="b4ee6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4ee6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4ee6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4ee6-108">Permission type</span></span>      | <span data-ttu-id="b4ee6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b4ee6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4ee6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4ee6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b4ee6-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4ee6-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b4ee6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4ee6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4ee6-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4ee6-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b4ee6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4ee6-114">Application</span></span> | <span data-ttu-id="b4ee6-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4ee6-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4ee6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4ee6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b4ee6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4ee6-117">Request headers</span></span>
| <span data-ttu-id="b4ee6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b4ee6-118">Name</span></span>       | <span data-ttu-id="b4ee6-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4ee6-119">Type</span></span> | <span data-ttu-id="b4ee6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4ee6-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b4ee6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4ee6-121">Authorization</span></span>  | <span data-ttu-id="b4ee6-122">string</span><span class="sxs-lookup"><span data-stu-id="b4ee6-122">string</span></span>  | <span data-ttu-id="b4ee6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4ee6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4ee6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4ee6-125">Request body</span></span>
<span data-ttu-id="b4ee6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b4ee6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4ee6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4ee6-127">Response</span></span>

<span data-ttu-id="b4ee6-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4ee6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4ee6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4ee6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4ee6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4ee6-131">Request</span></span>
<span data-ttu-id="b4ee6-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4ee6-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b4ee6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4ee6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b4ee6-134">C#</span><span class="sxs-lookup"><span data-stu-id="b4ee6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4ee6-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="b4ee6-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b4ee6-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b4ee6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b4ee6-137">Java</span><span class="sxs-lookup"><span data-stu-id="b4ee6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b4ee6-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4ee6-138">Response</span></span>
<span data-ttu-id="b4ee6-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4ee6-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
