---
title: Atualizar gráfico
description: Atualiza as propriedades do objeto de gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8636c09c12b0c505dd4b71f104fa6e2b8711ddee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059954"
---
# <a name="update-chart"></a><span data-ttu-id="ea0dd-103">Atualizar gráfico</span><span class="sxs-lookup"><span data-stu-id="ea0dd-103">Update chart</span></span>

<span data-ttu-id="ea0dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea0dd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea0dd-105">Atualiza as propriedades do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="ea0dd-105">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea0dd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ea0dd-106">Permissions</span></span>
<span data-ttu-id="ea0dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea0dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea0dd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea0dd-109">Permission type</span></span>      | <span data-ttu-id="ea0dd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ea0dd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea0dd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea0dd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ea0dd-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea0dd-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ea0dd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea0dd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea0dd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea0dd-114">Not supported.</span></span>    |
|<span data-ttu-id="ea0dd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea0dd-115">Application</span></span> | <span data-ttu-id="ea0dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea0dd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea0dd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea0dd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="ea0dd-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="ea0dd-118">Optional request headers</span></span>
| <span data-ttu-id="ea0dd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ea0dd-119">Name</span></span>       | <span data-ttu-id="ea0dd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea0dd-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ea0dd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea0dd-121">Authorization</span></span>  | <span data-ttu-id="ea0dd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea0dd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ea0dd-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ea0dd-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="ea0dd-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ea0dd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea0dd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea0dd-127">Request body</span></span>
<span data-ttu-id="ea0dd-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ea0dd-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ea0dd-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea0dd-131">Property</span></span>     | <span data-ttu-id="ea0dd-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea0dd-132">Type</span></span>   |<span data-ttu-id="ea0dd-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea0dd-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea0dd-134">height</span><span class="sxs-lookup"><span data-stu-id="ea0dd-134">height</span></span>|<span data-ttu-id="ea0dd-135">Double</span><span class="sxs-lookup"><span data-stu-id="ea0dd-135">double</span></span>|<span data-ttu-id="ea0dd-136">Representa a altura, em pontos, do objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="ea0dd-136">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="ea0dd-137">left</span><span class="sxs-lookup"><span data-stu-id="ea0dd-137">left</span></span>|<span data-ttu-id="ea0dd-138">Double</span><span class="sxs-lookup"><span data-stu-id="ea0dd-138">double</span></span>|<span data-ttu-id="ea0dd-139">A distância, em pontos, da esquerda do gráfico à origem da planilha.</span><span class="sxs-lookup"><span data-stu-id="ea0dd-139">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="ea0dd-140">nome</span><span class="sxs-lookup"><span data-stu-id="ea0dd-140">name</span></span>|<span data-ttu-id="ea0dd-141">string</span><span class="sxs-lookup"><span data-stu-id="ea0dd-141">string</span></span>|<span data-ttu-id="ea0dd-142">Representa o nome de um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="ea0dd-142">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="ea0dd-143">top</span><span class="sxs-lookup"><span data-stu-id="ea0dd-143">top</span></span>|<span data-ttu-id="ea0dd-144">Double</span><span class="sxs-lookup"><span data-stu-id="ea0dd-144">double</span></span>|<span data-ttu-id="ea0dd-145">Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="ea0dd-145">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="ea0dd-146">width</span><span class="sxs-lookup"><span data-stu-id="ea0dd-146">width</span></span>|<span data-ttu-id="ea0dd-147">Double</span><span class="sxs-lookup"><span data-stu-id="ea0dd-147">double</span></span>|<span data-ttu-id="ea0dd-148">Representa a largura, em pontos, do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="ea0dd-148">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="ea0dd-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea0dd-149">Response</span></span>

<span data-ttu-id="ea0dd-150">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookChart](../resources/chart.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea0dd-150">If successful, this method returns a `200 OK` response code and updated [WorkbookChart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ea0dd-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea0dd-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea0dd-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea0dd-152">Request</span></span>
<span data-ttu-id="ea0dd-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea0dd-153">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ea0dd-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea0dd-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
# <a name="c"></a>[<span data-ttu-id="ea0dd-155">C#</span><span class="sxs-lookup"><span data-stu-id="ea0dd-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea0dd-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea0dd-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea0dd-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea0dd-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea0dd-158">Java</span><span class="sxs-lookup"><span data-stu-id="ea0dd-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chart-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ea0dd-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea0dd-159">Response</span></span>
<span data-ttu-id="ea0dd-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea0dd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

