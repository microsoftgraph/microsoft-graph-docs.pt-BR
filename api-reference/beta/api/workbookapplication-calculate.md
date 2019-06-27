---
title: 'workbookApplication: calcular'
description: Recalcula todas as pastas de trabalho abertas no Excel no momento.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 653fd377e59570948716c5e663c2802e729e673a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269815"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="8c01a-103">workbookApplication: calcular</span><span class="sxs-lookup"><span data-stu-id="8c01a-103">workbookApplication: calculate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c01a-104">Recalcula todas as pastas de trabalho abertas no Excel no momento.</span><span class="sxs-lookup"><span data-stu-id="8c01a-104">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c01a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c01a-105">Permissions</span></span>
<span data-ttu-id="8c01a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c01a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c01a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c01a-108">Permission type</span></span>      | <span data-ttu-id="8c01a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c01a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c01a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c01a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8c01a-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c01a-111">Not supported.</span></span>    |
|<span data-ttu-id="8c01a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c01a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c01a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c01a-113">Not supported.</span></span>    |
|<span data-ttu-id="8c01a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c01a-114">Application</span></span> | <span data-ttu-id="8c01a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c01a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c01a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c01a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="8c01a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c01a-117">Request headers</span></span>
| <span data-ttu-id="8c01a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8c01a-118">Name</span></span>       | <span data-ttu-id="8c01a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c01a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8c01a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c01a-120">Authorization</span></span>  | <span data-ttu-id="8c01a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c01a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c01a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c01a-123">Request body</span></span>
<span data-ttu-id="8c01a-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c01a-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8c01a-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8c01a-125">Parameter</span></span>    | <span data-ttu-id="8c01a-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c01a-126">Type</span></span>   |<span data-ttu-id="8c01a-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c01a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c01a-128">Calculador de cálculo</span><span class="sxs-lookup"><span data-stu-id="8c01a-128">calculationType</span></span>|<span data-ttu-id="8c01a-129">string</span><span class="sxs-lookup"><span data-stu-id="8c01a-129">string</span></span>|<span data-ttu-id="8c01a-130">Especifica o tipo de cálculo a usar.</span><span class="sxs-lookup"><span data-stu-id="8c01a-130">Specifies the calculation type to use.</span></span>  <span data-ttu-id="8c01a-131">Os valores possíveis são: `Recalculate`, `Full`, `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="8c01a-131">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="8c01a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c01a-132">Response</span></span>

<span data-ttu-id="8c01a-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c01a-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c01a-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c01a-135">Example</span></span>
<span data-ttu-id="8c01a-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8c01a-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8c01a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c01a-137">Request</span></span>
<span data-ttu-id="8c01a-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c01a-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookApplication_calculate"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application/calculate
Content-type: application/json
Content-length: 48

{
  "calculationType": "calculationType-value"
}
```

##### <a name="response"></a><span data-ttu-id="8c01a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c01a-139">Response</span></span>
<span data-ttu-id="8c01a-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c01a-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8c01a-141">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="8c01a-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8c01a-142">C#</span><span class="sxs-lookup"><span data-stu-id="8c01a-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookApplication_calculate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c01a-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="8c01a-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookApplication_calculate-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8c01a-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8c01a-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/workbookApplication_calculate-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookApplication: calculate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookapplication-calculate.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/workbookapplication-calculate.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookapplication-calculate.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
