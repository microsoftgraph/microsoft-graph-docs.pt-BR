---
title: 'Range: Column'
description: Obtém uma coluna incluída no intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 50be67a2216583bb3b9b8d8b8d144cea28737b5e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857209"
---
# <a name="range-column"></a><span data-ttu-id="1c6ba-103">Range: Column</span><span class="sxs-lookup"><span data-stu-id="1c6ba-103">Range: Column</span></span>

<span data-ttu-id="1c6ba-104">Obtém uma coluna incluída no intervalo.</span><span class="sxs-lookup"><span data-stu-id="1c6ba-104">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c6ba-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c6ba-105">Permissions</span></span>
<span data-ttu-id="1c6ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c6ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c6ba-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c6ba-108">Permission type</span></span>      | <span data-ttu-id="1c6ba-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c6ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c6ba-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c6ba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1c6ba-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c6ba-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1c6ba-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c6ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c6ba-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c6ba-113">Not supported.</span></span>    |
|<span data-ttu-id="1c6ba-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c6ba-114">Application</span></span> | <span data-ttu-id="1c6ba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c6ba-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c6ba-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c6ba-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1c6ba-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c6ba-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/column
GET /workbook/worksheets/{id|name}/range(address='<address>')/column
GET /workbook/tables/{id|name}/columns/{id|name}/range/column

```
## <a name="request-headers"></a><span data-ttu-id="1c6ba-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c6ba-118">Request headers</span></span>
| <span data-ttu-id="1c6ba-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1c6ba-119">Name</span></span>       | <span data-ttu-id="1c6ba-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c6ba-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1c6ba-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c6ba-121">Authorization</span></span>  | <span data-ttu-id="1c6ba-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c6ba-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1c6ba-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1c6ba-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1c6ba-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1c6ba-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="1c6ba-127">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="1c6ba-127">Path parameters</span></span>
<span data-ttu-id="1c6ba-128">No caminho da solicitação, forneça os seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="1c6ba-128">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="1c6ba-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1c6ba-129">Parameter</span></span>    | <span data-ttu-id="1c6ba-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c6ba-130">Type</span></span>   |<span data-ttu-id="1c6ba-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c6ba-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c6ba-132">column</span><span class="sxs-lookup"><span data-stu-id="1c6ba-132">column</span></span>|<span data-ttu-id="1c6ba-133">Int32</span><span class="sxs-lookup"><span data-stu-id="1c6ba-133">Int32</span></span>|<span data-ttu-id="1c6ba-p104">O número da coluna do intervalo a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="1c6ba-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="1c6ba-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c6ba-136">Response</span></span>

<span data-ttu-id="1c6ba-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c6ba-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c6ba-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c6ba-138">Example</span></span>
<span data-ttu-id="1c6ba-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1c6ba-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1c6ba-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c6ba-140">Request</span></span>
<span data-ttu-id="1c6ba-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c6ba-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1c6ba-142">C#</span><span class="sxs-lookup"><span data-stu-id="1c6ba-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-column-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1c6ba-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="1c6ba-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-column-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1c6ba-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1c6ba-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-column-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1c6ba-145">Java</span><span class="sxs-lookup"><span data-stu-id="1c6ba-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-column-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1c6ba-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c6ba-146">Response</span></span>
<span data-ttu-id="1c6ba-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c6ba-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
