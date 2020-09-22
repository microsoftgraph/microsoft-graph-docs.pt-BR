---
title: Atualizar chartgridlines
description: Atualiza as propriedades do objeto chartgridlines.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1556b66782281db417527c4fe35f5c5c5cb36bd6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982945"
---
# <a name="update-chartgridlines"></a><span data-ttu-id="4a625-103">Atualizar chartgridlines</span><span class="sxs-lookup"><span data-stu-id="4a625-103">Update chartgridlines</span></span>

<span data-ttu-id="4a625-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a625-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a625-105">Atualiza as propriedades do objeto chartgridlines.</span><span class="sxs-lookup"><span data-stu-id="4a625-105">Update the properties of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4a625-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a625-106">Permissions</span></span>
<span data-ttu-id="4a625-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a625-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a625-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a625-109">Permission type</span></span>      | <span data-ttu-id="4a625-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a625-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a625-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a625-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4a625-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a625-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4a625-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a625-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a625-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a625-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4a625-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a625-115">Application</span></span> | <span data-ttu-id="4a625-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a625-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a625-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a625-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/minorgridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/majorgridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/majorgridlines
```
## <a name="optional-request-headers"></a><span data-ttu-id="4a625-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="4a625-118">Optional request headers</span></span>
| <span data-ttu-id="4a625-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4a625-119">Name</span></span>       | <span data-ttu-id="4a625-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a625-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4a625-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a625-121">Authorization</span></span>  | <span data-ttu-id="4a625-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a625-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a625-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4a625-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="4a625-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="4a625-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a625-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a625-127">Request body</span></span>
<span data-ttu-id="4a625-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4a625-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4a625-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a625-131">Property</span></span>     | <span data-ttu-id="4a625-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a625-132">Type</span></span>   |<span data-ttu-id="4a625-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a625-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a625-134">visible</span><span class="sxs-lookup"><span data-stu-id="4a625-134">visible</span></span>|<span data-ttu-id="4a625-135">booliano</span><span class="sxs-lookup"><span data-stu-id="4a625-135">boolean</span></span>|<span data-ttu-id="4a625-136">Valor booliano que determina se as linhas de grade do eixo ficam visíveis ou não.</span><span class="sxs-lookup"><span data-stu-id="4a625-136">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="4a625-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a625-137">Response</span></span>

<span data-ttu-id="4a625-138">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookChartGridlines](../resources/workbookchartgridlines.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a625-138">If successful, this method returns a `200 OK` response code and updated [workbookChartGridlines](../resources/workbookchartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a625-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a625-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a625-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a625-140">Request</span></span>
<span data-ttu-id="4a625-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a625-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a625-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a625-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartgridlines"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/minorgridlines
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```
# <a name="c"></a>[<span data-ttu-id="4a625-143">C#</span><span class="sxs-lookup"><span data-stu-id="4a625-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartgridlines-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a625-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a625-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartgridlines-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a625-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a625-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartgridlines-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4a625-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a625-146">Response</span></span>
<span data-ttu-id="4a625-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a625-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartGridlines"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartgridlines",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


