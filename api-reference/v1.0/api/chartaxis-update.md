---
title: Atualizar chartaxis
description: Atualiza as propriedades do objeto chartaxis.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 515f342a84d031cd5e32566abee942447154bac9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003683"
---
# <a name="update-chartaxis"></a><span data-ttu-id="8fbcb-103">Atualizar chartaxis</span><span class="sxs-lookup"><span data-stu-id="8fbcb-103">Update chartaxis</span></span>

<span data-ttu-id="8fbcb-104">Atualiza as propriedades do objeto chartaxis.</span><span class="sxs-lookup"><span data-stu-id="8fbcb-104">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8fbcb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8fbcb-105">Permissions</span></span>
<span data-ttu-id="8fbcb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fbcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fbcb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8fbcb-108">Permission type</span></span>      | <span data-ttu-id="8fbcb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8fbcb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fbcb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8fbcb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8fbcb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8fbcb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8fbcb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8fbcb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fbcb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fbcb-113">Not supported.</span></span>    |
|<span data-ttu-id="8fbcb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8fbcb-114">Application</span></span> | <span data-ttu-id="8fbcb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fbcb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8fbcb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8fbcb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="8fbcb-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="8fbcb-117">Optional request headers</span></span>
| <span data-ttu-id="8fbcb-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8fbcb-118">Name</span></span>       | <span data-ttu-id="8fbcb-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fbcb-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8fbcb-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8fbcb-120">Authorization</span></span>  | <span data-ttu-id="8fbcb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8fbcb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8fbcb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8fbcb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8fbcb-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="8fbcb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fbcb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8fbcb-126">Request body</span></span>
<span data-ttu-id="8fbcb-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8fbcb-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8fbcb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8fbcb-130">Property</span></span>     | <span data-ttu-id="8fbcb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8fbcb-131">Type</span></span>   |<span data-ttu-id="8fbcb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fbcb-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fbcb-133">majorUnit</span><span class="sxs-lookup"><span data-stu-id="8fbcb-133">majorUnit</span></span>|<span data-ttu-id="8fbcb-134">Json</span><span class="sxs-lookup"><span data-stu-id="8fbcb-134">Json</span></span>|<span data-ttu-id="8fbcb-p105">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="8fbcb-p105">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="8fbcb-138">maximum</span><span class="sxs-lookup"><span data-stu-id="8fbcb-138">maximum</span></span>|<span data-ttu-id="8fbcb-139">Json</span><span class="sxs-lookup"><span data-stu-id="8fbcb-139">Json</span></span>|<span data-ttu-id="8fbcb-p106">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="8fbcb-p106">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="8fbcb-143">minimum</span><span class="sxs-lookup"><span data-stu-id="8fbcb-143">minimum</span></span>|<span data-ttu-id="8fbcb-144">Json</span><span class="sxs-lookup"><span data-stu-id="8fbcb-144">Json</span></span>|<span data-ttu-id="8fbcb-p107">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="8fbcb-p107">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="8fbcb-148">minorUnit</span><span class="sxs-lookup"><span data-stu-id="8fbcb-148">minorUnit</span></span>|<span data-ttu-id="8fbcb-149">Json</span><span class="sxs-lookup"><span data-stu-id="8fbcb-149">Json</span></span>|<span data-ttu-id="8fbcb-p108">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="8fbcb-p108">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="8fbcb-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fbcb-153">Response</span></span>

<span data-ttu-id="8fbcb-154">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookChartAxis](../resources/chartaxis.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8fbcb-154">If successful, this method returns a `200 OK` response code and updated [WorkbookChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8fbcb-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8fbcb-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8fbcb-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8fbcb-156">Request</span></span>
<span data-ttu-id="8fbcb-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8fbcb-157">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8fbcb-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="8fbcb-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartaxis"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8fbcb-159">C#</span><span class="sxs-lookup"><span data-stu-id="8fbcb-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartaxis-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8fbcb-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="8fbcb-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartaxis-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8fbcb-161">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8fbcb-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartaxis-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8fbcb-162">Java</span><span class="sxs-lookup"><span data-stu-id="8fbcb-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartaxis-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8fbcb-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fbcb-163">Response</span></span>
<span data-ttu-id="8fbcb-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8fbcb-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
