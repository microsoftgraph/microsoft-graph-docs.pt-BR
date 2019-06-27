---
title: 'TableColumnCollection: add'
description: Adiciona uma nova coluna à tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6df308e7076ffce00dcaa7401ea6a921334d62b0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270893"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="52c8f-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="52c8f-103">TableColumnCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52c8f-104">Adiciona uma nova coluna à tabela.</span><span class="sxs-lookup"><span data-stu-id="52c8f-104">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="52c8f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="52c8f-105">Permissions</span></span>
<span data-ttu-id="52c8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52c8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52c8f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52c8f-108">Permission type</span></span>      | <span data-ttu-id="52c8f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52c8f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52c8f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52c8f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="52c8f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52c8f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="52c8f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52c8f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52c8f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52c8f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="52c8f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52c8f-114">Application</span></span> | <span data-ttu-id="52c8f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52c8f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52c8f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52c8f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="52c8f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52c8f-117">Request headers</span></span>
| <span data-ttu-id="52c8f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="52c8f-118">Name</span></span>       | <span data-ttu-id="52c8f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="52c8f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="52c8f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="52c8f-120">Authorization</span></span>  | <span data-ttu-id="52c8f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52c8f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52c8f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="52c8f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="52c8f-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="52c8f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52c8f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52c8f-126">Request body</span></span>
<span data-ttu-id="52c8f-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52c8f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="52c8f-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="52c8f-128">Parameter</span></span>    | <span data-ttu-id="52c8f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="52c8f-129">Type</span></span>   |<span data-ttu-id="52c8f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="52c8f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52c8f-131">index</span><span class="sxs-lookup"><span data-stu-id="52c8f-131">index</span></span>|<span data-ttu-id="52c8f-132">number</span><span class="sxs-lookup"><span data-stu-id="52c8f-132">number</span></span>|<span data-ttu-id="52c8f-p104">Especifica a posição relativa da nova coluna. A coluna anterior nessa posição é deslocada para a direita. O valor do índice deve ser igual ou menor que o valor do índice da última coluna, portanto não pode ser usado para acrescentar uma coluna ao final da tabela. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="52c8f-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="52c8f-137">values</span><span class="sxs-lookup"><span data-stu-id="52c8f-137">values</span></span>|<span data-ttu-id="52c8f-138">coleção (booliano ou cadeia de caracteres ou número)</span><span class="sxs-lookup"><span data-stu-id="52c8f-138">(boolean or string or number) collection</span></span>|<span data-ttu-id="52c8f-p105">Opcional. Uma matriz bidimensional de valores não formatados da coluna da tabela.</span><span class="sxs-lookup"><span data-stu-id="52c8f-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="52c8f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="52c8f-141">Response</span></span>

<span data-ttu-id="52c8f-142">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [workbookTableColumn](../resources/workbooktablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52c8f-142">If successful, this method returns `200 OK` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52c8f-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52c8f-143">Example</span></span>
<span data-ttu-id="52c8f-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="52c8f-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="52c8f-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52c8f-145">Request</span></span>
<span data-ttu-id="52c8f-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52c8f-146">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="52c8f-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="52c8f-147">Response</span></span>
<span data-ttu-id="52c8f-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52c8f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="52c8f-151">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="52c8f-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="52c8f-152">C#</span><span class="sxs-lookup"><span data-stu-id="52c8f-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablecolumncollection_add-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52c8f-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="52c8f-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablecolumncollection_add-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="52c8f-154">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="52c8f-154">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/tablecolumncollection_add-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/tablecolumncollection-add.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tablecolumncollection-add.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tablecolumncollection-add.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
