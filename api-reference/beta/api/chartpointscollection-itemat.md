---
title: 'ChartPointsCollection: ItemAt'
description: Recupera um ponto com base na respectiva posição dentro da série.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2709031283af2778b23aec7c2261f4c8d9d4cb1e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982854"
---
# <a name="chartpointscollection-itemat"></a><span data-ttu-id="99976-103">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="99976-103">ChartPointsCollection: ItemAt</span></span>

<span data-ttu-id="99976-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99976-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99976-105">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="99976-105">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="99976-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="99976-106">Permissions</span></span>
<span data-ttu-id="99976-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99976-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99976-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99976-109">Permission type</span></span>      | <span data-ttu-id="99976-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="99976-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99976-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99976-111">Delegated (work or school account)</span></span> | <span data-ttu-id="99976-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99976-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="99976-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99976-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99976-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99976-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="99976-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99976-115">Application</span></span> | <span data-ttu-id="99976-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99976-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="99976-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99976-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="99976-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99976-118">Request headers</span></span>
| <span data-ttu-id="99976-119">Nome</span><span class="sxs-lookup"><span data-stu-id="99976-119">Name</span></span>       | <span data-ttu-id="99976-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="99976-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="99976-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="99976-121">Authorization</span></span>  | <span data-ttu-id="99976-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99976-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="99976-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="99976-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="99976-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="99976-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="99976-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99976-127">Request body</span></span>
<span data-ttu-id="99976-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99976-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="99976-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="99976-129">Parameter</span></span>    | <span data-ttu-id="99976-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="99976-130">Type</span></span>   |<span data-ttu-id="99976-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="99976-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99976-132">index</span><span class="sxs-lookup"><span data-stu-id="99976-132">index</span></span>|<span data-ttu-id="99976-133">number</span><span class="sxs-lookup"><span data-stu-id="99976-133">number</span></span>|<span data-ttu-id="99976-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="99976-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="99976-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="99976-136">Response</span></span>

<span data-ttu-id="99976-137">Se bem-sucedido, este método retorna o `200 OK` código de resposta e o objeto [workbookChartPoint](../resources/workbookchartpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99976-137">If successful, this method returns `200 OK` response code and [workbookChartPoint](../resources/workbookchartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99976-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99976-138">Example</span></span>
<span data-ttu-id="99976-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="99976-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="99976-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99976-140">Request</span></span>
<span data-ttu-id="99976-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99976-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="99976-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="99976-142">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="99976-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99976-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartpointscollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="99976-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="99976-144">Response</span></span>
<span data-ttu-id="99976-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99976-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


