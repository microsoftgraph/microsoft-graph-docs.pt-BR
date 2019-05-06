---
title: 'Filter: apply'
description: Aplica os critérios de filtro determinados à coluna fornecida.
localization_priority: Normal
ms.openlocfilehash: 44c08067b6202d445f18b92f31ad87e4520eb9c5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33586413"
---
# <a name="filter-apply"></a><span data-ttu-id="63508-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="63508-103">Filter: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63508-104">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="63508-104">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="63508-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="63508-105">Permissions</span></span>
<span data-ttu-id="63508-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63508-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63508-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63508-108">Permission type</span></span>      | <span data-ttu-id="63508-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63508-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63508-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63508-110">Delegated (work or school account)</span></span> | <span data-ttu-id="63508-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63508-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="63508-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63508-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63508-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63508-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="63508-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63508-114">Application</span></span> | <span data-ttu-id="63508-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63508-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63508-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63508-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="63508-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63508-117">Request headers</span></span>
| <span data-ttu-id="63508-118">Nome</span><span class="sxs-lookup"><span data-stu-id="63508-118">Name</span></span>       | <span data-ttu-id="63508-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="63508-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="63508-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="63508-120">Authorization</span></span>  | <span data-ttu-id="63508-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63508-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63508-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63508-123">Request body</span></span>
<span data-ttu-id="63508-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63508-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="63508-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="63508-125">Parameter</span></span>    | <span data-ttu-id="63508-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="63508-126">Type</span></span>   |<span data-ttu-id="63508-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="63508-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63508-128">criteria</span><span class="sxs-lookup"><span data-stu-id="63508-128">criteria</span></span>|<span data-ttu-id="63508-129">workbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="63508-129">workbookFilterCriteria</span></span>|<span data-ttu-id="63508-130">Os critérios a aplicar.</span><span class="sxs-lookup"><span data-stu-id="63508-130">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="63508-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="63508-131">Response</span></span>

<span data-ttu-id="63508-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63508-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63508-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63508-134">Example</span></span>
<span data-ttu-id="63508-135">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="63508-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="63508-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63508-136">Request</span></span>
<span data-ttu-id="63508-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63508-137">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="63508-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="63508-138">Response</span></span>
<span data-ttu-id="63508-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63508-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="63508-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="63508-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="63508-141">Basic</span><span class="sxs-lookup"><span data-stu-id="63508-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/filter_apply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63508-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63508-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/filter_apply-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/filter-apply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/filter-apply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
