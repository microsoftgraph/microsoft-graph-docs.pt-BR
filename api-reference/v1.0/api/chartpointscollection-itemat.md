---
title: 'ChartPointsCollection: ItemAt'
description: Recupera um ponto com base na respectiva posição dentro da série.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5b5766e19fd58548706c6fbc319697871aac8efa
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054144"
---
# <a name="chartpointscollection-itemat"></a><span data-ttu-id="19aab-103">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="19aab-103">ChartPointsCollection: ItemAt</span></span>

<span data-ttu-id="19aab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19aab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19aab-105">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="19aab-105">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="19aab-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="19aab-106">Permissions</span></span>
<span data-ttu-id="19aab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19aab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19aab-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19aab-109">Permission type</span></span>      | <span data-ttu-id="19aab-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19aab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19aab-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19aab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="19aab-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19aab-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19aab-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19aab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19aab-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19aab-114">Not supported.</span></span>    |
|<span data-ttu-id="19aab-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19aab-115">Application</span></span> | <span data-ttu-id="19aab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19aab-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19aab-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19aab-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points/itemAt
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="19aab-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19aab-118">Request headers</span></span>
| <span data-ttu-id="19aab-119">Nome</span><span class="sxs-lookup"><span data-stu-id="19aab-119">Name</span></span>       | <span data-ttu-id="19aab-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="19aab-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="19aab-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="19aab-121">Authorization</span></span>  | <span data-ttu-id="19aab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19aab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19aab-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="19aab-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="19aab-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="19aab-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="19aab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19aab-127">Request body</span></span>
<span data-ttu-id="19aab-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19aab-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="19aab-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="19aab-129">Parameter</span></span>    | <span data-ttu-id="19aab-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="19aab-130">Type</span></span>   |<span data-ttu-id="19aab-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="19aab-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19aab-132">índice</span><span class="sxs-lookup"><span data-stu-id="19aab-132">index</span></span>|<span data-ttu-id="19aab-133">Int32</span><span class="sxs-lookup"><span data-stu-id="19aab-133">Int32</span></span>|<span data-ttu-id="19aab-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="19aab-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="19aab-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="19aab-136">Response</span></span>

<span data-ttu-id="19aab-137">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [WorkbookChartPoint](../resources/chartpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19aab-137">If successful, this method returns `200 OK` response code and [WorkbookChartPoint](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19aab-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19aab-138">Example</span></span>
<span data-ttu-id="19aab-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="19aab-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="19aab-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19aab-140">Request</span></span>
<span data-ttu-id="19aab-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19aab-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="19aab-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="19aab-142">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "chartpointscollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.chartpointscollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 8
}
```
# <a name="javascript"></a>[<span data-ttu-id="19aab-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19aab-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartpointscollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19aab-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19aab-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartpointscollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="19aab-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="19aab-145">Response</span></span>
<span data-ttu-id="19aab-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19aab-146">Here is an example of the response.</span></span> <span data-ttu-id="19aab-147">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="19aab-147">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 20

{
  "value": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointsCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

