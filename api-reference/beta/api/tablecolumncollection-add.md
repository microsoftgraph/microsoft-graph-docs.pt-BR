---
title: 'TableColumnCollection: add'
description: Adiciona uma nova coluna à tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e168eb6e81234e9e12dc70b8896d3bbd9aecbb60
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363043"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="33de0-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="33de0-103">TableColumnCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33de0-104">Adiciona uma nova coluna à tabela.</span><span class="sxs-lookup"><span data-stu-id="33de0-104">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="33de0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="33de0-105">Permissions</span></span>
<span data-ttu-id="33de0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33de0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33de0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33de0-108">Permission type</span></span>      | <span data-ttu-id="33de0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33de0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33de0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33de0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="33de0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33de0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="33de0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33de0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33de0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33de0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="33de0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33de0-114">Application</span></span> | <span data-ttu-id="33de0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33de0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="33de0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33de0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="33de0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33de0-117">Request headers</span></span>
| <span data-ttu-id="33de0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="33de0-118">Name</span></span>       | <span data-ttu-id="33de0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="33de0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="33de0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="33de0-120">Authorization</span></span>  | <span data-ttu-id="33de0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33de0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="33de0-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="33de0-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="33de0-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="33de0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="33de0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33de0-126">Request body</span></span>
<span data-ttu-id="33de0-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33de0-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="33de0-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="33de0-128">Parameter</span></span>    | <span data-ttu-id="33de0-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="33de0-129">Type</span></span>   |<span data-ttu-id="33de0-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="33de0-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33de0-131">index</span><span class="sxs-lookup"><span data-stu-id="33de0-131">index</span></span>|<span data-ttu-id="33de0-132">number</span><span class="sxs-lookup"><span data-stu-id="33de0-132">number</span></span>|<span data-ttu-id="33de0-p104">Especifica a posição relativa da nova coluna. A coluna anterior nessa posição é deslocada para a direita. O valor do índice deve ser igual ou menor que o valor do índice da última coluna, portanto não pode ser usado para acrescentar uma coluna ao final da tabela. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="33de0-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="33de0-137">values</span><span class="sxs-lookup"><span data-stu-id="33de0-137">values</span></span>|<span data-ttu-id="33de0-138">coleção (booliano ou cadeia de caracteres ou número)</span><span class="sxs-lookup"><span data-stu-id="33de0-138">(boolean or string or number) collection</span></span>|<span data-ttu-id="33de0-p105">Opcional. Uma matriz bidimensional de valores não formatados da coluna da tabela.</span><span class="sxs-lookup"><span data-stu-id="33de0-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="33de0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="33de0-141">Response</span></span>

<span data-ttu-id="33de0-142">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [workbookTableColumn](../resources/workbooktablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33de0-142">If successful, this method returns `200 OK` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33de0-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33de0-143">Example</span></span>
<span data-ttu-id="33de0-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="33de0-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="33de0-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33de0-145">Request</span></span>
<span data-ttu-id="33de0-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33de0-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="33de0-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="33de0-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="33de0-148">C#</span><span class="sxs-lookup"><span data-stu-id="33de0-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumncollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="33de0-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33de0-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="33de0-150">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="33de0-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="33de0-151">Java</span><span class="sxs-lookup"><span data-stu-id="33de0-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumncollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="33de0-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="33de0-152">Response</span></span>
<span data-ttu-id="33de0-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33de0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": 99,
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
