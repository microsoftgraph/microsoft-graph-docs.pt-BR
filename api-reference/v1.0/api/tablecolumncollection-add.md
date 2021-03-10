---
title: 'TableColumnCollection: add'
description: Adiciona uma nova coluna à tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 09312b06c0ba3be49e5f26b1346345017cd05095
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575887"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="0f4be-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="0f4be-103">TableColumnCollection: add</span></span>

<span data-ttu-id="0f4be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f4be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f4be-105">Adiciona uma nova coluna à tabela.</span><span class="sxs-lookup"><span data-stu-id="0f4be-105">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="0f4be-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f4be-106">Permissions</span></span>
<span data-ttu-id="0f4be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f4be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f4be-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f4be-109">Permission type</span></span>      | <span data-ttu-id="0f4be-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f4be-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f4be-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f4be-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0f4be-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f4be-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0f4be-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f4be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f4be-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f4be-114">Not supported.</span></span>    |
|<span data-ttu-id="0f4be-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f4be-115">Application</span></span> | <span data-ttu-id="0f4be-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f4be-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f4be-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f4be-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/add
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="0f4be-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f4be-118">Request headers</span></span>
| <span data-ttu-id="0f4be-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0f4be-119">Name</span></span>       | <span data-ttu-id="0f4be-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f4be-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0f4be-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f4be-121">Authorization</span></span>  | <span data-ttu-id="0f4be-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f4be-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0f4be-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0f4be-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0f4be-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0f4be-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f4be-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f4be-127">Request body</span></span>
<span data-ttu-id="0f4be-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f4be-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0f4be-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0f4be-129">Parameter</span></span>    | <span data-ttu-id="0f4be-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f4be-130">Type</span></span>   |<span data-ttu-id="0f4be-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f4be-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f4be-132">índice</span><span class="sxs-lookup"><span data-stu-id="0f4be-132">index</span></span>|<span data-ttu-id="0f4be-133">Int32</span><span class="sxs-lookup"><span data-stu-id="0f4be-133">Int32</span></span>|<span data-ttu-id="0f4be-p104">Especifica a posição relativa da nova coluna. A coluna anterior nessa posição é deslocada para a direita. O valor do índice deve ser igual ou menor que o valor do índice da última coluna, portanto não pode ser usado para acrescentar uma coluna ao final da tabela. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="0f4be-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="0f4be-138">values</span><span class="sxs-lookup"><span data-stu-id="0f4be-138">values</span></span>|<span data-ttu-id="0f4be-139">Json</span><span class="sxs-lookup"><span data-stu-id="0f4be-139">Json</span></span>|<span data-ttu-id="0f4be-p105">Opcional. Uma matriz bidimensional de valores não formatados da coluna da tabela.</span><span class="sxs-lookup"><span data-stu-id="0f4be-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|
|<span data-ttu-id="0f4be-142">nome</span><span class="sxs-lookup"><span data-stu-id="0f4be-142">name</span></span>|<span data-ttu-id="0f4be-143">string</span><span class="sxs-lookup"><span data-stu-id="0f4be-143">string</span></span>|<span data-ttu-id="0f4be-144">nome</span><span class="sxs-lookup"><span data-stu-id="0f4be-144">name</span></span>
## <a name="response"></a><span data-ttu-id="0f4be-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f4be-145">Response</span></span>

<span data-ttu-id="0f4be-146">Se tiver êxito, este método retornará o código de resposta e o `200 OK` [objeto WorkbookTableColumn](../resources/workbooktablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f4be-146">If successful, this method returns `200 OK` response code and [WorkbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f4be-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f4be-147">Example</span></span>
<span data-ttu-id="0f4be-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0f4be-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0f4be-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f4be-149">Request</span></span>
<span data-ttu-id="0f4be-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f4be-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0f4be-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f4be-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0f4be-152">C#</span><span class="sxs-lookup"><span data-stu-id="0f4be-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumncollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0f4be-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f4be-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f4be-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f4be-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0f4be-155">Java</span><span class="sxs-lookup"><span data-stu-id="0f4be-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumncollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0f4be-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f4be-156">Response</span></span>
<span data-ttu-id="0f4be-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f4be-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

