---
title: 'Range: insert'
description: Insere uma célula ou um intervalo de células na planilha, no lugar desse intervalo, e desloca as outras células para liberar espaço. Retorna um novo objeto Range no espaço em branco atual.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f8cba57e4163377c3542e7416b1926ec675ee8dd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048656"
---
# <a name="range-insert"></a><span data-ttu-id="1866b-104">Range: insert</span><span class="sxs-lookup"><span data-stu-id="1866b-104">Range: insert</span></span>

<span data-ttu-id="1866b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1866b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1866b-p102">Insere uma célula ou um intervalo de células na planilha, no lugar desse intervalo, e desloca as outras células para liberar espaço. Retorna um novo objeto Range no espaço em branco atual.</span><span class="sxs-lookup"><span data-stu-id="1866b-p102">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="1866b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1866b-108">Permissions</span></span>
<span data-ttu-id="1866b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1866b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1866b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1866b-111">Permission type</span></span>      | <span data-ttu-id="1866b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1866b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1866b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1866b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1866b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1866b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1866b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1866b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1866b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1866b-116">Not supported.</span></span>    |
|<span data-ttu-id="1866b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1866b-117">Application</span></span> | <span data-ttu-id="1866b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1866b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1866b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1866b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/insert
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/insert
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/insert
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="1866b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1866b-120">Request headers</span></span>
| <span data-ttu-id="1866b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1866b-121">Name</span></span>       | <span data-ttu-id="1866b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1866b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1866b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1866b-123">Authorization</span></span>  | <span data-ttu-id="1866b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1866b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1866b-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1866b-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="1866b-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1866b-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1866b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1866b-129">Request body</span></span>
<span data-ttu-id="1866b-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1866b-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1866b-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1866b-131">Parameter</span></span>    | <span data-ttu-id="1866b-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1866b-132">Type</span></span>   |<span data-ttu-id="1866b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1866b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1866b-134">shift</span><span class="sxs-lookup"><span data-stu-id="1866b-134">shift</span></span>|<span data-ttu-id="1866b-135">string</span><span class="sxs-lookup"><span data-stu-id="1866b-135">string</span></span>|<span data-ttu-id="1866b-136">Especifica como deslocar as células.</span><span class="sxs-lookup"><span data-stu-id="1866b-136">Specifies which way to shift the cells.</span></span>  <span data-ttu-id="1866b-137">Os valores possíveis são: `Down` , `Right` .</span><span class="sxs-lookup"><span data-stu-id="1866b-137">The possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="1866b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1866b-138">Response</span></span>

<span data-ttu-id="1866b-139">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1866b-139">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1866b-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1866b-140">Example</span></span>
<span data-ttu-id="1866b-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1866b-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1866b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1866b-142">Request</span></span>
<span data-ttu-id="1866b-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1866b-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1866b-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="1866b-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1866b-145">C#</span><span class="sxs-lookup"><span data-stu-id="1866b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-insert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1866b-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1866b-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-insert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1866b-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1866b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-insert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1866b-148">Java</span><span class="sxs-lookup"><span data-stu-id="1866b-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-insert-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1866b-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1866b-149">Response</span></span>
<span data-ttu-id="1866b-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1866b-150">Here is an example of the response.</span></span> <span data-ttu-id="1866b-151">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1866b-151">Note: The response object shown here might be shortened for readability.</span></span>
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

