---
title: Excluir contactFolder
description: Exclui uma contactFolder que não a padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1b2b34b1b5d7299fc7e002e26dc9545151dc1108
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943320"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="0697c-103">Excluir contactFolder</span><span class="sxs-lookup"><span data-stu-id="0697c-103">Delete contactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0697c-104">Exclui uma contactFolder que não a padrão.</span><span class="sxs-lookup"><span data-stu-id="0697c-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="0697c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0697c-105">Permissions</span></span>
<span data-ttu-id="0697c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0697c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0697c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0697c-108">Permission type</span></span>      | <span data-ttu-id="0697c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0697c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0697c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0697c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0697c-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0697c-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0697c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0697c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0697c-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0697c-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0697c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0697c-114">Application</span></span> | <span data-ttu-id="0697c-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0697c-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0697c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0697c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0697c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0697c-117">Request headers</span></span>
| <span data-ttu-id="0697c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0697c-118">Name</span></span>       | <span data-ttu-id="0697c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="0697c-119">Type</span></span> | <span data-ttu-id="0697c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0697c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0697c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0697c-121">Authorization</span></span>  | <span data-ttu-id="0697c-122">string</span><span class="sxs-lookup"><span data-stu-id="0697c-122">string</span></span>  | <span data-ttu-id="0697c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0697c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0697c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0697c-125">Request body</span></span>
<span data-ttu-id="0697c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0697c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0697c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0697c-127">Response</span></span>

<span data-ttu-id="0697c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0697c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0697c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0697c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0697c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0697c-131">Request</span></span>
<span data-ttu-id="0697c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0697c-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0697c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0697c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contactFolders/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0697c-134">C#</span><span class="sxs-lookup"><span data-stu-id="0697c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0697c-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="0697c-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0697c-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0697c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0697c-137">Java</span><span class="sxs-lookup"><span data-stu-id="0697c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0697c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0697c-138">Response</span></span>
<span data-ttu-id="0697c-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0697c-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
