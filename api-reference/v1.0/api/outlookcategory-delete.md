---
title: Excluir categoria do Outlook
description: Exclua o objeto outlookCategory especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1752d51d7463c575ab5957257132f27c72d78443
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611558"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="a34d4-103">Excluir categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="a34d4-103">Delete Outlook category</span></span>


<span data-ttu-id="a34d4-104">Exclua o objeto [outlookCategory](../resources/outlookcategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="a34d4-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a34d4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a34d4-105">Permissions</span></span>
<span data-ttu-id="a34d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a34d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a34d4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a34d4-108">Permission type</span></span>      | <span data-ttu-id="a34d4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a34d4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a34d4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a34d4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a34d4-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a34d4-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="a34d4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a34d4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a34d4-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a34d4-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="a34d4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a34d4-114">Application</span></span> | <span data-ttu-id="a34d4-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a34d4-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a34d4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a34d4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a34d4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a34d4-117">Request headers</span></span>
| <span data-ttu-id="a34d4-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a34d4-118">Name</span></span>      |<span data-ttu-id="a34d4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a34d4-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a34d4-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a34d4-120">Authorization</span></span>  | <span data-ttu-id="a34d4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a34d4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a34d4-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a34d4-123">Request body</span></span>
<span data-ttu-id="a34d4-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a34d4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a34d4-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="a34d4-125">Response</span></span>

<span data-ttu-id="a34d4-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a34d4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a34d4-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a34d4-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a34d4-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a34d4-129">Request</span></span>
<span data-ttu-id="a34d4-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a34d4-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"],
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
##### <a name="response"></a><span data-ttu-id="a34d4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a34d4-131">Response</span></span>
<span data-ttu-id="a34d4-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a34d4-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a34d4-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a34d4-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a34d4-134">Basic</span><span class="sxs-lookup"><span data-stu-id="a34d4-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_outlookcategory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a34d4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a34d4-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_outlookcategory-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/outlookcategory-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/outlookcategory-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
