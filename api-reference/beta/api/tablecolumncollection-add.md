---
title: 'TableColumnCollection: add'
description: Adiciona uma nova coluna à tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f93c113135d21b8e705e181c954855d6b9828ca8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452705"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="42959-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="42959-103">TableColumnCollection: add</span></span>

<span data-ttu-id="42959-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="42959-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42959-105">Adiciona uma nova coluna à tabela.</span><span class="sxs-lookup"><span data-stu-id="42959-105">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="42959-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="42959-106">Permissions</span></span>
<span data-ttu-id="42959-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42959-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42959-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42959-109">Permission type</span></span>      | <span data-ttu-id="42959-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42959-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42959-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42959-111">Delegated (work or school account)</span></span> | <span data-ttu-id="42959-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42959-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="42959-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42959-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42959-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42959-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="42959-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42959-115">Application</span></span> | <span data-ttu-id="42959-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42959-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42959-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42959-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="42959-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42959-118">Request headers</span></span>
| <span data-ttu-id="42959-119">Nome</span><span class="sxs-lookup"><span data-stu-id="42959-119">Name</span></span>       | <span data-ttu-id="42959-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="42959-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="42959-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="42959-121">Authorization</span></span>  | <span data-ttu-id="42959-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42959-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="42959-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="42959-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="42959-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="42959-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="42959-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42959-127">Request body</span></span>
<span data-ttu-id="42959-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42959-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="42959-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="42959-129">Parameter</span></span>    | <span data-ttu-id="42959-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="42959-130">Type</span></span>   |<span data-ttu-id="42959-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="42959-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42959-132">index</span><span class="sxs-lookup"><span data-stu-id="42959-132">index</span></span>|<span data-ttu-id="42959-133">number</span><span class="sxs-lookup"><span data-stu-id="42959-133">number</span></span>|<span data-ttu-id="42959-p104">Especifica a posição relativa da nova coluna. A coluna anterior nessa posição é deslocada para a direita. O valor do índice deve ser igual ou menor que o valor do índice da última coluna, portanto não pode ser usado para acrescentar uma coluna ao final da tabela. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="42959-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="42959-138">values</span><span class="sxs-lookup"><span data-stu-id="42959-138">values</span></span>|<span data-ttu-id="42959-139">coleção (booliano ou cadeia de caracteres ou número)</span><span class="sxs-lookup"><span data-stu-id="42959-139">(boolean or string or number) collection</span></span>|<span data-ttu-id="42959-p105">Opcional. Uma matriz bidimensional de valores não formatados da coluna da tabela.</span><span class="sxs-lookup"><span data-stu-id="42959-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="42959-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="42959-142">Response</span></span>

<span data-ttu-id="42959-143">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [workbookTableColumn](../resources/workbooktablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42959-143">If successful, this method returns `200 OK` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42959-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42959-144">Example</span></span>
<span data-ttu-id="42959-145">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="42959-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="42959-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42959-146">Request</span></span>
<span data-ttu-id="42959-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42959-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42959-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="42959-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="42959-149">C#</span><span class="sxs-lookup"><span data-stu-id="42959-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumncollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42959-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42959-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42959-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42959-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="42959-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="42959-152">Response</span></span>
<span data-ttu-id="42959-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42959-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
