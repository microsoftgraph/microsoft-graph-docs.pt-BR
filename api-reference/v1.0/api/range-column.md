---
title: 'Range: Column'
description: Obtém uma coluna incluída no intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4cf776fb1e66ce3088681fe7d2a553af1f9ad685
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607601"
---
# <a name="range-column"></a><span data-ttu-id="47835-103">Range: Column</span><span class="sxs-lookup"><span data-stu-id="47835-103">Range: Column</span></span>

<span data-ttu-id="47835-104">Obtém uma coluna incluída no intervalo.</span><span class="sxs-lookup"><span data-stu-id="47835-104">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="47835-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="47835-105">Permissions</span></span>
<span data-ttu-id="47835-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47835-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47835-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47835-108">Permission type</span></span>      | <span data-ttu-id="47835-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47835-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47835-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47835-110">Delegated (work or school account)</span></span> | <span data-ttu-id="47835-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47835-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="47835-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47835-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47835-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47835-113">Not supported.</span></span>    |
|<span data-ttu-id="47835-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47835-114">Application</span></span> | <span data-ttu-id="47835-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47835-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="47835-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47835-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/column
GET /workbook/worksheets/{id|name}/range(address='<address>')/column
GET /workbook/tables/{id|name}/columns/{id|name}/range/column

```
## <a name="request-headers"></a><span data-ttu-id="47835-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47835-117">Request headers</span></span>
| <span data-ttu-id="47835-118">Nome</span><span class="sxs-lookup"><span data-stu-id="47835-118">Name</span></span>       | <span data-ttu-id="47835-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="47835-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="47835-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="47835-120">Authorization</span></span>  | <span data-ttu-id="47835-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47835-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="47835-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="47835-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="47835-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="47835-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="47835-126">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="47835-126">Path parameters</span></span>
<span data-ttu-id="47835-127">No caminho da solicitação, forneça os seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="47835-127">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="47835-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="47835-128">Parameter</span></span>    | <span data-ttu-id="47835-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="47835-129">Type</span></span>   |<span data-ttu-id="47835-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="47835-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47835-131">column</span><span class="sxs-lookup"><span data-stu-id="47835-131">column</span></span>|<span data-ttu-id="47835-132">Int32</span><span class="sxs-lookup"><span data-stu-id="47835-132">Int32</span></span>|<span data-ttu-id="47835-p104">O número da coluna do intervalo a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="47835-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="47835-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="47835-135">Response</span></span>

<span data-ttu-id="47835-136">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47835-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47835-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47835-137">Example</span></span>
<span data-ttu-id="47835-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="47835-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="47835-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47835-139">Request</span></span>
<span data-ttu-id="47835-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47835-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)
```

##### <a name="response"></a><span data-ttu-id="47835-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="47835-141">Response</span></span>
<span data-ttu-id="47835-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47835-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="47835-145">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="47835-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="47835-146">Basic</span><span class="sxs-lookup"><span data-stu-id="47835-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_column-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="47835-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47835-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_column-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/range-column.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-column.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
