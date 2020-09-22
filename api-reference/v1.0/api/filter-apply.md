---
title: 'Filter: apply'
description: Aplica os critérios de filtro determinados à coluna fornecida.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 51d78cf2d839968a9683c7ecab910ce0aeccb611
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038645"
---
# <a name="filter-apply"></a><span data-ttu-id="6f8fc-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="6f8fc-103">Filter: apply</span></span>

<span data-ttu-id="6f8fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f8fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f8fc-105">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="6f8fc-105">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="6f8fc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f8fc-106">Permissions</span></span>
<span data-ttu-id="6f8fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f8fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f8fc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f8fc-109">Permission type</span></span>      | <span data-ttu-id="6f8fc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f8fc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f8fc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f8fc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6f8fc-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f8fc-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6f8fc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f8fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f8fc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f8fc-114">Not supported.</span></span>    |
|<span data-ttu-id="6f8fc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f8fc-115">Application</span></span> | <span data-ttu-id="6f8fc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f8fc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f8fc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f8fc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="6f8fc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f8fc-118">Request headers</span></span>
| <span data-ttu-id="6f8fc-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6f8fc-119">Name</span></span>       | <span data-ttu-id="6f8fc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f8fc-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6f8fc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f8fc-121">Authorization</span></span>  | <span data-ttu-id="6f8fc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f8fc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f8fc-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f8fc-124">Request body</span></span>
<span data-ttu-id="6f8fc-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f8fc-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6f8fc-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6f8fc-126">Parameter</span></span>    | <span data-ttu-id="6f8fc-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f8fc-127">Type</span></span>   |<span data-ttu-id="6f8fc-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f8fc-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f8fc-129">criteria</span><span class="sxs-lookup"><span data-stu-id="6f8fc-129">criteria</span></span>|<span data-ttu-id="6f8fc-130">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="6f8fc-130">WorkbookFilterCriteria</span></span>|<span data-ttu-id="6f8fc-131">Os critérios a aplicar.</span><span class="sxs-lookup"><span data-stu-id="6f8fc-131">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="6f8fc-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f8fc-132">Response</span></span>

<span data-ttu-id="6f8fc-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f8fc-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f8fc-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f8fc-135">Example</span></span>
<span data-ttu-id="6f8fc-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6f8fc-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6f8fc-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f8fc-137">Request</span></span>
<span data-ttu-id="6f8fc-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f8fc-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6f8fc-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f8fc-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
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
# <a name="c"></a>[<span data-ttu-id="6f8fc-140">C#</span><span class="sxs-lookup"><span data-stu-id="6f8fc-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f8fc-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f8fc-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f8fc-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f8fc-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f8fc-143">Java</span><span class="sxs-lookup"><span data-stu-id="6f8fc-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6f8fc-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f8fc-144">Response</span></span>
<span data-ttu-id="6f8fc-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f8fc-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

