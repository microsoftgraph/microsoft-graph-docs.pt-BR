---
title: Atualizar chartlegend
description: Atualiza as propriedades do objeto chartlegend.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 6299de840cef45827a026d0201d1699e047f685c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958608"
---
# <a name="update-chartlegend"></a><span data-ttu-id="146c5-103">Atualizar chartlegend</span><span class="sxs-lookup"><span data-stu-id="146c5-103">Update chartlegend</span></span>

<span data-ttu-id="146c5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="146c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="146c5-105">Atualiza as propriedades do objeto chartlegend.</span><span class="sxs-lookup"><span data-stu-id="146c5-105">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="146c5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="146c5-106">Permissions</span></span>
<span data-ttu-id="146c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="146c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="146c5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="146c5-109">Permission type</span></span>      | <span data-ttu-id="146c5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="146c5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="146c5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="146c5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="146c5-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="146c5-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="146c5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="146c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="146c5-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="146c5-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="146c5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="146c5-115">Application</span></span> | <span data-ttu-id="146c5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="146c5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="146c5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="146c5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="146c5-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="146c5-118">Optional request headers</span></span>
| <span data-ttu-id="146c5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="146c5-119">Name</span></span>       | <span data-ttu-id="146c5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="146c5-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="146c5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="146c5-121">Authorization</span></span>  | <span data-ttu-id="146c5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="146c5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="146c5-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="146c5-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="146c5-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="146c5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="146c5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="146c5-127">Request body</span></span>
<span data-ttu-id="146c5-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="146c5-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="146c5-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="146c5-131">Property</span></span>     | <span data-ttu-id="146c5-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="146c5-132">Type</span></span>   |<span data-ttu-id="146c5-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="146c5-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="146c5-134">overlay</span><span class="sxs-lookup"><span data-stu-id="146c5-134">overlay</span></span>|<span data-ttu-id="146c5-135">booliano</span><span class="sxs-lookup"><span data-stu-id="146c5-135">boolean</span></span>|<span data-ttu-id="146c5-136">Valor booliano para determinar se a legenda do gráfico deve se sobrepor ao corpo principal do gráfico.</span><span class="sxs-lookup"><span data-stu-id="146c5-136">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="146c5-137">position</span><span class="sxs-lookup"><span data-stu-id="146c5-137">position</span></span>|<span data-ttu-id="146c5-138">string</span><span class="sxs-lookup"><span data-stu-id="146c5-138">string</span></span>|<span data-ttu-id="146c5-p105">Representa a posição da legenda no gráfico. Os valores possíveis são: `Top`, `Bottom`, `Left`, `Right`, `Corner` e `Custom`.</span><span class="sxs-lookup"><span data-stu-id="146c5-p105">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="146c5-141">visible</span><span class="sxs-lookup"><span data-stu-id="146c5-141">visible</span></span>|<span data-ttu-id="146c5-142">booliano</span><span class="sxs-lookup"><span data-stu-id="146c5-142">boolean</span></span>|<span data-ttu-id="146c5-143">Um valor booliano que representa a visibilidade de um objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="146c5-143">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="146c5-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="146c5-144">Response</span></span>

<span data-ttu-id="146c5-145">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookChartLegend](../resources/workbookchartlegend.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="146c5-145">If successful, this method returns a `200 OK` response code and updated [workbookChartLegend](../resources/workbookchartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="146c5-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="146c5-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="146c5-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="146c5-147">Request</span></span>
<span data-ttu-id="146c5-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="146c5-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="146c5-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="146c5-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
# <a name="c"></a>[<span data-ttu-id="146c5-150">C#</span><span class="sxs-lookup"><span data-stu-id="146c5-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartlegend-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="146c5-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="146c5-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartlegend-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="146c5-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="146c5-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartlegend-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="146c5-153">Java</span><span class="sxs-lookup"><span data-stu-id="146c5-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartlegend-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="146c5-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="146c5-154">Response</span></span>
<span data-ttu-id="146c5-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="146c5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


