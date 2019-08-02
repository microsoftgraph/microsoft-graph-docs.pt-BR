---
title: 'Range: Column'
description: Obtém uma coluna incluída no intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9942d09a0c47ee47b7b1a2781bbee87c636cd2f8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025348"
---
# <a name="range-column"></a><span data-ttu-id="81dc4-103">Range: Column</span><span class="sxs-lookup"><span data-stu-id="81dc4-103">Range: Column</span></span>

<span data-ttu-id="81dc4-104">Obtém uma coluna incluída no intervalo.</span><span class="sxs-lookup"><span data-stu-id="81dc4-104">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="81dc4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="81dc4-105">Permissions</span></span>
<span data-ttu-id="81dc4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81dc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81dc4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81dc4-108">Permission type</span></span>      | <span data-ttu-id="81dc4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81dc4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81dc4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81dc4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="81dc4-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81dc4-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="81dc4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81dc4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81dc4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81dc4-113">Not supported.</span></span>    |
|<span data-ttu-id="81dc4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81dc4-114">Application</span></span> | <span data-ttu-id="81dc4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81dc4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81dc4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81dc4-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="81dc4-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="81dc4-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/column
GET /workbook/worksheets/{id|name}/range(address='<address>')/column
GET /workbook/tables/{id|name}/columns/{id|name}/range/column

```
## <a name="request-headers"></a><span data-ttu-id="81dc4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81dc4-118">Request headers</span></span>
| <span data-ttu-id="81dc4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="81dc4-119">Name</span></span>       | <span data-ttu-id="81dc4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="81dc4-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="81dc4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="81dc4-121">Authorization</span></span>  | <span data-ttu-id="81dc4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81dc4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81dc4-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="81dc4-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="81dc4-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="81dc4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="81dc4-127">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="81dc4-127">Path parameters</span></span>
<span data-ttu-id="81dc4-128">No caminho da solicitação, forneça os seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="81dc4-128">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="81dc4-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="81dc4-129">Parameter</span></span>    | <span data-ttu-id="81dc4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="81dc4-130">Type</span></span>   |<span data-ttu-id="81dc4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="81dc4-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81dc4-132">column</span><span class="sxs-lookup"><span data-stu-id="81dc4-132">column</span></span>|<span data-ttu-id="81dc4-133">Int32</span><span class="sxs-lookup"><span data-stu-id="81dc4-133">Int32</span></span>|<span data-ttu-id="81dc4-p104">O número da coluna do intervalo a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="81dc4-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="81dc4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="81dc4-136">Response</span></span>

<span data-ttu-id="81dc4-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81dc4-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81dc4-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81dc4-138">Example</span></span>
<span data-ttu-id="81dc4-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="81dc4-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="81dc4-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81dc4-140">Request</span></span>
<span data-ttu-id="81dc4-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81dc4-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="81dc4-142">C#</span><span class="sxs-lookup"><span data-stu-id="81dc4-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-column-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="81dc4-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="81dc4-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-column-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="81dc4-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="81dc4-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-column-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="81dc4-145">Java</span><span class="sxs-lookup"><span data-stu-id="81dc4-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-column-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="81dc4-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="81dc4-146">Response</span></span>
<span data-ttu-id="81dc4-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81dc4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
