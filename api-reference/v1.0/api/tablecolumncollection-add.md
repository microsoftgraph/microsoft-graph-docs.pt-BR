---
title: 'TableColumnCollection: add'
description: Adiciona uma nova coluna à tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f5def48977bafef35efc23972211e91022e1d97f
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034216"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="37460-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="37460-103">TableColumnCollection: add</span></span>

<span data-ttu-id="37460-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37460-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37460-105">Adiciona uma nova coluna à tabela.</span><span class="sxs-lookup"><span data-stu-id="37460-105">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="37460-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37460-106">Permissions</span></span>
<span data-ttu-id="37460-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37460-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37460-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37460-109">Permission type</span></span>      | <span data-ttu-id="37460-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37460-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37460-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37460-111">Delegated (work or school account)</span></span> | <span data-ttu-id="37460-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37460-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="37460-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37460-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37460-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37460-114">Not supported.</span></span>    |
|<span data-ttu-id="37460-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37460-115">Application</span></span> | <span data-ttu-id="37460-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37460-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="37460-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37460-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="37460-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37460-118">Request headers</span></span>
| <span data-ttu-id="37460-119">Nome</span><span class="sxs-lookup"><span data-stu-id="37460-119">Name</span></span>       | <span data-ttu-id="37460-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="37460-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="37460-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="37460-121">Authorization</span></span>  | <span data-ttu-id="37460-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37460-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="37460-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="37460-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="37460-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="37460-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37460-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37460-127">Request body</span></span>
<span data-ttu-id="37460-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37460-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="37460-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="37460-129">Parameter</span></span>    | <span data-ttu-id="37460-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="37460-130">Type</span></span>   |<span data-ttu-id="37460-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="37460-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37460-132">índice</span><span class="sxs-lookup"><span data-stu-id="37460-132">index</span></span>|<span data-ttu-id="37460-133">Int32</span><span class="sxs-lookup"><span data-stu-id="37460-133">Int32</span></span>|<span data-ttu-id="37460-p104">Especifica a posição relativa da nova coluna. A coluna anterior nessa posição é deslocada para a direita. O valor do índice deve ser igual ou menor que o valor do índice da última coluna, portanto não pode ser usado para acrescentar uma coluna ao final da tabela. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="37460-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="37460-138">values</span><span class="sxs-lookup"><span data-stu-id="37460-138">values</span></span>|<span data-ttu-id="37460-139">Json</span><span class="sxs-lookup"><span data-stu-id="37460-139">Json</span></span>|<span data-ttu-id="37460-p105">Opcional. Uma matriz bidimensional de valores não formatados da coluna da tabela.</span><span class="sxs-lookup"><span data-stu-id="37460-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|
|<span data-ttu-id="37460-142">nome</span><span class="sxs-lookup"><span data-stu-id="37460-142">name</span></span>|<span data-ttu-id="37460-143">string</span><span class="sxs-lookup"><span data-stu-id="37460-143">string</span></span>|<span data-ttu-id="37460-144">nome</span><span class="sxs-lookup"><span data-stu-id="37460-144">name</span></span>
## <a name="response"></a><span data-ttu-id="37460-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="37460-145">Response</span></span>

<span data-ttu-id="37460-146">Se bem-sucedido, este método retorna o código de resposta e o `200 OK` [objeto WorkbookTableColumn](../resources/workbooktablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37460-146">If successful, this method returns `200 OK` response code and [WorkbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37460-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37460-147">Example</span></span>
<span data-ttu-id="37460-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="37460-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="37460-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37460-149">Request</span></span>
<span data-ttu-id="37460-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37460-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37460-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="37460-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="37460-152">C#</span><span class="sxs-lookup"><span data-stu-id="37460-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumncollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37460-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37460-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37460-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37460-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37460-155">Java</span><span class="sxs-lookup"><span data-stu-id="37460-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumncollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="37460-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="37460-156">Response</span></span>
<span data-ttu-id="37460-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37460-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

