---
title: Atualizar chartaxistitle
description: Atualiza as propriedades do objeto chartaxistitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 07503fd8a90aecdf07737ddf0cf2c11438777a51
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048824"
---
# <a name="update-chartaxistitle"></a><span data-ttu-id="28a4f-103">Atualizar chartaxistitle</span><span class="sxs-lookup"><span data-stu-id="28a4f-103">Update chartaxistitle</span></span>

<span data-ttu-id="28a4f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28a4f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="28a4f-105">Atualiza as propriedades do objeto chartaxistitle.</span><span class="sxs-lookup"><span data-stu-id="28a4f-105">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="28a4f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="28a4f-106">Permissions</span></span>
<span data-ttu-id="28a4f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28a4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28a4f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28a4f-109">Permission type</span></span>      | <span data-ttu-id="28a4f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28a4f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28a4f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28a4f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="28a4f-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28a4f-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="28a4f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28a4f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28a4f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28a4f-114">Not supported.</span></span>    |
|<span data-ttu-id="28a4f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28a4f-115">Application</span></span> | <span data-ttu-id="28a4f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28a4f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28a4f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28a4f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/title
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/title
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="28a4f-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="28a4f-118">Optional request headers</span></span>
| <span data-ttu-id="28a4f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="28a4f-119">Name</span></span>       | <span data-ttu-id="28a4f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="28a4f-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="28a4f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="28a4f-121">Authorization</span></span>  | <span data-ttu-id="28a4f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28a4f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="28a4f-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="28a4f-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="28a4f-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="28a4f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="28a4f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28a4f-127">Request body</span></span>
<span data-ttu-id="28a4f-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="28a4f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="28a4f-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28a4f-131">Property</span></span>     | <span data-ttu-id="28a4f-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="28a4f-132">Type</span></span>   |<span data-ttu-id="28a4f-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="28a4f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28a4f-134">texto</span><span class="sxs-lookup"><span data-stu-id="28a4f-134">text</span></span>|<span data-ttu-id="28a4f-135">string</span><span class="sxs-lookup"><span data-stu-id="28a4f-135">string</span></span>|<span data-ttu-id="28a4f-136">Representa o título do eixo.</span><span class="sxs-lookup"><span data-stu-id="28a4f-136">Represents the axis title.</span></span>|
|<span data-ttu-id="28a4f-137">visible</span><span class="sxs-lookup"><span data-stu-id="28a4f-137">visible</span></span>|<span data-ttu-id="28a4f-138">booliano</span><span class="sxs-lookup"><span data-stu-id="28a4f-138">boolean</span></span>|<span data-ttu-id="28a4f-139">Um booliano que especifica a visibilidade de um título do eixo.</span><span class="sxs-lookup"><span data-stu-id="28a4f-139">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="28a4f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="28a4f-140">Response</span></span>

<span data-ttu-id="28a4f-141">Se tiver êxito, este método retornará um código de resposta e `200 OK` o [objeto WorkbookChartAxisTitle](../resources/chartaxistitle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28a4f-141">If successful, this method returns a `200 OK` response code and updated [WorkbookChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="28a4f-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28a4f-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28a4f-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28a4f-143">Request</span></span>
<span data-ttu-id="28a4f-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28a4f-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28a4f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="28a4f-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
# <a name="c"></a>[<span data-ttu-id="28a4f-146">C#</span><span class="sxs-lookup"><span data-stu-id="28a4f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartaxistitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28a4f-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28a4f-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartaxistitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28a4f-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28a4f-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartaxistitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28a4f-149">Java</span><span class="sxs-lookup"><span data-stu-id="28a4f-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartaxistitle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="28a4f-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="28a4f-150">Response</span></span>
<span data-ttu-id="28a4f-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28a4f-151">Here is an example of the response.</span></span> <span data-ttu-id="28a4f-152">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="28a4f-152">Note: The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

