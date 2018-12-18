---
title: Atualizar gráfico
description: Atualiza as propriedades do objeto de gráfico.
author: lumine2008
ms.openlocfilehash: 086d4a2ea0ce823ace141df0d5576af732bf8c0f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328179"
---
# <a name="update-chart"></a><span data-ttu-id="89ae6-103">Atualizar gráfico</span><span class="sxs-lookup"><span data-stu-id="89ae6-103">Update chart</span></span>

> <span data-ttu-id="89ae6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="89ae6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89ae6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="89ae6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89ae6-106">Atualiza as propriedades do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="89ae6-106">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="89ae6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="89ae6-107">Permissions</span></span>
<span data-ttu-id="89ae6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89ae6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89ae6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89ae6-110">Permission type</span></span>      | <span data-ttu-id="89ae6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89ae6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89ae6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89ae6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="89ae6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89ae6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="89ae6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89ae6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89ae6-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89ae6-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="89ae6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89ae6-116">Application</span></span> | <span data-ttu-id="89ae6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89ae6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89ae6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89ae6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="89ae6-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="89ae6-119">Optional request headers</span></span>
| <span data-ttu-id="89ae6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="89ae6-120">Name</span></span>       | <span data-ttu-id="89ae6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="89ae6-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="89ae6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="89ae6-122">Authorization</span></span>  | <span data-ttu-id="89ae6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89ae6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="89ae6-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="89ae6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="89ae6-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="89ae6-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="89ae6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89ae6-128">Request body</span></span>
<span data-ttu-id="89ae6-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="89ae6-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="89ae6-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89ae6-132">Property</span></span>     | <span data-ttu-id="89ae6-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="89ae6-133">Type</span></span>   |<span data-ttu-id="89ae6-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="89ae6-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89ae6-135">height</span><span class="sxs-lookup"><span data-stu-id="89ae6-135">height</span></span>|<span data-ttu-id="89ae6-136">Double</span><span class="sxs-lookup"><span data-stu-id="89ae6-136">double</span></span>|<span data-ttu-id="89ae6-137">Representa a altura, em pontos, do objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="89ae6-137">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="89ae6-138">left</span><span class="sxs-lookup"><span data-stu-id="89ae6-138">left</span></span>|<span data-ttu-id="89ae6-139">Double</span><span class="sxs-lookup"><span data-stu-id="89ae6-139">double</span></span>|<span data-ttu-id="89ae6-140">A distância, em pontos, da esquerda do gráfico à origem da planilha.</span><span class="sxs-lookup"><span data-stu-id="89ae6-140">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="89ae6-141">name</span><span class="sxs-lookup"><span data-stu-id="89ae6-141">name</span></span>|<span data-ttu-id="89ae6-142">string</span><span class="sxs-lookup"><span data-stu-id="89ae6-142">string</span></span>|<span data-ttu-id="89ae6-143">Representa o nome de um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="89ae6-143">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="89ae6-144">top</span><span class="sxs-lookup"><span data-stu-id="89ae6-144">top</span></span>|<span data-ttu-id="89ae6-145">Double</span><span class="sxs-lookup"><span data-stu-id="89ae6-145">double</span></span>|<span data-ttu-id="89ae6-146">Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="89ae6-146">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="89ae6-147">width</span><span class="sxs-lookup"><span data-stu-id="89ae6-147">width</span></span>|<span data-ttu-id="89ae6-148">Double</span><span class="sxs-lookup"><span data-stu-id="89ae6-148">double</span></span>|<span data-ttu-id="89ae6-149">Representa a largura, em pontos, do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="89ae6-149">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="89ae6-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="89ae6-150">Response</span></span>

<span data-ttu-id="89ae6-151">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Chart](../resources/chart.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89ae6-151">If successful, this method returns a `200 OK` response code and updated [Chart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="89ae6-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89ae6-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89ae6-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89ae6-153">Request</span></span>
<span data-ttu-id="89ae6-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89ae6-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
##### <a name="response"></a><span data-ttu-id="89ae6-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="89ae6-155">Response</span></span>
<span data-ttu-id="89ae6-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89ae6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->