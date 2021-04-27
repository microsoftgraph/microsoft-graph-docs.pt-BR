---
title: Atualizar charttitle
description: Atualiza as propriedades do objeto charttitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 925308e4c68f6479f7da0059f077eb411edd4724
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047305"
---
# <a name="update-charttitle"></a><span data-ttu-id="948e1-103">Atualizar charttitle</span><span class="sxs-lookup"><span data-stu-id="948e1-103">Update charttitle</span></span>

<span data-ttu-id="948e1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="948e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="948e1-105">Atualiza as propriedades do objeto charttitle.</span><span class="sxs-lookup"><span data-stu-id="948e1-105">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="948e1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="948e1-106">Permissions</span></span>
<span data-ttu-id="948e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="948e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="948e1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="948e1-109">Permission type</span></span>      | <span data-ttu-id="948e1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="948e1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="948e1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="948e1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="948e1-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="948e1-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="948e1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="948e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="948e1-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="948e1-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="948e1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="948e1-115">Application</span></span> | <span data-ttu-id="948e1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="948e1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="948e1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="948e1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="948e1-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="948e1-118">Optional request headers</span></span>
| <span data-ttu-id="948e1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="948e1-119">Name</span></span>       | <span data-ttu-id="948e1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="948e1-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="948e1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="948e1-121">Authorization</span></span>  | <span data-ttu-id="948e1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="948e1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="948e1-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="948e1-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="948e1-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="948e1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="948e1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="948e1-127">Request body</span></span>
<span data-ttu-id="948e1-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="948e1-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="948e1-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="948e1-131">Property</span></span>     | <span data-ttu-id="948e1-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="948e1-132">Type</span></span>   |<span data-ttu-id="948e1-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="948e1-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="948e1-134">overlay</span><span class="sxs-lookup"><span data-stu-id="948e1-134">overlay</span></span>|<span data-ttu-id="948e1-135">booliano</span><span class="sxs-lookup"><span data-stu-id="948e1-135">boolean</span></span>|<span data-ttu-id="948e1-136">Valor booliano que determina se o título do gráfico deve se sobrepor ao gráfico ou não.</span><span class="sxs-lookup"><span data-stu-id="948e1-136">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="948e1-137">texto</span><span class="sxs-lookup"><span data-stu-id="948e1-137">text</span></span>|<span data-ttu-id="948e1-138">string</span><span class="sxs-lookup"><span data-stu-id="948e1-138">string</span></span>|<span data-ttu-id="948e1-139">Representa o texto do título de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="948e1-139">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="948e1-140">visible</span><span class="sxs-lookup"><span data-stu-id="948e1-140">visible</span></span>|<span data-ttu-id="948e1-141">booliano</span><span class="sxs-lookup"><span data-stu-id="948e1-141">boolean</span></span>|<span data-ttu-id="948e1-142">Um valor booliano que representa a visibilidade de um objeto de título de gráfico.</span><span class="sxs-lookup"><span data-stu-id="948e1-142">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="948e1-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="948e1-143">Response</span></span>

<span data-ttu-id="948e1-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [workbookChartTitle](../resources/workbookcharttitle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="948e1-144">If successful, this method returns a `200 OK` response code and updated [workbookChartTitle](../resources/workbookcharttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="948e1-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="948e1-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="948e1-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="948e1-146">Request</span></span>
<span data-ttu-id="948e1-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="948e1-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="948e1-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="948e1-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
# <a name="c"></a>[<span data-ttu-id="948e1-149">C#</span><span class="sxs-lookup"><span data-stu-id="948e1-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-charttitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="948e1-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="948e1-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-charttitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="948e1-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="948e1-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-charttitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="948e1-152">Java</span><span class="sxs-lookup"><span data-stu-id="948e1-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-charttitle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="948e1-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="948e1-153">Response</span></span>
<span data-ttu-id="948e1-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="948e1-154">Here is an example of the response.</span></span> <span data-ttu-id="948e1-155">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="948e1-155">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


