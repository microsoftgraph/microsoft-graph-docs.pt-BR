---
title: Atualizar chartlegend
description: Atualiza as propriedades do objeto chartlegend.
ms.openlocfilehash: c9c3d39bda04e178a892c94f2ea533460a7bfad8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007543"
---
# <a name="update-chartlegend"></a><span data-ttu-id="08b9e-103">Atualizar chartlegend</span><span class="sxs-lookup"><span data-stu-id="08b9e-103">Update chartlegend</span></span>

<span data-ttu-id="08b9e-104">Atualiza as propriedades do objeto chartlegend.</span><span class="sxs-lookup"><span data-stu-id="08b9e-104">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="08b9e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="08b9e-105">Permissions</span></span>
<span data-ttu-id="08b9e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08b9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08b9e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08b9e-108">Permission type</span></span>      | <span data-ttu-id="08b9e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08b9e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08b9e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08b9e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="08b9e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08b9e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="08b9e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08b9e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08b9e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08b9e-113">Not supported.</span></span>    |
|<span data-ttu-id="08b9e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08b9e-114">Application</span></span> | <span data-ttu-id="08b9e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08b9e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08b9e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08b9e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="08b9e-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="08b9e-117">Optional request headers</span></span>
| <span data-ttu-id="08b9e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="08b9e-118">Name</span></span>       | <span data-ttu-id="08b9e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="08b9e-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="08b9e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="08b9e-120">Authorization</span></span>  | <span data-ttu-id="08b9e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08b9e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08b9e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="08b9e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="08b9e-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="08b9e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="08b9e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08b9e-126">Request body</span></span>
<span data-ttu-id="08b9e-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="08b9e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="08b9e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08b9e-130">Property</span></span>     | <span data-ttu-id="08b9e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="08b9e-131">Type</span></span>   |<span data-ttu-id="08b9e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="08b9e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08b9e-133">overlay</span><span class="sxs-lookup"><span data-stu-id="08b9e-133">overlay</span></span>|<span data-ttu-id="08b9e-134">booliano</span><span class="sxs-lookup"><span data-stu-id="08b9e-134">boolean</span></span>|<span data-ttu-id="08b9e-135">Valor booliano para determinar se a legenda do gráfico deve se sobrepor ao corpo principal do gráfico.</span><span class="sxs-lookup"><span data-stu-id="08b9e-135">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="08b9e-136">position</span><span class="sxs-lookup"><span data-stu-id="08b9e-136">position</span></span>|<span data-ttu-id="08b9e-137">string</span><span class="sxs-lookup"><span data-stu-id="08b9e-137">string</span></span>|<span data-ttu-id="08b9e-138">Representa a posição da legenda no gráfico.</span><span class="sxs-lookup"><span data-stu-id="08b9e-138">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="08b9e-139">Os valores possíveis são: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="08b9e-139">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="08b9e-140">visible</span><span class="sxs-lookup"><span data-stu-id="08b9e-140">visible</span></span>|<span data-ttu-id="08b9e-141">booliano</span><span class="sxs-lookup"><span data-stu-id="08b9e-141">boolean</span></span>|<span data-ttu-id="08b9e-142">Um valor booliano que representa a visibilidade de um objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="08b9e-142">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="08b9e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="08b9e-143">Response</span></span>

<span data-ttu-id="08b9e-144">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto de [WorkbookChartLegend](../resources/chartlegend.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08b9e-144">If successful, this method returns a `200 OK` response code and updated [WorkbookChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="08b9e-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08b9e-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08b9e-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08b9e-146">Request</span></span>
<span data-ttu-id="08b9e-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08b9e-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
##### <a name="response"></a><span data-ttu-id="08b9e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="08b9e-148">Response</span></span>
<span data-ttu-id="08b9e-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08b9e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->