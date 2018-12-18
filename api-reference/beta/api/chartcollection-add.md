---
title: 'ChartCollection: add'
description: Cria um novo gráfico.
author: lumine2008
ms.openlocfilehash: 704afc9890e3921c69cdd7b746c0e362c4627511
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325547"
---
# <a name="chartcollection-add"></a><span data-ttu-id="0671c-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="0671c-103">ChartCollection: add</span></span>

> <span data-ttu-id="0671c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0671c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0671c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0671c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0671c-106">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="0671c-106">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="0671c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0671c-107">Permissions</span></span>
<span data-ttu-id="0671c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0671c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0671c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0671c-110">Permission type</span></span>      | <span data-ttu-id="0671c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0671c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0671c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0671c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0671c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0671c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0671c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0671c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0671c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0671c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0671c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0671c-116">Application</span></span> | <span data-ttu-id="0671c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0671c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0671c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0671c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="0671c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0671c-119">Request headers</span></span>
| <span data-ttu-id="0671c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0671c-120">Name</span></span>       | <span data-ttu-id="0671c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0671c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0671c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0671c-122">Authorization</span></span>  | <span data-ttu-id="0671c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0671c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0671c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0671c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="0671c-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0671c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0671c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0671c-128">Request body</span></span>
<span data-ttu-id="0671c-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0671c-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0671c-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0671c-130">Parameter</span></span>    | <span data-ttu-id="0671c-131">Type</span><span class="sxs-lookup"><span data-stu-id="0671c-131">Type</span></span>   |<span data-ttu-id="0671c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0671c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0671c-133">type</span><span class="sxs-lookup"><span data-stu-id="0671c-133">type</span></span>|<span data-ttu-id="0671c-134">string</span><span class="sxs-lookup"><span data-stu-id="0671c-134">string</span></span>|<span data-ttu-id="0671c-p105">Representa o tipo de um gráfico.  Os valores possíveis são: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie` e `etc.`.</span><span class="sxs-lookup"><span data-stu-id="0671c-p105">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="0671c-137">sourceData</span><span class="sxs-lookup"><span data-stu-id="0671c-137">sourceData</span></span>|<span data-ttu-id="0671c-138">string</span><span class="sxs-lookup"><span data-stu-id="0671c-138">string</span></span>|<span data-ttu-id="0671c-139">O objeto Range que corresponde aos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="0671c-139">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="0671c-140">seriesBy</span><span class="sxs-lookup"><span data-stu-id="0671c-140">seriesBy</span></span>|<span data-ttu-id="0671c-141">string</span><span class="sxs-lookup"><span data-stu-id="0671c-141">string</span></span>|<span data-ttu-id="0671c-p106">Opcional. Especifica a forma como as colunas ou linhas são usadas como séries de dados no gráfico.  Os valores possíveis são: `Auto`, `Columns` e `Rows`.</span><span class="sxs-lookup"><span data-stu-id="0671c-p106">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="0671c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="0671c-145">Response</span></span>

<span data-ttu-id="0671c-146">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Chart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0671c-146">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0671c-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0671c-147">Example</span></span>
<span data-ttu-id="0671c-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0671c-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0671c-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0671c-149">Request</span></span>
<span data-ttu-id="0671c-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0671c-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="0671c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="0671c-151">Response</span></span>
<span data-ttu-id="0671c-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0671c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
