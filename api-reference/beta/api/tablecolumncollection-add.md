---
title: 'TableColumnCollection: add'
description: Adiciona uma nova coluna à tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 656340fafa39b074f7a1438b2ed9902b4e975ee4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052674"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="0a876-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="0a876-103">TableColumnCollection: add</span></span>

<span data-ttu-id="0a876-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a876-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a876-105">Adiciona uma nova coluna à tabela.</span><span class="sxs-lookup"><span data-stu-id="0a876-105">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="0a876-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0a876-106">Permissions</span></span>
<span data-ttu-id="0a876-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a876-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a876-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a876-109">Permission type</span></span>      | <span data-ttu-id="0a876-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a876-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a876-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a876-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0a876-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a876-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0a876-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a876-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a876-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a876-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0a876-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a876-115">Application</span></span> | <span data-ttu-id="0a876-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a876-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a876-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a876-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/add
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="0a876-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a876-118">Request headers</span></span>
| <span data-ttu-id="0a876-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0a876-119">Name</span></span>       | <span data-ttu-id="0a876-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a876-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0a876-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a876-121">Authorization</span></span>  | <span data-ttu-id="0a876-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a876-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0a876-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0a876-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0a876-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0a876-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a876-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a876-127">Request body</span></span>
<span data-ttu-id="0a876-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a876-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0a876-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0a876-129">Parameter</span></span>    | <span data-ttu-id="0a876-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a876-130">Type</span></span>   |<span data-ttu-id="0a876-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a876-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a876-132">index</span><span class="sxs-lookup"><span data-stu-id="0a876-132">index</span></span>|<span data-ttu-id="0a876-133">number</span><span class="sxs-lookup"><span data-stu-id="0a876-133">number</span></span>|<span data-ttu-id="0a876-p104">Especifica a posição relativa da nova coluna. A coluna anterior nessa posição é deslocada para a direita. O valor do índice deve ser igual ou menor que o valor do índice da última coluna, portanto não pode ser usado para acrescentar uma coluna ao final da tabela. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="0a876-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="0a876-138">values</span><span class="sxs-lookup"><span data-stu-id="0a876-138">values</span></span>|<span data-ttu-id="0a876-139">(booleano ou cadeia de caracteres ou número) coleção</span><span class="sxs-lookup"><span data-stu-id="0a876-139">(boolean or string or number) collection</span></span>|<span data-ttu-id="0a876-p105">Opcional. Uma matriz bidimensional de valores não formatados da coluna da tabela.</span><span class="sxs-lookup"><span data-stu-id="0a876-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="0a876-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a876-142">Response</span></span>

<span data-ttu-id="0a876-143">Se tiver êxito, este método retornará o código de resposta e o objeto `200 OK` [workbookTableColumn](../resources/workbooktablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a876-143">If successful, this method returns `200 OK` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a876-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a876-144">Example</span></span>
<span data-ttu-id="0a876-145">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0a876-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0a876-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a876-146">Request</span></span>
<span data-ttu-id="0a876-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a876-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0a876-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a876-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": {
  },
  "values": [
    {
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="0a876-149">C#</span><span class="sxs-lookup"><span data-stu-id="0a876-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumncollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a876-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a876-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a876-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a876-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a876-152">Java</span><span class="sxs-lookup"><span data-stu-id="0a876-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumncollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0a876-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a876-153">Response</span></span>
<span data-ttu-id="0a876-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a876-154">Here is an example of the response.</span></span> <span data-ttu-id="0a876-155">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0a876-155">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


