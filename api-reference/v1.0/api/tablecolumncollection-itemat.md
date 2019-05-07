---
title: 'TableColumnCollection: ItemAt'
description: Obtém uma coluna com base em sua posição na coleção.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 01878a2ecf663231701289f5a734dac0407dd54b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33602546"
---
# <a name="tablecolumncollection-itemat"></a><span data-ttu-id="c1962-103">TableColumnCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="c1962-103">TableColumnCollection: ItemAt</span></span>

<span data-ttu-id="c1962-104">Obtém uma coluna com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="c1962-104">Gets a column based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="c1962-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c1962-105">Permissions</span></span>
<span data-ttu-id="c1962-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1962-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1962-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1962-108">Permission type</span></span>      | <span data-ttu-id="c1962-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c1962-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1962-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1962-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c1962-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1962-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c1962-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1962-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1962-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1962-113">Not supported.</span></span>    |
|<span data-ttu-id="c1962-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1962-114">Application</span></span> | <span data-ttu-id="c1962-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1962-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1962-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1962-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/itemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="c1962-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1962-117">Request headers</span></span>
| <span data-ttu-id="c1962-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c1962-118">Name</span></span>       | <span data-ttu-id="c1962-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1962-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c1962-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1962-120">Authorization</span></span>  | <span data-ttu-id="c1962-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1962-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1962-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c1962-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c1962-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c1962-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1962-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1962-126">Request body</span></span>
<span data-ttu-id="c1962-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1962-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c1962-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c1962-128">Parameter</span></span>    | <span data-ttu-id="c1962-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1962-129">Type</span></span>   |<span data-ttu-id="c1962-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1962-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1962-131">índice</span><span class="sxs-lookup"><span data-stu-id="c1962-131">index</span></span>|<span data-ttu-id="c1962-132">Int32</span><span class="sxs-lookup"><span data-stu-id="c1962-132">Int32</span></span>|<span data-ttu-id="c1962-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="c1962-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="c1962-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1962-135">Response</span></span>

<span data-ttu-id="c1962-136">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [WorkbookTableColumn](../resources/tablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1962-136">If successful, this method returns `200 OK` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1962-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1962-137">Example</span></span>
<span data-ttu-id="c1962-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c1962-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c1962-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1962-139">Request</span></span>
<span data-ttu-id="c1962-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1962-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumncollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.tablecolumncollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 3
}
```

##### <a name="response"></a><span data-ttu-id="c1962-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1962-141">Response</span></span>
<span data-ttu-id="c1962-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1962-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c1962-145">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c1962-145">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1962-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1962-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablecolumncollection_itemat-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/tablecolumncollection-itemat.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
