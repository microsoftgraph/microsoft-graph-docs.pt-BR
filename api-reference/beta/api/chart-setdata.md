---
title: 'Chart: setData'
description: Redefine os dados de origem do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5aa0d5a4584a8dafb105e9f64865a135229d3e0d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958972"
---
# <a name="chart-setdata"></a><span data-ttu-id="dae87-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="dae87-103">Chart: setData</span></span>

<span data-ttu-id="dae87-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dae87-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dae87-105">Redefine os dados de origem do gráfico.</span><span class="sxs-lookup"><span data-stu-id="dae87-105">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="dae87-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dae87-106">Permissions</span></span>
<span data-ttu-id="dae87-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dae87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dae87-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dae87-109">Permission type</span></span>      | <span data-ttu-id="dae87-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dae87-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dae87-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dae87-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dae87-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dae87-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dae87-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dae87-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dae87-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dae87-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dae87-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dae87-115">Application</span></span> | <span data-ttu-id="dae87-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dae87-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dae87-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dae87-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setData

```
## <a name="request-headers"></a><span data-ttu-id="dae87-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dae87-118">Request headers</span></span>
| <span data-ttu-id="dae87-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dae87-119">Name</span></span>       | <span data-ttu-id="dae87-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dae87-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dae87-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dae87-121">Authorization</span></span>  | <span data-ttu-id="dae87-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dae87-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dae87-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dae87-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="dae87-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="dae87-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dae87-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dae87-127">Request body</span></span>
<span data-ttu-id="dae87-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dae87-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dae87-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dae87-129">Parameter</span></span>    | <span data-ttu-id="dae87-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dae87-130">Type</span></span>   |<span data-ttu-id="dae87-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dae87-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dae87-132">sourceData</span><span class="sxs-lookup"><span data-stu-id="dae87-132">sourceData</span></span>|<span data-ttu-id="dae87-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dae87-133">string</span></span>|<span data-ttu-id="dae87-134">O objeto Range que corresponde aos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="dae87-134">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="dae87-135">seriesBy</span><span class="sxs-lookup"><span data-stu-id="dae87-135">seriesBy</span></span>|<span data-ttu-id="dae87-136">string</span><span class="sxs-lookup"><span data-stu-id="dae87-136">string</span></span>|<span data-ttu-id="dae87-p104">Opcional. Especifica a forma como as colunas ou linhas são usadas como série de dados no gráfico. Pode ser um dos seguintes: automático (padrão), linhas ou colunas.  Os valores possíveis são: `Auto`, `Columns` e `Rows`.</span><span class="sxs-lookup"><span data-stu-id="dae87-p104">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="dae87-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="dae87-141">Response</span></span>

<span data-ttu-id="dae87-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dae87-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dae87-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dae87-144">Example</span></span>
<span data-ttu-id="dae87-145">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="dae87-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dae87-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dae87-146">Request</span></span>
<span data-ttu-id="dae87-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dae87-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dae87-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="dae87-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```
# <a name="c"></a>[<span data-ttu-id="dae87-149">C#</span><span class="sxs-lookup"><span data-stu-id="dae87-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chart-setdata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dae87-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dae87-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chart-setdata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dae87-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dae87-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chart-setdata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dae87-152">Java</span><span class="sxs-lookup"><span data-stu-id="dae87-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chart-setdata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dae87-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="dae87-153">Response</span></span>
<span data-ttu-id="dae87-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dae87-154">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


