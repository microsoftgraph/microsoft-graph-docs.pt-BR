---
title: Atualizar charttitle
description: Atualiza as propriedades do objeto charttitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 84f7f6f074469f11986044575ccf45282ff4d581
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054088"
---
# <a name="update-charttitle"></a><span data-ttu-id="da384-103">Atualizar charttitle</span><span class="sxs-lookup"><span data-stu-id="da384-103">Update charttitle</span></span>

<span data-ttu-id="da384-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da384-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da384-105">Atualiza as propriedades do objeto charttitle.</span><span class="sxs-lookup"><span data-stu-id="da384-105">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="da384-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="da384-106">Permissions</span></span>
<span data-ttu-id="da384-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da384-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da384-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da384-109">Permission type</span></span>      | <span data-ttu-id="da384-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da384-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da384-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da384-111">Delegated (work or school account)</span></span> | <span data-ttu-id="da384-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da384-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="da384-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da384-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da384-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da384-114">Not supported.</span></span>    |
|<span data-ttu-id="da384-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da384-115">Application</span></span> | <span data-ttu-id="da384-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da384-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da384-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da384-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="da384-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="da384-118">Optional request headers</span></span>
| <span data-ttu-id="da384-119">Nome</span><span class="sxs-lookup"><span data-stu-id="da384-119">Name</span></span>       | <span data-ttu-id="da384-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="da384-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="da384-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="da384-121">Authorization</span></span>  | <span data-ttu-id="da384-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da384-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="da384-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="da384-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="da384-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="da384-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da384-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da384-127">Request body</span></span>
<span data-ttu-id="da384-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="da384-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="da384-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da384-131">Property</span></span>     | <span data-ttu-id="da384-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="da384-132">Type</span></span>   |<span data-ttu-id="da384-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="da384-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da384-134">overlay</span><span class="sxs-lookup"><span data-stu-id="da384-134">overlay</span></span>|<span data-ttu-id="da384-135">booliano</span><span class="sxs-lookup"><span data-stu-id="da384-135">boolean</span></span>|<span data-ttu-id="da384-136">Valor booliano que determina se o título do gráfico deve se sobrepor ao gráfico ou não.</span><span class="sxs-lookup"><span data-stu-id="da384-136">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="da384-137">texto</span><span class="sxs-lookup"><span data-stu-id="da384-137">text</span></span>|<span data-ttu-id="da384-138">string</span><span class="sxs-lookup"><span data-stu-id="da384-138">string</span></span>|<span data-ttu-id="da384-139">Representa o texto do título de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="da384-139">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="da384-140">visible</span><span class="sxs-lookup"><span data-stu-id="da384-140">visible</span></span>|<span data-ttu-id="da384-141">booliano</span><span class="sxs-lookup"><span data-stu-id="da384-141">boolean</span></span>|<span data-ttu-id="da384-142">Um valor booliano que representa a visibilidade de um objeto de título de gráfico.</span><span class="sxs-lookup"><span data-stu-id="da384-142">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="da384-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="da384-143">Response</span></span>

<span data-ttu-id="da384-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e o [objeto WorkbookChartTitle](../resources/charttitle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da384-144">If successful, this method returns a `200 OK` response code and updated [WorkbookChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da384-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da384-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da384-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da384-146">Request</span></span>
<span data-ttu-id="da384-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da384-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="da384-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="da384-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
# <a name="c"></a>[<span data-ttu-id="da384-149">C#</span><span class="sxs-lookup"><span data-stu-id="da384-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-charttitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da384-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da384-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-charttitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da384-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da384-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-charttitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da384-152">Java</span><span class="sxs-lookup"><span data-stu-id="da384-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-charttitle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="da384-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="da384-153">Response</span></span>
<span data-ttu-id="da384-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da384-154">Here is an example of the response.</span></span> <span data-ttu-id="da384-155">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="da384-155">Note: The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

