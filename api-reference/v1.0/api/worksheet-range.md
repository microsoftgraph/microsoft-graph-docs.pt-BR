---
title: 'Worksheet: Range'
description: Obtém o objeto de intervalo especificado pelo nome ou endereço.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b1ad7b8c1c23400c02ab1833217c86f00b67f493
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601408"
---
# <a name="worksheet-range"></a><span data-ttu-id="2ec0b-103">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="2ec0b-103">Worksheet: Range</span></span>

<span data-ttu-id="2ec0b-104">Obtém o objeto de intervalo especificado pelo nome ou endereço.</span><span class="sxs-lookup"><span data-stu-id="2ec0b-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="2ec0b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ec0b-105">Permissions</span></span>
<span data-ttu-id="2ec0b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ec0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ec0b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ec0b-108">Permission type</span></span>      | <span data-ttu-id="2ec0b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ec0b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ec0b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ec0b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2ec0b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ec0b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2ec0b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ec0b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ec0b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ec0b-113">Not supported.</span></span>    |
|<span data-ttu-id="2ec0b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ec0b-114">Application</span></span> | <span data-ttu-id="2ec0b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ec0b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ec0b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ec0b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="2ec0b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ec0b-117">Request headers</span></span>
| <span data-ttu-id="2ec0b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2ec0b-118">Name</span></span>       | <span data-ttu-id="2ec0b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ec0b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2ec0b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ec0b-120">Authorization</span></span>  | <span data-ttu-id="2ec0b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ec0b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2ec0b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2ec0b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2ec0b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2ec0b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="2ec0b-126">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="2ec0b-126">Function parameters</span></span>

| <span data-ttu-id="2ec0b-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2ec0b-127">Parameter</span></span>    | <span data-ttu-id="2ec0b-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ec0b-128">Type</span></span>   |<span data-ttu-id="2ec0b-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ec0b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ec0b-130">address</span><span class="sxs-lookup"><span data-stu-id="2ec0b-130">address</span></span>|<span data-ttu-id="2ec0b-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ec0b-131">string</span></span>|<span data-ttu-id="2ec0b-p104">Opcional. O endereço ou nome do intervalo. Caso não seja especificado, todo o intervalo da planilha será retornado.</span><span class="sxs-lookup"><span data-stu-id="2ec0b-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="2ec0b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ec0b-135">Response</span></span>

<span data-ttu-id="2ec0b-136">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ec0b-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ec0b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ec0b-137">Example</span></span>
<span data-ttu-id="2ec0b-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2ec0b-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2ec0b-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ec0b-139">Request</span></span>
<span data-ttu-id="2ec0b-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ec0b-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```

##### <a name="response"></a><span data-ttu-id="2ec0b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ec0b-141">Response</span></span>
<span data-ttu-id="2ec0b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ec0b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2ec0b-145">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2ec0b-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2ec0b-146">Basic</span><span class="sxs-lookup"><span data-stu-id="2ec0b-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/worksheet_range-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ec0b-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ec0b-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/worksheet_range-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="2ec0b-148">Se o parâmetro `address` optional não for especificado, essa função retornará todo o intervalo de planilha.</span><span class="sxs-lookup"><span data-stu-id="2ec0b-148">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="2ec0b-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ec0b-149">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```

##### <a name="response"></a><span data-ttu-id="2ec0b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ec0b-150">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2ec0b-151">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2ec0b-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2ec0b-152">Basic</span><span class="sxs-lookup"><span data-stu-id="2ec0b-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/worksheet_range_noaddress-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ec0b-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ec0b-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/worksheet_range_noaddress-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
