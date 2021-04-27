---
title: Atualizar chartseries
description: Atualiza as propriedades do objeto chartseries.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d2c791b7211cf83fbc323963d4aaa387fd1f1098
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047326"
---
# <a name="update-chartseries"></a><span data-ttu-id="d142b-103">Atualizar chartseries</span><span class="sxs-lookup"><span data-stu-id="d142b-103">Update chartseries</span></span>

<span data-ttu-id="d142b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d142b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d142b-105">Atualiza as propriedades do objeto chartseries.</span><span class="sxs-lookup"><span data-stu-id="d142b-105">Update the properties of chartseries object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d142b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d142b-106">Permissions</span></span>
<span data-ttu-id="d142b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d142b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d142b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d142b-109">Permission type</span></span>      | <span data-ttu-id="d142b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d142b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d142b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d142b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d142b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d142b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d142b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d142b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d142b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d142b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d142b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d142b-115">Application</span></span> | <span data-ttu-id="d142b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d142b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d142b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d142b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}
```
## <a name="optional-request-headers"></a><span data-ttu-id="d142b-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="d142b-118">Optional request headers</span></span>
| <span data-ttu-id="d142b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d142b-119">Name</span></span>       | <span data-ttu-id="d142b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d142b-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d142b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d142b-121">Authorization</span></span>  | <span data-ttu-id="d142b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d142b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d142b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d142b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="d142b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d142b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d142b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d142b-127">Request body</span></span>
<span data-ttu-id="d142b-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d142b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d142b-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d142b-131">Property</span></span>     | <span data-ttu-id="d142b-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d142b-132">Type</span></span>   |<span data-ttu-id="d142b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d142b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d142b-134">nome</span><span class="sxs-lookup"><span data-stu-id="d142b-134">name</span></span>|<span data-ttu-id="d142b-135">string</span><span class="sxs-lookup"><span data-stu-id="d142b-135">string</span></span>|<span data-ttu-id="d142b-136">Representa o nome de uma série em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="d142b-136">Represents the name of a series in a chart.</span></span>|

## <a name="response"></a><span data-ttu-id="d142b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d142b-137">Response</span></span>

<span data-ttu-id="d142b-138">Se tiver êxito, este método retornará um código de resposta e `200 OK` um objeto [workbookChartSeries](../resources/workbookchartseries.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d142b-138">If successful, this method returns a `200 OK` response code and updated [workbookChartSeries](../resources/workbookchartseries.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d142b-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d142b-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d142b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d142b-140">Request</span></span>
<span data-ttu-id="d142b-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d142b-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d142b-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="d142b-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartseries"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
# <a name="c"></a>[<span data-ttu-id="d142b-143">C#</span><span class="sxs-lookup"><span data-stu-id="d142b-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartseries-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d142b-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d142b-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartseries-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d142b-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d142b-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartseries-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d142b-146">Java</span><span class="sxs-lookup"><span data-stu-id="d142b-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartseries-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d142b-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="d142b-147">Response</span></span>
<span data-ttu-id="d142b-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d142b-148">Here is an example of the response.</span></span> <span data-ttu-id="d142b-149">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d142b-149">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartseries",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


