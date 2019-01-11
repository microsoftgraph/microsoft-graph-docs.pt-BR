---
title: 'Filter: apply'
description: Aplica os critérios de filtro determinados à coluna fornecida.
localization_priority: Normal
ms.openlocfilehash: e7223c1b3d7cd75356c459f366c1a230eeb06e59
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846141"
---
# <a name="filter-apply"></a><span data-ttu-id="09ff0-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="09ff0-103">Filter: apply</span></span>

<span data-ttu-id="09ff0-104">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="09ff0-104">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="09ff0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="09ff0-105">Permissions</span></span>
<span data-ttu-id="09ff0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09ff0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09ff0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09ff0-108">Permission type</span></span>      | <span data-ttu-id="09ff0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09ff0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09ff0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09ff0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="09ff0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09ff0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="09ff0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09ff0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09ff0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09ff0-113">Not supported.</span></span>    |
|<span data-ttu-id="09ff0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09ff0-114">Application</span></span> | <span data-ttu-id="09ff0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09ff0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="09ff0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09ff0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="09ff0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09ff0-117">Request headers</span></span>
| <span data-ttu-id="09ff0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="09ff0-118">Name</span></span>       | <span data-ttu-id="09ff0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="09ff0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="09ff0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="09ff0-120">Authorization</span></span>  | <span data-ttu-id="09ff0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09ff0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09ff0-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09ff0-123">Request body</span></span>
<span data-ttu-id="09ff0-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09ff0-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="09ff0-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="09ff0-125">Parameter</span></span>    | <span data-ttu-id="09ff0-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="09ff0-126">Type</span></span>   |<span data-ttu-id="09ff0-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="09ff0-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09ff0-128">critérios</span><span class="sxs-lookup"><span data-stu-id="09ff0-128">criteria</span></span>|<span data-ttu-id="09ff0-129">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="09ff0-129">WorkbookFilterCriteria</span></span>|<span data-ttu-id="09ff0-130">Os critérios a aplicar.</span><span class="sxs-lookup"><span data-stu-id="09ff0-130">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="09ff0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="09ff0-131">Response</span></span>

<span data-ttu-id="09ff0-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09ff0-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09ff0-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09ff0-134">Example</span></span>
<span data-ttu-id="09ff0-135">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="09ff0-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="09ff0-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09ff0-136">Request</span></span>
<span data-ttu-id="09ff0-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09ff0-137">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="09ff0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="09ff0-138">Response</span></span>
<span data-ttu-id="09ff0-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09ff0-139">Here is an example of the response.</span></span> 
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
  "tocPath": ""
}-->
