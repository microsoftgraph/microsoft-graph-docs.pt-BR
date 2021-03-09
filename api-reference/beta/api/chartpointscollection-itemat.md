---
title: 'ChartPointsCollection: ItemAt'
description: Recupera um ponto com base na respectiva posição dentro da série.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8208fff0436bf1764a8b25959768a94d1966d920
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574426"
---
# <a name="chartpointscollection-itemat"></a><span data-ttu-id="5c16b-103">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="5c16b-103">ChartPointsCollection: ItemAt</span></span>

<span data-ttu-id="5c16b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c16b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c16b-105">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="5c16b-105">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="5c16b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c16b-106">Permissions</span></span>
<span data-ttu-id="5c16b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c16b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c16b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c16b-109">Permission type</span></span>      | <span data-ttu-id="5c16b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c16b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c16b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c16b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5c16b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c16b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5c16b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c16b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c16b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c16b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5c16b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c16b-115">Application</span></span> | <span data-ttu-id="5c16b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c16b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c16b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c16b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points/ItemAt
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="5c16b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c16b-118">Request headers</span></span>
| <span data-ttu-id="5c16b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5c16b-119">Name</span></span>       | <span data-ttu-id="5c16b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c16b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5c16b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c16b-121">Authorization</span></span>  | <span data-ttu-id="5c16b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c16b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5c16b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5c16b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="5c16b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5c16b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c16b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c16b-127">Request body</span></span>
<span data-ttu-id="5c16b-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c16b-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5c16b-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5c16b-129">Parameter</span></span>    | <span data-ttu-id="5c16b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c16b-130">Type</span></span>   |<span data-ttu-id="5c16b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c16b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c16b-132">index</span><span class="sxs-lookup"><span data-stu-id="5c16b-132">index</span></span>|<span data-ttu-id="5c16b-133">number</span><span class="sxs-lookup"><span data-stu-id="5c16b-133">number</span></span>|<span data-ttu-id="5c16b-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="5c16b-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="5c16b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c16b-136">Response</span></span>

<span data-ttu-id="5c16b-137">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [workbookChartPoint](../resources/workbookchartpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c16b-137">If successful, this method returns `200 OK` response code and [workbookChartPoint](../resources/workbookchartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c16b-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c16b-138">Example</span></span>
<span data-ttu-id="5c16b-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5c16b-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5c16b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c16b-140">Request</span></span>
<span data-ttu-id="5c16b-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c16b-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c16b-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c16b-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartpointscollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="5c16b-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c16b-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartpointscollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5c16b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c16b-144">Response</span></span>
<span data-ttu-id="5c16b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c16b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartPointsCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


