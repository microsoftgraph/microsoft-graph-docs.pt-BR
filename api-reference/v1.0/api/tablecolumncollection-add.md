---
title: 'TableColumnCollection: add'
description: Adiciona uma nova coluna à tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c05316721be4e03ef83c9f36f8eeee0e6f2a62fb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52034403"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="96d56-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="96d56-103">TableColumnCollection: add</span></span>

<span data-ttu-id="96d56-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96d56-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="96d56-105">Adiciona uma nova coluna à tabela.</span><span class="sxs-lookup"><span data-stu-id="96d56-105">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="96d56-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="96d56-106">Permissions</span></span>
<span data-ttu-id="96d56-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96d56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96d56-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96d56-109">Permission type</span></span>      | <span data-ttu-id="96d56-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96d56-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96d56-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96d56-111">Delegated (work or school account)</span></span> | <span data-ttu-id="96d56-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96d56-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="96d56-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96d56-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96d56-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96d56-114">Not supported.</span></span>    |
|<span data-ttu-id="96d56-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96d56-115">Application</span></span> | <span data-ttu-id="96d56-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96d56-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96d56-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96d56-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/add
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="96d56-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96d56-118">Request headers</span></span>
| <span data-ttu-id="96d56-119">Nome</span><span class="sxs-lookup"><span data-stu-id="96d56-119">Name</span></span>       | <span data-ttu-id="96d56-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="96d56-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="96d56-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="96d56-121">Authorization</span></span>  | <span data-ttu-id="96d56-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96d56-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96d56-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="96d56-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="96d56-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="96d56-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96d56-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96d56-127">Request body</span></span>
<span data-ttu-id="96d56-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96d56-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="96d56-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="96d56-129">Parameter</span></span>    | <span data-ttu-id="96d56-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="96d56-130">Type</span></span>   |<span data-ttu-id="96d56-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="96d56-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96d56-132">índice</span><span class="sxs-lookup"><span data-stu-id="96d56-132">index</span></span>|<span data-ttu-id="96d56-133">Int32</span><span class="sxs-lookup"><span data-stu-id="96d56-133">Int32</span></span>|<span data-ttu-id="96d56-p104">Especifica a posição relativa da nova coluna. A coluna anterior nessa posição é deslocada para a direita. O valor do índice deve ser igual ou menor que o valor do índice da última coluna, portanto não pode ser usado para acrescentar uma coluna ao final da tabela. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="96d56-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="96d56-138">values</span><span class="sxs-lookup"><span data-stu-id="96d56-138">values</span></span>|<span data-ttu-id="96d56-139">Json</span><span class="sxs-lookup"><span data-stu-id="96d56-139">Json</span></span>|<span data-ttu-id="96d56-p105">Opcional. Uma matriz bidimensional de valores não formatados da coluna da tabela.</span><span class="sxs-lookup"><span data-stu-id="96d56-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|
|<span data-ttu-id="96d56-142">nome</span><span class="sxs-lookup"><span data-stu-id="96d56-142">name</span></span>|<span data-ttu-id="96d56-143">string</span><span class="sxs-lookup"><span data-stu-id="96d56-143">string</span></span>|<span data-ttu-id="96d56-144">nome</span><span class="sxs-lookup"><span data-stu-id="96d56-144">name</span></span>
## <a name="response"></a><span data-ttu-id="96d56-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="96d56-145">Response</span></span>

<span data-ttu-id="96d56-146">Se tiver êxito, este método retornará o código de resposta e o `200 OK` [objeto WorkbookTableColumn](../resources/workbooktablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96d56-146">If successful, this method returns `200 OK` response code and [WorkbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96d56-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96d56-147">Example</span></span>
<span data-ttu-id="96d56-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="96d56-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="96d56-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96d56-149">Request</span></span>
<span data-ttu-id="96d56-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96d56-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="96d56-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="96d56-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": 3,
  "values": [
    {
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="96d56-152">C#</span><span class="sxs-lookup"><span data-stu-id="96d56-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumncollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96d56-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96d56-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96d56-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96d56-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96d56-155">Java</span><span class="sxs-lookup"><span data-stu-id="96d56-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumncollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="96d56-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="96d56-156">Response</span></span>
<span data-ttu-id="96d56-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96d56-157">Here is an example of the response.</span></span> <span data-ttu-id="96d56-158">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="96d56-158">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": "99",
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/tablecolumncollection-add.md/tablecolumncollection_add/values:
      Inconsistent types between parameter (Object) and table (None)",
    "Error: /api-reference/v1.0/api/tablecolumncollection-add.md/tablecolumncollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Object)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->

