---
title: 'Filter: apply'
description: Aplica os critérios de filtro determinados à coluna fornecida.
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: c9b9c4c3ef6537548affe095ab1b7bba1bcf0313
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574094"
---
# <a name="filter-apply"></a><span data-ttu-id="2d09f-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="2d09f-103">Filter: apply</span></span>

<span data-ttu-id="2d09f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d09f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d09f-105">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="2d09f-105">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="2d09f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2d09f-106">Permissions</span></span>
<span data-ttu-id="2d09f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d09f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d09f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d09f-109">Permission type</span></span>      | <span data-ttu-id="2d09f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2d09f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d09f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d09f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2d09f-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d09f-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2d09f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d09f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d09f-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d09f-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2d09f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d09f-115">Application</span></span> | <span data-ttu-id="2d09f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d09f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d09f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d09f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="2d09f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d09f-118">Request headers</span></span>
| <span data-ttu-id="2d09f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2d09f-119">Name</span></span>       | <span data-ttu-id="2d09f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d09f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2d09f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d09f-121">Authorization</span></span>  | <span data-ttu-id="2d09f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d09f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d09f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d09f-124">Request body</span></span>
<span data-ttu-id="2d09f-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d09f-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2d09f-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2d09f-126">Parameter</span></span>    | <span data-ttu-id="2d09f-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d09f-127">Type</span></span>   |<span data-ttu-id="2d09f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d09f-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d09f-129">criteria</span><span class="sxs-lookup"><span data-stu-id="2d09f-129">criteria</span></span>|<span data-ttu-id="2d09f-130">workbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="2d09f-130">workbookFilterCriteria</span></span>|<span data-ttu-id="2d09f-131">Os critérios a aplicar.</span><span class="sxs-lookup"><span data-stu-id="2d09f-131">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="2d09f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d09f-132">Response</span></span>

<span data-ttu-id="2d09f-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d09f-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d09f-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d09f-135">Example</span></span>
<span data-ttu-id="2d09f-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2d09f-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2d09f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d09f-137">Request</span></span>
<span data-ttu-id="2d09f-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d09f-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2d09f-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d09f-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2d09f-140">C#</span><span class="sxs-lookup"><span data-stu-id="2d09f-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d09f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d09f-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d09f-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d09f-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d09f-143">Java</span><span class="sxs-lookup"><span data-stu-id="2d09f-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2d09f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d09f-144">Response</span></span>
<span data-ttu-id="2d09f-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d09f-145">Here is an example of the response.</span></span>
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


