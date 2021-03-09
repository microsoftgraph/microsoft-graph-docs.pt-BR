---
title: 'Chart: setPosition'
description: Posiciona o gráfico em relação às células na planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9e59d5c85779758cb2e4d02e3693d9cdeec345f6
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574759"
---
# <a name="chart-setposition"></a><span data-ttu-id="ba1e4-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="ba1e4-103">Chart: setPosition</span></span>

<span data-ttu-id="ba1e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba1e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba1e4-105">Posiciona o gráfico em relação às células na planilha.</span><span class="sxs-lookup"><span data-stu-id="ba1e4-105">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="ba1e4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba1e4-106">Permissions</span></span>
<span data-ttu-id="ba1e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba1e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba1e4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba1e4-109">Permission type</span></span>      | <span data-ttu-id="ba1e4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba1e4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba1e4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba1e4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ba1e4-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba1e4-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ba1e4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba1e4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba1e4-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba1e4-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ba1e4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba1e4-115">Application</span></span> | <span data-ttu-id="ba1e4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba1e4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba1e4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba1e4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="ba1e4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba1e4-118">Request headers</span></span>
| <span data-ttu-id="ba1e4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ba1e4-119">Name</span></span>       | <span data-ttu-id="ba1e4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba1e4-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ba1e4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba1e4-121">Authorization</span></span>  | <span data-ttu-id="ba1e4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba1e4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ba1e4-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ba1e4-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="ba1e4-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ba1e4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba1e4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba1e4-127">Request body</span></span>
<span data-ttu-id="ba1e4-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba1e4-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ba1e4-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ba1e4-129">Parameter</span></span>    | <span data-ttu-id="ba1e4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba1e4-130">Type</span></span>   |<span data-ttu-id="ba1e4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba1e4-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba1e4-132">startCell</span><span class="sxs-lookup"><span data-stu-id="ba1e4-132">startCell</span></span>|<span data-ttu-id="ba1e4-133">string</span><span class="sxs-lookup"><span data-stu-id="ba1e4-133">string</span></span>|<span data-ttu-id="ba1e4-p104">A célula inicial. Esse é o local para o qual o gráfico será movido. A célula inicial é a célula superior esquerda ou direita, dependendo das configurações de exibição do usuário, da esquerda para a direita.</span><span class="sxs-lookup"><span data-stu-id="ba1e4-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="ba1e4-137">endCell</span><span class="sxs-lookup"><span data-stu-id="ba1e4-137">endCell</span></span>|<span data-ttu-id="ba1e4-138">string</span><span class="sxs-lookup"><span data-stu-id="ba1e4-138">string</span></span>|<span data-ttu-id="ba1e4-p105">Opcional. A célula final. Quando é especificada, a altura e a largura do gráfico são definidas para cobrirem totalmente essa célula ou intervalo.</span><span class="sxs-lookup"><span data-stu-id="ba1e4-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="ba1e4-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba1e4-142">Response</span></span>

<span data-ttu-id="ba1e4-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba1e4-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba1e4-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba1e4-145">Example</span></span>
<span data-ttu-id="ba1e4-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ba1e4-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ba1e4-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba1e4-147">Request</span></span>
<span data-ttu-id="ba1e4-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba1e4-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ba1e4-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba1e4-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```
# <a name="c"></a>[<span data-ttu-id="ba1e4-150">C#</span><span class="sxs-lookup"><span data-stu-id="ba1e4-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chart-setposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba1e4-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba1e4-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chart-setposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba1e4-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba1e4-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chart-setposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba1e4-153">Java</span><span class="sxs-lookup"><span data-stu-id="ba1e4-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chart-setposition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ba1e4-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba1e4-154">Response</span></span>
<span data-ttu-id="ba1e4-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba1e4-155">Here is an example of the response.</span></span> 
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
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


