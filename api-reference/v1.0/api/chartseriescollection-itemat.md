---
title: 'ChartSeriesCollection: ItemAt'
description: Recupera uma série com base na respectiva posição na coleção.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6d6d9cc9b8625d5303843d7427d3eb3e23cec82b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912761"
---
# <a name="chartseriescollection-itemat"></a><span data-ttu-id="e2bbf-103">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="e2bbf-103">ChartSeriesCollection: ItemAt</span></span>

<span data-ttu-id="e2bbf-104">Recupera uma série com base na respectiva posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="e2bbf-104">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="e2bbf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2bbf-105">Permissions</span></span>
<span data-ttu-id="e2bbf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2bbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2bbf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2bbf-108">Permission type</span></span>      | <span data-ttu-id="e2bbf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2bbf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2bbf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2bbf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e2bbf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2bbf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e2bbf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2bbf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2bbf-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2bbf-113">Not supported.</span></span>    |
|<span data-ttu-id="e2bbf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2bbf-114">Application</span></span> | <span data-ttu-id="e2bbf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2bbf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2bbf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2bbf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="e2bbf-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2bbf-117">Request headers</span></span>
| <span data-ttu-id="e2bbf-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e2bbf-118">Name</span></span>       | <span data-ttu-id="e2bbf-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2bbf-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e2bbf-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2bbf-120">Authorization</span></span>  | <span data-ttu-id="e2bbf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2bbf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e2bbf-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e2bbf-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e2bbf-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e2bbf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2bbf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2bbf-126">Request body</span></span>
<span data-ttu-id="e2bbf-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2bbf-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e2bbf-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e2bbf-128">Parameter</span></span>    | <span data-ttu-id="e2bbf-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2bbf-129">Type</span></span>   |<span data-ttu-id="e2bbf-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2bbf-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2bbf-131">índice</span><span class="sxs-lookup"><span data-stu-id="e2bbf-131">index</span></span>|<span data-ttu-id="e2bbf-132">Int32</span><span class="sxs-lookup"><span data-stu-id="e2bbf-132">Int32</span></span>|<span data-ttu-id="e2bbf-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="e2bbf-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="e2bbf-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2bbf-135">Response</span></span>

<span data-ttu-id="e2bbf-136">Se tiver êxito, este método retornará `200 OK` código de resposta e o objeto [WorkbookChartSeries](../resources/chartseries.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2bbf-136">If successful, this method returns `200 OK` response code and [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2bbf-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2bbf-137">Example</span></span>
<span data-ttu-id="e2bbf-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e2bbf-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e2bbf-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2bbf-139">Request</span></span>
<span data-ttu-id="e2bbf-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2bbf-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "chartseriescollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 2
}
```

##### <a name="response"></a><span data-ttu-id="e2bbf-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2bbf-141">Response</span></span>
<span data-ttu-id="e2bbf-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2bbf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
