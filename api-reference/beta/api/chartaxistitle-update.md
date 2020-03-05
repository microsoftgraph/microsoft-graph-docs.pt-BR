---
title: Atualizar workbookChartAxisTitle
description: Atualize as propriedades do objeto workbookchartaxistitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 58e3a6b4715112386ea04fc6881cf7e3a8371f5b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42439643"
---
# <a name="update-workbookchartaxistitle"></a><span data-ttu-id="c90ef-103">Atualizar workbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="c90ef-103">Update workbookChartAxisTitle</span></span>

<span data-ttu-id="c90ef-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c90ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c90ef-105">Atualize as propriedades do objeto workbookChartAxisTitle.</span><span class="sxs-lookup"><span data-stu-id="c90ef-105">Update the properties of workbookChartAxisTitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c90ef-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c90ef-106">Permissions</span></span>
<span data-ttu-id="c90ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c90ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c90ef-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c90ef-109">Permission type</span></span>      | <span data-ttu-id="c90ef-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c90ef-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c90ef-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c90ef-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c90ef-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c90ef-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c90ef-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c90ef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c90ef-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c90ef-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c90ef-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c90ef-115">Application</span></span> | <span data-ttu-id="c90ef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c90ef-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c90ef-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c90ef-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="c90ef-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c90ef-118">Optional request headers</span></span>
| <span data-ttu-id="c90ef-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c90ef-119">Name</span></span>       | <span data-ttu-id="c90ef-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c90ef-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c90ef-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c90ef-121">Authorization</span></span>  | <span data-ttu-id="c90ef-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c90ef-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c90ef-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c90ef-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c90ef-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c90ef-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c90ef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c90ef-127">Request body</span></span>
<span data-ttu-id="c90ef-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c90ef-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c90ef-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c90ef-131">Property</span></span>     | <span data-ttu-id="c90ef-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="c90ef-132">Type</span></span>   |<span data-ttu-id="c90ef-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="c90ef-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c90ef-134">texto</span><span class="sxs-lookup"><span data-stu-id="c90ef-134">text</span></span>|<span data-ttu-id="c90ef-135">string</span><span class="sxs-lookup"><span data-stu-id="c90ef-135">string</span></span>|<span data-ttu-id="c90ef-136">Representa o título do eixo.</span><span class="sxs-lookup"><span data-stu-id="c90ef-136">Represents the axis title.</span></span>|
|<span data-ttu-id="c90ef-137">visible</span><span class="sxs-lookup"><span data-stu-id="c90ef-137">visible</span></span>|<span data-ttu-id="c90ef-138">booliano</span><span class="sxs-lookup"><span data-stu-id="c90ef-138">boolean</span></span>|<span data-ttu-id="c90ef-139">Um booliano que especifica a visibilidade de um título do eixo.</span><span class="sxs-lookup"><span data-stu-id="c90ef-139">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="c90ef-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c90ef-140">Response</span></span>

<span data-ttu-id="c90ef-141">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c90ef-141">If successful, this method returns a `200 OK` response code and updated [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c90ef-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c90ef-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c90ef-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c90ef-143">Request</span></span>
<span data-ttu-id="c90ef-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c90ef-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c90ef-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="c90ef-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
# <a name="c"></a>[<span data-ttu-id="c90ef-146">C#</span><span class="sxs-lookup"><span data-stu-id="c90ef-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartaxistitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c90ef-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c90ef-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartaxistitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c90ef-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c90ef-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartaxistitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c90ef-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c90ef-149">Response</span></span>
<span data-ttu-id="c90ef-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c90ef-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
