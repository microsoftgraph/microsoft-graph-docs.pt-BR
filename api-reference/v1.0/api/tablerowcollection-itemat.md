---
title: 'TableRowCollection: ItemAt'
description: Obtém uma linha com base em sua posição na coleção.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 36f1fc28721710be5250309dcee357be34768b7b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48012779"
---
# <a name="tablerowcollection-itemat"></a><span data-ttu-id="5de10-103">TableRowCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="5de10-103">TableRowCollection: ItemAt</span></span>

<span data-ttu-id="5de10-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5de10-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5de10-105">Obtém uma linha com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="5de10-105">Gets a row based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="5de10-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5de10-106">Permissions</span></span>
<span data-ttu-id="5de10-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5de10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5de10-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5de10-109">Permission type</span></span>      | <span data-ttu-id="5de10-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5de10-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5de10-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5de10-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5de10-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5de10-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5de10-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5de10-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5de10-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5de10-114">Not supported.</span></span>    |
|<span data-ttu-id="5de10-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5de10-115">Application</span></span> | <span data-ttu-id="5de10-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5de10-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5de10-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5de10-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/itemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="5de10-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5de10-118">Request headers</span></span>
| <span data-ttu-id="5de10-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5de10-119">Name</span></span>       | <span data-ttu-id="5de10-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5de10-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5de10-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5de10-121">Authorization</span></span>  | <span data-ttu-id="5de10-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5de10-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5de10-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5de10-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="5de10-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5de10-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5de10-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5de10-127">Request body</span></span>
<span data-ttu-id="5de10-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5de10-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5de10-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5de10-129">Parameter</span></span>    | <span data-ttu-id="5de10-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5de10-130">Type</span></span>   |<span data-ttu-id="5de10-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5de10-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5de10-132">índice</span><span class="sxs-lookup"><span data-stu-id="5de10-132">index</span></span>|<span data-ttu-id="5de10-133">Int32</span><span class="sxs-lookup"><span data-stu-id="5de10-133">Int32</span></span>|<span data-ttu-id="5de10-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="5de10-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="5de10-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5de10-136">Response</span></span>

<span data-ttu-id="5de10-137">Se bem-sucedido, este método retorna o `200 OK` código de resposta e o objeto [WorkbookTableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5de10-137">If successful, this method returns `200 OK` response code and [WorkbookTableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5de10-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5de10-138">Example</span></span>
<span data-ttu-id="5de10-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5de10-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5de10-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5de10-140">Request</span></span>
<span data-ttu-id="5de10-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5de10-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5de10-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="5de10-142">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="5de10-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5de10-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5de10-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5de10-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablerowcollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5de10-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="5de10-145">Response</span></span>
<span data-ttu-id="5de10-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5de10-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

