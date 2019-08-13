---
title: 'Filter: apply'
description: Aplica os critérios de filtro determinados à coluna fornecida.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 4ea902dc44fa12383f2a4029414cebba9af61561
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323581"
---
# <a name="filter-apply"></a><span data-ttu-id="abcdb-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="abcdb-103">Filter: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abcdb-104">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="abcdb-104">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="abcdb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="abcdb-105">Permissions</span></span>
<span data-ttu-id="abcdb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abcdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abcdb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abcdb-108">Permission type</span></span>      | <span data-ttu-id="abcdb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="abcdb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abcdb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abcdb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="abcdb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="abcdb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="abcdb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abcdb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abcdb-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="abcdb-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="abcdb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abcdb-114">Application</span></span> | <span data-ttu-id="abcdb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abcdb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="abcdb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abcdb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="abcdb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abcdb-117">Request headers</span></span>
| <span data-ttu-id="abcdb-118">Nome</span><span class="sxs-lookup"><span data-stu-id="abcdb-118">Name</span></span>       | <span data-ttu-id="abcdb-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="abcdb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="abcdb-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="abcdb-120">Authorization</span></span>  | <span data-ttu-id="abcdb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abcdb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="abcdb-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abcdb-123">Request body</span></span>
<span data-ttu-id="abcdb-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abcdb-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="abcdb-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="abcdb-125">Parameter</span></span>    | <span data-ttu-id="abcdb-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="abcdb-126">Type</span></span>   |<span data-ttu-id="abcdb-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="abcdb-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abcdb-128">criteria</span><span class="sxs-lookup"><span data-stu-id="abcdb-128">criteria</span></span>|<span data-ttu-id="abcdb-129">workbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="abcdb-129">workbookFilterCriteria</span></span>|<span data-ttu-id="abcdb-130">Os critérios a aplicar.</span><span class="sxs-lookup"><span data-stu-id="abcdb-130">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="abcdb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="abcdb-131">Response</span></span>

<span data-ttu-id="abcdb-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abcdb-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abcdb-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abcdb-134">Example</span></span>
<span data-ttu-id="abcdb-135">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="abcdb-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="abcdb-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abcdb-136">Request</span></span>
<span data-ttu-id="abcdb-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abcdb-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="abcdb-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="abcdb-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
Content-type: application/json
Content-length: 321

{
  "criteria": {
    "criterion1": "criterion1-value",
    "criterion2": "criterion2-value",
    "color": "color-value",
    "operator": {
    },
    "icon": {
      "set": "set-value",
      "index": 99
    },
    "dynamicCriteria": "dynamicCriteria-value",
    "values": {
    },
    "filterOn": "filterOn-value"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="abcdb-139">C#</span><span class="sxs-lookup"><span data-stu-id="abcdb-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="abcdb-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="abcdb-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="abcdb-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="abcdb-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="abcdb-142">Java</span><span class="sxs-lookup"><span data-stu-id="abcdb-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="abcdb-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="abcdb-143">Response</span></span>
<span data-ttu-id="abcdb-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abcdb-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
