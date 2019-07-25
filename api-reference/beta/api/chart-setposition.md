---
title: 'Chart: setPosition'
description: Posiciona o gráfico em relação às células na planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ce5b93e7a5d26facf84aa1c06c32f517ed90af2b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864259"
---
# <a name="chart-setposition"></a><span data-ttu-id="826dc-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="826dc-103">Chart: setPosition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="826dc-104">Posiciona o gráfico em relação às células na planilha.</span><span class="sxs-lookup"><span data-stu-id="826dc-104">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="826dc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="826dc-105">Permissions</span></span>
<span data-ttu-id="826dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="826dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="826dc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="826dc-108">Permission type</span></span>      | <span data-ttu-id="826dc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="826dc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="826dc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="826dc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="826dc-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="826dc-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="826dc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="826dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="826dc-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="826dc-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="826dc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="826dc-114">Application</span></span> | <span data-ttu-id="826dc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="826dc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="826dc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="826dc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="826dc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="826dc-117">Request headers</span></span>
| <span data-ttu-id="826dc-118">Nome</span><span class="sxs-lookup"><span data-stu-id="826dc-118">Name</span></span>       | <span data-ttu-id="826dc-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="826dc-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="826dc-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="826dc-120">Authorization</span></span>  | <span data-ttu-id="826dc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="826dc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="826dc-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="826dc-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="826dc-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="826dc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="826dc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="826dc-126">Request body</span></span>
<span data-ttu-id="826dc-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="826dc-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="826dc-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="826dc-128">Parameter</span></span>    | <span data-ttu-id="826dc-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="826dc-129">Type</span></span>   |<span data-ttu-id="826dc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="826dc-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="826dc-131">startCell</span><span class="sxs-lookup"><span data-stu-id="826dc-131">startCell</span></span>|<span data-ttu-id="826dc-132">string</span><span class="sxs-lookup"><span data-stu-id="826dc-132">string</span></span>|<span data-ttu-id="826dc-p104">A célula inicial. Esse é o local para o qual o gráfico será movido. A célula inicial é a célula superior esquerda ou direita, dependendo das configurações de exibição do usuário, da esquerda para a direita.</span><span class="sxs-lookup"><span data-stu-id="826dc-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="826dc-136">endCell</span><span class="sxs-lookup"><span data-stu-id="826dc-136">endCell</span></span>|<span data-ttu-id="826dc-137">string</span><span class="sxs-lookup"><span data-stu-id="826dc-137">string</span></span>|<span data-ttu-id="826dc-p105">Opcional. A célula final. Quando é especificada, a altura e a largura do gráfico são definidas para cobrirem totalmente essa célula ou intervalo.</span><span class="sxs-lookup"><span data-stu-id="826dc-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="826dc-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="826dc-141">Response</span></span>

<span data-ttu-id="826dc-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="826dc-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="826dc-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="826dc-144">Example</span></span>
<span data-ttu-id="826dc-145">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="826dc-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="826dc-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="826dc-146">Request</span></span>
<span data-ttu-id="826dc-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="826dc-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="826dc-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="826dc-148">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="826dc-149">C#</span><span class="sxs-lookup"><span data-stu-id="826dc-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chart-setposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="826dc-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="826dc-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chart-setposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="826dc-151">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="826dc-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chart-setposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="826dc-152">Java</span><span class="sxs-lookup"><span data-stu-id="826dc-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chart-setposition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="826dc-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="826dc-153">Response</span></span>
<span data-ttu-id="826dc-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="826dc-154">Here is an example of the response.</span></span> 
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
