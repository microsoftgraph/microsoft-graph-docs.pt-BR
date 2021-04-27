---
title: Atualizar a workbookChartAxis
description: Atualize as propriedades do objeto workbookchartaxis.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 023ae090b3aa303885c606ce2f9ef770d59da947
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047480"
---
# <a name="update-workbookchartaxis"></a><span data-ttu-id="8889a-103">Atualizar a workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="8889a-103">Update workbookChartAxis</span></span>

<span data-ttu-id="8889a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8889a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8889a-105">Atualiza as propriedades do objeto chartaxis.</span><span class="sxs-lookup"><span data-stu-id="8889a-105">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8889a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8889a-106">Permissions</span></span>
<span data-ttu-id="8889a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8889a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8889a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8889a-109">Permission type</span></span>      | <span data-ttu-id="8889a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8889a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8889a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8889a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8889a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8889a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8889a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8889a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8889a-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8889a-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8889a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8889a-115">Application</span></span> | <span data-ttu-id="8889a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8889a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8889a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8889a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="8889a-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="8889a-118">Optional request headers</span></span>
| <span data-ttu-id="8889a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8889a-119">Name</span></span>       | <span data-ttu-id="8889a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8889a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8889a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8889a-121">Authorization</span></span>  | <span data-ttu-id="8889a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8889a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8889a-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8889a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="8889a-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="8889a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8889a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8889a-127">Request body</span></span>
<span data-ttu-id="8889a-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8889a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8889a-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8889a-131">Property</span></span>     | <span data-ttu-id="8889a-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="8889a-132">Type</span></span>   |<span data-ttu-id="8889a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8889a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8889a-134">majorUnit</span><span class="sxs-lookup"><span data-stu-id="8889a-134">majorUnit</span></span>|<span data-ttu-id="8889a-135">Json</span><span class="sxs-lookup"><span data-stu-id="8889a-135">Json</span></span>|<span data-ttu-id="8889a-p105">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="8889a-p105">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="8889a-139">maximum</span><span class="sxs-lookup"><span data-stu-id="8889a-139">maximum</span></span>|<span data-ttu-id="8889a-140">Json</span><span class="sxs-lookup"><span data-stu-id="8889a-140">Json</span></span>|<span data-ttu-id="8889a-p106">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="8889a-p106">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="8889a-144">minimum</span><span class="sxs-lookup"><span data-stu-id="8889a-144">minimum</span></span>|<span data-ttu-id="8889a-145">Json</span><span class="sxs-lookup"><span data-stu-id="8889a-145">Json</span></span>|<span data-ttu-id="8889a-p107">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="8889a-p107">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="8889a-149">minorUnit</span><span class="sxs-lookup"><span data-stu-id="8889a-149">minorUnit</span></span>|<span data-ttu-id="8889a-150">Json</span><span class="sxs-lookup"><span data-stu-id="8889a-150">Json</span></span>|<span data-ttu-id="8889a-p108">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="8889a-p108">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="8889a-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="8889a-154">Response</span></span>

<span data-ttu-id="8889a-155">Se tiver êxito, este método retornará um código de resposta e `200 OK` um objeto [workbookChartAxis](../resources/workbookchartaxis.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8889a-155">If successful, this method returns a `200 OK` response code and updated [workbookChartAxis](../resources/workbookchartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8889a-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8889a-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8889a-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8889a-157">Request</span></span>
<span data-ttu-id="8889a-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8889a-158">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8889a-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="8889a-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartaxis"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```
# <a name="c"></a>[<span data-ttu-id="8889a-160">C#</span><span class="sxs-lookup"><span data-stu-id="8889a-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartaxis-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8889a-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8889a-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartaxis-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8889a-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8889a-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartaxis-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8889a-163">Java</span><span class="sxs-lookup"><span data-stu-id="8889a-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartaxis-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8889a-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="8889a-164">Response</span></span>
<span data-ttu-id="8889a-165">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8889a-165">Here is an example of the response.</span></span> <span data-ttu-id="8889a-166">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8889a-166">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxis"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartaxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


