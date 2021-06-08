---
title: 'Filter: apply'
description: Aplica os critérios de filtro determinados à coluna fornecida.
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: 4484f678c85b85fed0b659bfc45a7afaf869c840
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787260"
---
# <a name="filter-apply"></a><span data-ttu-id="66630-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="66630-103">Filter: apply</span></span>

<span data-ttu-id="66630-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66630-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66630-105">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="66630-105">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="66630-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="66630-106">Permissions</span></span>
<span data-ttu-id="66630-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66630-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66630-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66630-109">Permission type</span></span>      | <span data-ttu-id="66630-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66630-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66630-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66630-111">Delegated (work or school account)</span></span> | <span data-ttu-id="66630-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66630-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="66630-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66630-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66630-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66630-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="66630-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66630-115">Application</span></span> | <span data-ttu-id="66630-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66630-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66630-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66630-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="66630-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66630-118">Request headers</span></span>
| <span data-ttu-id="66630-119">Nome</span><span class="sxs-lookup"><span data-stu-id="66630-119">Name</span></span>       | <span data-ttu-id="66630-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="66630-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="66630-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="66630-121">Authorization</span></span>  | <span data-ttu-id="66630-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66630-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66630-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66630-124">Request body</span></span>
<span data-ttu-id="66630-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66630-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="66630-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="66630-126">Parameter</span></span>    | <span data-ttu-id="66630-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="66630-127">Type</span></span>   |<span data-ttu-id="66630-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="66630-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66630-129">criteria</span><span class="sxs-lookup"><span data-stu-id="66630-129">criteria</span></span>|<span data-ttu-id="66630-130">workbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="66630-130">workbookFilterCriteria</span></span>|<span data-ttu-id="66630-131">Os critérios a aplicar.</span><span class="sxs-lookup"><span data-stu-id="66630-131">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="66630-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="66630-132">Response</span></span>

<span data-ttu-id="66630-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66630-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66630-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66630-135">Example</span></span>
<span data-ttu-id="66630-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="66630-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="66630-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66630-137">Request</span></span>
<span data-ttu-id="66630-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66630-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66630-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="66630-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="66630-140">C#</span><span class="sxs-lookup"><span data-stu-id="66630-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66630-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66630-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66630-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66630-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66630-143">Java</span><span class="sxs-lookup"><span data-stu-id="66630-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="66630-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="66630-144">Response</span></span>
<span data-ttu-id="66630-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66630-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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


