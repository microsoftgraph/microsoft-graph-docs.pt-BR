---
title: Atualizar workbookChartAxis
description: Atualize as propriedades do objeto workbookchartaxis.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 69061badcdf8827322f664a50d9c6270604ab032
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958888"
---
# <a name="update-workbookchartaxis"></a><span data-ttu-id="5f7e3-103">Atualizar workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="5f7e3-103">Update workbookChartAxis</span></span>

<span data-ttu-id="5f7e3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f7e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f7e3-105">Atualiza as propriedades do objeto chartaxis.</span><span class="sxs-lookup"><span data-stu-id="5f7e3-105">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5f7e3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f7e3-106">Permissions</span></span>
<span data-ttu-id="5f7e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f7e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f7e3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f7e3-109">Permission type</span></span>      | <span data-ttu-id="5f7e3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f7e3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f7e3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f7e3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5f7e3-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f7e3-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5f7e3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f7e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f7e3-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f7e3-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5f7e3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f7e3-115">Application</span></span> | <span data-ttu-id="5f7e3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f7e3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f7e3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f7e3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="5f7e3-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="5f7e3-118">Optional request headers</span></span>
| <span data-ttu-id="5f7e3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5f7e3-119">Name</span></span>       | <span data-ttu-id="5f7e3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f7e3-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5f7e3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f7e3-121">Authorization</span></span>  | <span data-ttu-id="5f7e3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f7e3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f7e3-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5f7e3-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="5f7e3-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5f7e3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f7e3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f7e3-127">Request body</span></span>
<span data-ttu-id="5f7e3-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5f7e3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5f7e3-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f7e3-131">Property</span></span>     | <span data-ttu-id="5f7e3-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f7e3-132">Type</span></span>   |<span data-ttu-id="5f7e3-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f7e3-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f7e3-134">majorUnit</span><span class="sxs-lookup"><span data-stu-id="5f7e3-134">majorUnit</span></span>|<span data-ttu-id="5f7e3-135">Json</span><span class="sxs-lookup"><span data-stu-id="5f7e3-135">Json</span></span>|<span data-ttu-id="5f7e3-p105">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="5f7e3-p105">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="5f7e3-139">maximum</span><span class="sxs-lookup"><span data-stu-id="5f7e3-139">maximum</span></span>|<span data-ttu-id="5f7e3-140">Json</span><span class="sxs-lookup"><span data-stu-id="5f7e3-140">Json</span></span>|<span data-ttu-id="5f7e3-p106">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="5f7e3-p106">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="5f7e3-144">minimum</span><span class="sxs-lookup"><span data-stu-id="5f7e3-144">minimum</span></span>|<span data-ttu-id="5f7e3-145">Json</span><span class="sxs-lookup"><span data-stu-id="5f7e3-145">Json</span></span>|<span data-ttu-id="5f7e3-p107">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="5f7e3-p107">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="5f7e3-149">minorUnit</span><span class="sxs-lookup"><span data-stu-id="5f7e3-149">minorUnit</span></span>|<span data-ttu-id="5f7e3-150">Json</span><span class="sxs-lookup"><span data-stu-id="5f7e3-150">Json</span></span>|<span data-ttu-id="5f7e3-p108">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="5f7e3-p108">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="5f7e3-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f7e3-154">Response</span></span>

<span data-ttu-id="5f7e3-155">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookChartAxis](../resources/workbookchartaxis.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f7e3-155">If successful, this method returns a `200 OK` response code and updated [workbookChartAxis](../resources/workbookchartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5f7e3-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f7e3-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5f7e3-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f7e3-157">Request</span></span>
<span data-ttu-id="5f7e3-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f7e3-158">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5f7e3-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f7e3-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5f7e3-160">C#</span><span class="sxs-lookup"><span data-stu-id="5f7e3-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartaxis-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f7e3-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f7e3-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartaxis-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f7e3-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f7e3-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartaxis-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f7e3-163">Java</span><span class="sxs-lookup"><span data-stu-id="5f7e3-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartaxis-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5f7e3-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f7e3-164">Response</span></span>
<span data-ttu-id="5f7e3-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f7e3-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


