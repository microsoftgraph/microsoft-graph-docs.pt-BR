---
title: 'Range: insert'
description: Insere uma célula ou um intervalo de células na planilha, no lugar desse intervalo, e desloca as outras células para liberar espaço. Retorna um novo objeto Range no espaço em branco atual.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: a8d224d14bbfb8463315f84eadbeb0bd4d5d6981
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276025"
---
# <a name="range-insert"></a><span data-ttu-id="a23fb-104">Range: insert</span><span class="sxs-lookup"><span data-stu-id="a23fb-104">Range: insert</span></span>

<span data-ttu-id="a23fb-p102">Insere uma célula ou um intervalo de células na planilha, no lugar desse intervalo, e desloca as outras células para liberar espaço. Retorna um novo objeto Range no espaço em branco atual.</span><span class="sxs-lookup"><span data-stu-id="a23fb-p102">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="a23fb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a23fb-107">Permissions</span></span>
<span data-ttu-id="a23fb-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a23fb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a23fb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a23fb-110">Permission type</span></span>      | <span data-ttu-id="a23fb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a23fb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a23fb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a23fb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a23fb-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a23fb-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a23fb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a23fb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a23fb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a23fb-115">Not supported.</span></span>    |
|<span data-ttu-id="a23fb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a23fb-116">Application</span></span> | <span data-ttu-id="a23fb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a23fb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a23fb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a23fb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/insert
POST /workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="a23fb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a23fb-119">Request headers</span></span>
| <span data-ttu-id="a23fb-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a23fb-120">Name</span></span>       | <span data-ttu-id="a23fb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a23fb-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a23fb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a23fb-122">Authorization</span></span>  | <span data-ttu-id="a23fb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a23fb-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a23fb-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a23fb-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a23fb-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a23fb-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a23fb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a23fb-128">Request body</span></span>
<span data-ttu-id="a23fb-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a23fb-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a23fb-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a23fb-130">Parameter</span></span>    | <span data-ttu-id="a23fb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a23fb-131">Type</span></span>   |<span data-ttu-id="a23fb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a23fb-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a23fb-133">shift</span><span class="sxs-lookup"><span data-stu-id="a23fb-133">shift</span></span>|<span data-ttu-id="a23fb-134">string</span><span class="sxs-lookup"><span data-stu-id="a23fb-134">string</span></span>|<span data-ttu-id="a23fb-135">Especifica como deslocar as células.</span><span class="sxs-lookup"><span data-stu-id="a23fb-135">Specifies which way to shift the cells.</span></span>  <span data-ttu-id="a23fb-136">Os valores possíveis são: `Down`, `Right`.</span><span class="sxs-lookup"><span data-stu-id="a23fb-136">The possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="a23fb-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a23fb-137">Response</span></span>

<span data-ttu-id="a23fb-138">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a23fb-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a23fb-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a23fb-139">Example</span></span>
<span data-ttu-id="a23fb-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a23fb-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a23fb-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a23fb-141">Request</span></span>
<span data-ttu-id="a23fb-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a23fb-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="a23fb-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a23fb-143">Response</span></span>
<span data-ttu-id="a23fb-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a23fb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a23fb-147">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a23fb-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a23fb-148">C#</span><span class="sxs-lookup"><span data-stu-id="a23fb-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_insert-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a23fb-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="a23fb-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_insert-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a23fb-150">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a23fb-150">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/range_insert-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/range-insert.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/range-insert.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-insert.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
