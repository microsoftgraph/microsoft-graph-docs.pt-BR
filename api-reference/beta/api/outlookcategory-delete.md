---
title: Excluir categoria do Outlook
description: Exclua o objeto outlookCategory especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 096f1d42efdda9f7970d0f629fbc706a0ecc58ac
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265811"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="4157d-103">Excluir categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="4157d-103">Delete Outlook category</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4157d-104">Exclua o objeto [outlookCategory](../resources/outlookcategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="4157d-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4157d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4157d-105">Permissions</span></span>
<span data-ttu-id="4157d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4157d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4157d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4157d-108">Permission type</span></span>      | <span data-ttu-id="4157d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4157d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4157d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4157d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4157d-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4157d-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="4157d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4157d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4157d-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4157d-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="4157d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4157d-114">Application</span></span> | <span data-ttu-id="4157d-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4157d-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4157d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4157d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4157d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4157d-117">Request headers</span></span>
| <span data-ttu-id="4157d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4157d-118">Name</span></span>      |<span data-ttu-id="4157d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4157d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4157d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="4157d-120">Authorization</span></span>  | <span data-ttu-id="4157d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4157d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4157d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4157d-123">Request body</span></span>
<span data-ttu-id="4157d-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4157d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4157d-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="4157d-125">Response</span></span>

<span data-ttu-id="4157d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4157d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4157d-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4157d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4157d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4157d-129">Request</span></span>
<span data-ttu-id="4157d-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4157d-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
##### <a name="response"></a><span data-ttu-id="4157d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4157d-131">Response</span></span>
<span data-ttu-id="4157d-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4157d-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4157d-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="4157d-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4157d-134">C#</span><span class="sxs-lookup"><span data-stu-id="4157d-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_outlookcategory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4157d-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="4157d-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_outlookcategory-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4157d-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4157d-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_outlookcategory-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookcategory-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlookcategory-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookcategory-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
