---
title: 'ChartCollection: add'
description: Cria um novo gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: cdb3ff01b0741f0f1a4a0bff22e3a8e3dc32335c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516333"
---
# <a name="chartcollection-add"></a><span data-ttu-id="fe6b0-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="fe6b0-103">ChartCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe6b0-104">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="fe6b0-104">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe6b0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe6b0-105">Permissions</span></span>
<span data-ttu-id="fe6b0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe6b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe6b0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe6b0-108">Permission type</span></span>      | <span data-ttu-id="fe6b0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe6b0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe6b0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe6b0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fe6b0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe6b0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fe6b0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe6b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe6b0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe6b0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fe6b0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe6b0-114">Application</span></span> | <span data-ttu-id="fe6b0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe6b0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe6b0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe6b0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="fe6b0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe6b0-117">Request headers</span></span>
| <span data-ttu-id="fe6b0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="fe6b0-118">Name</span></span>       | <span data-ttu-id="fe6b0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe6b0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fe6b0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe6b0-120">Authorization</span></span>  | <span data-ttu-id="fe6b0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe6b0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe6b0-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fe6b0-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="fe6b0-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="fe6b0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe6b0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe6b0-126">Request body</span></span>
<span data-ttu-id="fe6b0-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe6b0-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fe6b0-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fe6b0-128">Parameter</span></span>    | <span data-ttu-id="fe6b0-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe6b0-129">Type</span></span>   |<span data-ttu-id="fe6b0-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe6b0-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe6b0-131">type</span><span class="sxs-lookup"><span data-stu-id="fe6b0-131">type</span></span>|<span data-ttu-id="fe6b0-132">string</span><span class="sxs-lookup"><span data-stu-id="fe6b0-132">string</span></span>|<span data-ttu-id="fe6b0-p104">Representa o tipo de um gráfico.  Os valores possíveis são: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie` e `etc.`.</span><span class="sxs-lookup"><span data-stu-id="fe6b0-p104">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="fe6b0-135">sourceData</span><span class="sxs-lookup"><span data-stu-id="fe6b0-135">sourceData</span></span>|<span data-ttu-id="fe6b0-136">string</span><span class="sxs-lookup"><span data-stu-id="fe6b0-136">string</span></span>|<span data-ttu-id="fe6b0-137">O objeto Range que corresponde aos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="fe6b0-137">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="fe6b0-138">seriesBy</span><span class="sxs-lookup"><span data-stu-id="fe6b0-138">seriesBy</span></span>|<span data-ttu-id="fe6b0-139">string</span><span class="sxs-lookup"><span data-stu-id="fe6b0-139">string</span></span>|<span data-ttu-id="fe6b0-p105">Opcional. Especifica a forma como as colunas ou linhas são usadas como séries de dados no gráfico.  Os valores possíveis são: `Auto`, `Columns` e `Rows`.</span><span class="sxs-lookup"><span data-stu-id="fe6b0-p105">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="fe6b0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe6b0-143">Response</span></span>

<span data-ttu-id="fe6b0-144">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Chart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe6b0-144">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe6b0-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe6b0-145">Example</span></span>
<span data-ttu-id="fe6b0-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="fe6b0-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fe6b0-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe6b0-147">Request</span></span>
<span data-ttu-id="fe6b0-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe6b0-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```

##### <a name="response"></a><span data-ttu-id="fe6b0-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe6b0-149">Response</span></span>
<span data-ttu-id="fe6b0-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe6b0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartcollection-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
