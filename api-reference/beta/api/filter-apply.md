---
title: 'Filter: apply'
description: Aplica os critérios de filtro determinados à coluna fornecida.
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: d250953f7df09162a778cac878259e6aa27ab4f1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811200"
---
# <a name="filter-apply"></a><span data-ttu-id="64285-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="64285-103">Filter: apply</span></span>

<span data-ttu-id="64285-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64285-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64285-105">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="64285-105">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="64285-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="64285-106">Permissions</span></span>
<span data-ttu-id="64285-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64285-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64285-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64285-109">Permission type</span></span>      | <span data-ttu-id="64285-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64285-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64285-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64285-111">Delegated (work or school account)</span></span> | <span data-ttu-id="64285-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64285-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="64285-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64285-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64285-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64285-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="64285-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64285-115">Application</span></span> | <span data-ttu-id="64285-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64285-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64285-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64285-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="64285-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64285-118">Request headers</span></span>
| <span data-ttu-id="64285-119">Nome</span><span class="sxs-lookup"><span data-stu-id="64285-119">Name</span></span>       | <span data-ttu-id="64285-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="64285-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="64285-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="64285-121">Authorization</span></span>  | <span data-ttu-id="64285-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64285-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64285-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64285-124">Request body</span></span>
<span data-ttu-id="64285-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64285-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="64285-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="64285-126">Parameter</span></span>    | <span data-ttu-id="64285-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="64285-127">Type</span></span>   |<span data-ttu-id="64285-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="64285-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64285-129">criteria</span><span class="sxs-lookup"><span data-stu-id="64285-129">criteria</span></span>|<span data-ttu-id="64285-130">workbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="64285-130">workbookFilterCriteria</span></span>|<span data-ttu-id="64285-131">Os critérios a aplicar.</span><span class="sxs-lookup"><span data-stu-id="64285-131">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="64285-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="64285-132">Response</span></span>

<span data-ttu-id="64285-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64285-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64285-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64285-135">Example</span></span>
<span data-ttu-id="64285-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="64285-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="64285-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64285-137">Request</span></span>
<span data-ttu-id="64285-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64285-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64285-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="64285-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="64285-140">C#</span><span class="sxs-lookup"><span data-stu-id="64285-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64285-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64285-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64285-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64285-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="64285-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="64285-143">Response</span></span>
<span data-ttu-id="64285-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64285-144">Here is an example of the response.</span></span>
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
