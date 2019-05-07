---
title: 'Range: UsedRange'
description: Retorna o intervalo usado do objeto range determinado.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 97ea9cd720b38b774aa262eee53a1457bc2c842d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607921"
---
# <a name="range-usedrange"></a><span data-ttu-id="0792c-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="0792c-103">Range: UsedRange</span></span>

<span data-ttu-id="0792c-104">Retorna o intervalo usado do objeto range determinado.</span><span class="sxs-lookup"><span data-stu-id="0792c-104">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0792c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0792c-105">Permissions</span></span>
<span data-ttu-id="0792c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0792c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0792c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0792c-108">Permission type</span></span>      | <span data-ttu-id="0792c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0792c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0792c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0792c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0792c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0792c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0792c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0792c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0792c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0792c-113">Not supported.</span></span>    |
|<span data-ttu-id="0792c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0792c-114">Application</span></span> | <span data-ttu-id="0792c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0792c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0792c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0792c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/usedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="0792c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0792c-117">Request headers</span></span>
| <span data-ttu-id="0792c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0792c-118">Name</span></span>       | <span data-ttu-id="0792c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0792c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0792c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0792c-120">Authorization</span></span>  | <span data-ttu-id="0792c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0792c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0792c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0792c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0792c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0792c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="0792c-126">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="0792c-126">Path parameters</span></span>
| <span data-ttu-id="0792c-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0792c-127">Parameter</span></span>    | <span data-ttu-id="0792c-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="0792c-128">Type</span></span>   |<span data-ttu-id="0792c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="0792c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0792c-130">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="0792c-130">valuesOnly</span></span>|<span data-ttu-id="0792c-131">booliano</span><span class="sxs-lookup"><span data-stu-id="0792c-131">boolean</span></span>|<span data-ttu-id="0792c-p104">Opcional. Considera apenas as células com valores como células usadas.</span><span class="sxs-lookup"><span data-stu-id="0792c-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="0792c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0792c-134">Response</span></span>

<span data-ttu-id="0792c-135">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0792c-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0792c-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0792c-136">Example</span></span>
<span data-ttu-id="0792c-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0792c-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0792c-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0792c-138">Request</span></span>
<span data-ttu-id="0792c-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0792c-139">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```

##### <a name="response"></a><span data-ttu-id="0792c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0792c-140">Response</span></span>
<span data-ttu-id="0792c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0792c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0792c-144">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="0792c-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0792c-145">Basic</span><span class="sxs-lookup"><span data-stu-id="0792c-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_usedrange-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0792c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0792c-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_usedrange-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="0792c-147">Veja um exemplo que especifica o parâmetro `valuesOnly` opcional.</span><span class="sxs-lookup"><span data-stu-id="0792c-147">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="0792c-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0792c-148">Request</span></span>
<span data-ttu-id="0792c-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0792c-149">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="0792c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="0792c-150">Response</span></span>

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
  "cellCount": 90,
  "columnCount": 90,
  "columnIndex": 90,
  "valueTypes": "valueTypes-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0792c-151">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="0792c-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0792c-152">Basic</span><span class="sxs-lookup"><span data-stu-id="0792c-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_usedrange_valuesonly-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0792c-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0792c-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_usedrange_valuesonly-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/range-usedrange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-usedrange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/range-usedrange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-usedrange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
