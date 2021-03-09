---
title: 'Range: insert'
description: Insere uma célula ou um intervalo de células na planilha, no lugar desse intervalo, e desloca as outras células para liberar espaço. Retorna um novo objeto Range no espaço em branco atual.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2f5f9d3952afed0cad6430d1ae35078906f6b00f
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578679"
---
# <a name="range-insert"></a><span data-ttu-id="96bc2-104">Range: insert</span><span class="sxs-lookup"><span data-stu-id="96bc2-104">Range: insert</span></span>

<span data-ttu-id="96bc2-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96bc2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96bc2-p102">Insere uma célula ou um intervalo de células na planilha, no lugar desse intervalo, e desloca as outras células para liberar espaço. Retorna um novo objeto Range no espaço em branco atual.</span><span class="sxs-lookup"><span data-stu-id="96bc2-p102">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="96bc2-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="96bc2-108">Permissions</span></span>
<span data-ttu-id="96bc2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96bc2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96bc2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96bc2-111">Permission type</span></span>      | <span data-ttu-id="96bc2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96bc2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96bc2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96bc2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="96bc2-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96bc2-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="96bc2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96bc2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96bc2-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96bc2-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="96bc2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96bc2-117">Application</span></span> | <span data-ttu-id="96bc2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96bc2-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96bc2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96bc2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/insert
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/insert
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/insert
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="96bc2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96bc2-120">Request headers</span></span>
| <span data-ttu-id="96bc2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="96bc2-121">Name</span></span>       | <span data-ttu-id="96bc2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="96bc2-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="96bc2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="96bc2-123">Authorization</span></span>  | <span data-ttu-id="96bc2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96bc2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96bc2-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="96bc2-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="96bc2-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="96bc2-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96bc2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96bc2-129">Request body</span></span>
<span data-ttu-id="96bc2-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96bc2-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="96bc2-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="96bc2-131">Parameter</span></span>    | <span data-ttu-id="96bc2-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="96bc2-132">Type</span></span>   |<span data-ttu-id="96bc2-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="96bc2-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96bc2-134">shift</span><span class="sxs-lookup"><span data-stu-id="96bc2-134">shift</span></span>|<span data-ttu-id="96bc2-135">string</span><span class="sxs-lookup"><span data-stu-id="96bc2-135">string</span></span>|<span data-ttu-id="96bc2-p106">Especifica como deslocar as células.  Os valores possíveis são: `Down` e `Right`.</span><span class="sxs-lookup"><span data-stu-id="96bc2-p106">Specifies which way to shift the cells.  Possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="96bc2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="96bc2-138">Response</span></span>

<span data-ttu-id="96bc2-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96bc2-139">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96bc2-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96bc2-140">Example</span></span>
<span data-ttu-id="96bc2-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="96bc2-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="96bc2-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96bc2-142">Request</span></span>
<span data-ttu-id="96bc2-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96bc2-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="96bc2-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="96bc2-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```
# <a name="c"></a>[<span data-ttu-id="96bc2-145">C#</span><span class="sxs-lookup"><span data-stu-id="96bc2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-insert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96bc2-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96bc2-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-insert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96bc2-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96bc2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-insert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96bc2-148">Java</span><span class="sxs-lookup"><span data-stu-id="96bc2-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-insert-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="96bc2-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="96bc2-149">Response</span></span>
<span data-ttu-id="96bc2-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96bc2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


