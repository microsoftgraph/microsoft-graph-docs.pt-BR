---
title: Atualizar chartlineformat
description: Atualiza as propriedades do objeto chartlineformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: aa8e90142de30451c277961cef55de54e80c9e93
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083894"
---
# <a name="update-chartlineformat"></a><span data-ttu-id="13000-103">Atualizar chartlineformat</span><span class="sxs-lookup"><span data-stu-id="13000-103">Update chartlineformat</span></span>

<span data-ttu-id="13000-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13000-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="13000-105">Atualiza as propriedades do objeto chartlineformat.</span><span class="sxs-lookup"><span data-stu-id="13000-105">Update the properties of chartlineformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="13000-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="13000-106">Permissions</span></span>
<span data-ttu-id="13000-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13000-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13000-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13000-109">Permission type</span></span>      | <span data-ttu-id="13000-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13000-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13000-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13000-111">Delegated (work or school account)</span></span> | <span data-ttu-id="13000-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13000-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="13000-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13000-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13000-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13000-114">Not supported.</span></span>    |
|<span data-ttu-id="13000-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13000-115">Application</span></span> | <span data-ttu-id="13000-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13000-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="13000-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13000-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorgridlines/format/line
```
## <a name="optional-request-headers"></a><span data-ttu-id="13000-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="13000-118">Optional request headers</span></span>
| <span data-ttu-id="13000-119">Nome</span><span class="sxs-lookup"><span data-stu-id="13000-119">Name</span></span>       | <span data-ttu-id="13000-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="13000-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="13000-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="13000-121">Authorization</span></span>  | <span data-ttu-id="13000-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13000-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="13000-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="13000-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="13000-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="13000-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="13000-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13000-127">Request body</span></span>
<span data-ttu-id="13000-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="13000-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="13000-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13000-131">Property</span></span>     | <span data-ttu-id="13000-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="13000-132">Type</span></span>   |<span data-ttu-id="13000-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="13000-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13000-134">color</span><span class="sxs-lookup"><span data-stu-id="13000-134">color</span></span>|<span data-ttu-id="13000-135">string</span><span class="sxs-lookup"><span data-stu-id="13000-135">string</span></span>|<span data-ttu-id="13000-136">Código de cor HTML que representa a cor das linhas no gráfico.</span><span class="sxs-lookup"><span data-stu-id="13000-136">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="response"></a><span data-ttu-id="13000-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="13000-137">Response</span></span>

<span data-ttu-id="13000-138">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookChartLineFormat](../resources/chartlineformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13000-138">If successful, this method returns a `200 OK` response code and updated [WorkbookChartLineFormat](../resources/chartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="13000-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13000-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13000-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13000-140">Request</span></span>
<span data-ttu-id="13000-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13000-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="13000-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="13000-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartlineformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
# <a name="c"></a>[<span data-ttu-id="13000-143">C#</span><span class="sxs-lookup"><span data-stu-id="13000-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartlineformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13000-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13000-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartlineformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13000-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13000-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartlineformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13000-146">Java</span><span class="sxs-lookup"><span data-stu-id="13000-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartlineformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="13000-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="13000-147">Response</span></span>
<span data-ttu-id="13000-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13000-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlineformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

