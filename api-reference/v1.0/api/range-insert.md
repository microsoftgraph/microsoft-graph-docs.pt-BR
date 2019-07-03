---
title: 'Range: insert'
description: Insere uma célula ou um intervalo de células na planilha, no lugar desse intervalo, e desloca as outras células para liberar espaço. Retorna um novo objeto Range no espaço em branco atual.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 2ea7252994775558976501c0b263f7df0c85c8e4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449558"
---
# <a name="range-insert"></a><span data-ttu-id="90153-104">Range: insert</span><span class="sxs-lookup"><span data-stu-id="90153-104">Range: insert</span></span>

<span data-ttu-id="90153-p102">Insere uma célula ou um intervalo de células na planilha, no lugar desse intervalo, e desloca as outras células para liberar espaço. Retorna um novo objeto Range no espaço em branco atual.</span><span class="sxs-lookup"><span data-stu-id="90153-p102">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="90153-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="90153-107">Permissions</span></span>
<span data-ttu-id="90153-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90153-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90153-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90153-110">Permission type</span></span>      | <span data-ttu-id="90153-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90153-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90153-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90153-112">Delegated (work or school account)</span></span> | <span data-ttu-id="90153-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90153-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="90153-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90153-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90153-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90153-115">Not supported.</span></span>    |
|<span data-ttu-id="90153-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90153-116">Application</span></span> | <span data-ttu-id="90153-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90153-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90153-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90153-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/insert
POST /workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="90153-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90153-119">Request headers</span></span>
| <span data-ttu-id="90153-120">Nome</span><span class="sxs-lookup"><span data-stu-id="90153-120">Name</span></span>       | <span data-ttu-id="90153-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="90153-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="90153-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="90153-122">Authorization</span></span>  | <span data-ttu-id="90153-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90153-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="90153-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="90153-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="90153-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="90153-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="90153-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90153-128">Request body</span></span>
<span data-ttu-id="90153-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90153-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="90153-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="90153-130">Parameter</span></span>    | <span data-ttu-id="90153-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="90153-131">Type</span></span>   |<span data-ttu-id="90153-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="90153-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90153-133">shift</span><span class="sxs-lookup"><span data-stu-id="90153-133">shift</span></span>|<span data-ttu-id="90153-134">string</span><span class="sxs-lookup"><span data-stu-id="90153-134">string</span></span>|<span data-ttu-id="90153-135">Especifica como deslocar as células.</span><span class="sxs-lookup"><span data-stu-id="90153-135">Specifies which way to shift the cells.</span></span>  <span data-ttu-id="90153-136">Os valores possíveis são: `Down`, `Right`.</span><span class="sxs-lookup"><span data-stu-id="90153-136">The possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="90153-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="90153-137">Response</span></span>

<span data-ttu-id="90153-138">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90153-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90153-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90153-139">Example</span></span>
<span data-ttu-id="90153-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="90153-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="90153-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90153-141">Request</span></span>
<span data-ttu-id="90153-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90153-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="90153-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="90153-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="90153-144">C#</span><span class="sxs-lookup"><span data-stu-id="90153-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-insert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90153-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="90153-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-insert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="90153-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="90153-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-insert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="90153-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="90153-147">Response</span></span>
<span data-ttu-id="90153-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90153-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
