---
title: 'Range: UsedRange'
description: Retorna o intervalo usado do objeto range determinado.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 85100aea78f6478bde9cbf8ce852d6cdfd81a0b6
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412156"
---
# <a name="range-usedrange"></a><span data-ttu-id="90a43-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="90a43-103">Range: UsedRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90a43-104">Retorna o intervalo usado do objeto range determinado.</span><span class="sxs-lookup"><span data-stu-id="90a43-104">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="90a43-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="90a43-105">Permissions</span></span>
<span data-ttu-id="90a43-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90a43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90a43-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90a43-108">Permission type</span></span>      | <span data-ttu-id="90a43-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90a43-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90a43-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90a43-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90a43-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90a43-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="90a43-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90a43-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90a43-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90a43-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="90a43-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90a43-114">Application</span></span> | <span data-ttu-id="90a43-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90a43-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90a43-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90a43-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/UsedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="90a43-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90a43-117">Request headers</span></span>
| <span data-ttu-id="90a43-118">Nome</span><span class="sxs-lookup"><span data-stu-id="90a43-118">Name</span></span>       | <span data-ttu-id="90a43-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="90a43-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="90a43-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="90a43-120">Authorization</span></span>  | <span data-ttu-id="90a43-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90a43-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="90a43-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="90a43-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="90a43-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="90a43-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="90a43-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90a43-126">Request body</span></span>
<span data-ttu-id="90a43-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90a43-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="90a43-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="90a43-128">Parameter</span></span>    | <span data-ttu-id="90a43-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="90a43-129">Type</span></span>   |<span data-ttu-id="90a43-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="90a43-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90a43-131">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="90a43-131">valuesOnly</span></span>|<span data-ttu-id="90a43-132">booliano</span><span class="sxs-lookup"><span data-stu-id="90a43-132">boolean</span></span>|<span data-ttu-id="90a43-p104">Opcional. Considera apenas as células com valores como células usadas.</span><span class="sxs-lookup"><span data-stu-id="90a43-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="90a43-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="90a43-135">Response</span></span>

<span data-ttu-id="90a43-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90a43-136">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90a43-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90a43-137">Example</span></span>
<span data-ttu-id="90a43-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="90a43-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="90a43-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90a43-139">Request</span></span>
<span data-ttu-id="90a43-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90a43-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="90a43-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="90a43-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/UsedRange
Content-type: application/json
Content-length: 24

{
  "valuesOnly": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="90a43-142">C#</span><span class="sxs-lookup"><span data-stu-id="90a43-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90a43-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90a43-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="90a43-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="90a43-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="90a43-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="90a43-145">Response</span></span>
<span data-ttu-id="90a43-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90a43-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
