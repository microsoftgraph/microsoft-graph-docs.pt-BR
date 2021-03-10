---
title: 'ChartCollection: ItemAt'
description: Obtém um gráfico com base em sua posição na coleção.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e36ef7d95da25b216237f4abb4f5848199f51cd4
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578443"
---
# <a name="chartcollection-itemat"></a><span data-ttu-id="e29c0-103">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="e29c0-103">ChartCollection: ItemAt</span></span>

<span data-ttu-id="e29c0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e29c0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e29c0-105">Obtém um gráfico com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="e29c0-105">Gets a chart based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="e29c0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e29c0-106">Permissions</span></span>
<span data-ttu-id="e29c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e29c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e29c0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e29c0-109">Permission type</span></span>      | <span data-ttu-id="e29c0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e29c0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e29c0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e29c0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e29c0-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e29c0-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e29c0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e29c0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e29c0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e29c0-114">Not supported.</span></span>    |
|<span data-ttu-id="e29c0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e29c0-115">Application</span></span> | <span data-ttu-id="e29c0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e29c0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e29c0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e29c0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/itemAt
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="e29c0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e29c0-118">Request headers</span></span>
| <span data-ttu-id="e29c0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e29c0-119">Name</span></span>       | <span data-ttu-id="e29c0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e29c0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e29c0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e29c0-121">Authorization</span></span>  | <span data-ttu-id="e29c0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e29c0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e29c0-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e29c0-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e29c0-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e29c0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e29c0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e29c0-127">Request body</span></span>
<span data-ttu-id="e29c0-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e29c0-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e29c0-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e29c0-129">Parameter</span></span>    | <span data-ttu-id="e29c0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e29c0-130">Type</span></span>   |<span data-ttu-id="e29c0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e29c0-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e29c0-132">índice</span><span class="sxs-lookup"><span data-stu-id="e29c0-132">index</span></span>|<span data-ttu-id="e29c0-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e29c0-133">Int32</span></span>|<span data-ttu-id="e29c0-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="e29c0-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="e29c0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e29c0-136">Response</span></span>

<span data-ttu-id="e29c0-137">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [WorkbookChart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e29c0-137">If successful, this method returns `200 OK` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e29c0-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e29c0-138">Example</span></span>
<span data-ttu-id="e29c0-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e29c0-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e29c0-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e29c0-140">Request</span></span>
<span data-ttu-id="e29c0-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e29c0-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e29c0-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="e29c0-142">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "chartcollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.chartcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 8
}
```
# <a name="javascript"></a>[<span data-ttu-id="e29c0-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e29c0-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartcollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e29c0-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e29c0-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartcollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e29c0-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e29c0-145">Response</span></span>
<span data-ttu-id="e29c0-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e29c0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

