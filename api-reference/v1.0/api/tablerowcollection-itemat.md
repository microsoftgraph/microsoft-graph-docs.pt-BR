---
title: 'TableRowCollection: ItemAt'
description: Obtém uma linha com base em sua posição na coleção.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ecded1222bd50731989aa486dad14367f1c6d3ce
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456061"
---
# <a name="tablerowcollection-itemat"></a><span data-ttu-id="0997b-103">TableRowCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="0997b-103">TableRowCollection: ItemAt</span></span>

<span data-ttu-id="0997b-104">Obtém uma linha com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="0997b-104">Gets a row based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="0997b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0997b-105">Permissions</span></span>
<span data-ttu-id="0997b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0997b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0997b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0997b-108">Permission type</span></span>      | <span data-ttu-id="0997b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0997b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0997b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0997b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0997b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0997b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0997b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0997b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0997b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0997b-113">Not supported.</span></span>    |
|<span data-ttu-id="0997b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0997b-114">Application</span></span> | <span data-ttu-id="0997b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0997b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0997b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0997b-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0997b-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="0997b-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/itemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="0997b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0997b-118">Request headers</span></span>
| <span data-ttu-id="0997b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0997b-119">Name</span></span>       | <span data-ttu-id="0997b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0997b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0997b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0997b-121">Authorization</span></span>  | <span data-ttu-id="0997b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0997b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0997b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0997b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0997b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0997b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0997b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0997b-127">Request body</span></span>
<span data-ttu-id="0997b-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0997b-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0997b-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0997b-129">Parameter</span></span>    | <span data-ttu-id="0997b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0997b-130">Type</span></span>   |<span data-ttu-id="0997b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0997b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0997b-132">índice</span><span class="sxs-lookup"><span data-stu-id="0997b-132">index</span></span>|<span data-ttu-id="0997b-133">Int32</span><span class="sxs-lookup"><span data-stu-id="0997b-133">Int32</span></span>|<span data-ttu-id="0997b-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="0997b-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="0997b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0997b-136">Response</span></span>

<span data-ttu-id="0997b-137">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [WorkbookTableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0997b-137">If successful, this method returns `200 OK` response code and [WorkbookTableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0997b-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0997b-138">Example</span></span>
<span data-ttu-id="0997b-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0997b-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0997b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0997b-140">Request</span></span>
<span data-ttu-id="0997b-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0997b-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablerowcollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.tablerowcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 4
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0997b-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="0997b-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0997b-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0997b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablerowcollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0997b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="0997b-144">Response</span></span>
<span data-ttu-id="0997b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0997b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
