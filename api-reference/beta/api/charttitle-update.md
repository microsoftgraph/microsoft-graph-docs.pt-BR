---
title: Atualizar charttitle
description: Atualiza as propriedades do objeto charttitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b1b5d1b60d68e12634cd069aa02fe70b435bd0b6
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574296"
---
# <a name="update-charttitle"></a><span data-ttu-id="f0731-103">Atualizar charttitle</span><span class="sxs-lookup"><span data-stu-id="f0731-103">Update charttitle</span></span>

<span data-ttu-id="f0731-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0731-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0731-105">Atualiza as propriedades do objeto charttitle.</span><span class="sxs-lookup"><span data-stu-id="f0731-105">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f0731-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0731-106">Permissions</span></span>
<span data-ttu-id="f0731-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0731-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0731-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0731-109">Permission type</span></span>      | <span data-ttu-id="f0731-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0731-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0731-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0731-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f0731-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0731-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f0731-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0731-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0731-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0731-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f0731-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0731-115">Application</span></span> | <span data-ttu-id="f0731-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0731-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0731-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0731-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="f0731-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="f0731-118">Optional request headers</span></span>
| <span data-ttu-id="f0731-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f0731-119">Name</span></span>       | <span data-ttu-id="f0731-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0731-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f0731-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0731-121">Authorization</span></span>  | <span data-ttu-id="f0731-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0731-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0731-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f0731-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="f0731-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f0731-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0731-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0731-127">Request body</span></span>
<span data-ttu-id="f0731-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f0731-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f0731-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0731-131">Property</span></span>     | <span data-ttu-id="f0731-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0731-132">Type</span></span>   |<span data-ttu-id="f0731-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0731-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0731-134">overlay</span><span class="sxs-lookup"><span data-stu-id="f0731-134">overlay</span></span>|<span data-ttu-id="f0731-135">booliano</span><span class="sxs-lookup"><span data-stu-id="f0731-135">boolean</span></span>|<span data-ttu-id="f0731-136">Valor booliano que determina se o título do gráfico deve se sobrepor ao gráfico ou não.</span><span class="sxs-lookup"><span data-stu-id="f0731-136">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="f0731-137">texto</span><span class="sxs-lookup"><span data-stu-id="f0731-137">text</span></span>|<span data-ttu-id="f0731-138">string</span><span class="sxs-lookup"><span data-stu-id="f0731-138">string</span></span>|<span data-ttu-id="f0731-139">Representa o texto do título de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="f0731-139">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="f0731-140">visible</span><span class="sxs-lookup"><span data-stu-id="f0731-140">visible</span></span>|<span data-ttu-id="f0731-141">booliano</span><span class="sxs-lookup"><span data-stu-id="f0731-141">boolean</span></span>|<span data-ttu-id="f0731-142">Um valor booliano que representa a visibilidade de um objeto de título de gráfico.</span><span class="sxs-lookup"><span data-stu-id="f0731-142">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="f0731-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0731-143">Response</span></span>

<span data-ttu-id="f0731-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [workbookChartTitle](../resources/workbookcharttitle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0731-144">If successful, this method returns a `200 OK` response code and updated [workbookChartTitle](../resources/workbookcharttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0731-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0731-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0731-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0731-146">Request</span></span>
<span data-ttu-id="f0731-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0731-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f0731-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0731-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f0731-149">C#</span><span class="sxs-lookup"><span data-stu-id="f0731-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-charttitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0731-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0731-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-charttitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0731-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0731-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-charttitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0731-152">Java</span><span class="sxs-lookup"><span data-stu-id="f0731-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-charttitle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f0731-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0731-153">Response</span></span>
<span data-ttu-id="f0731-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0731-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


