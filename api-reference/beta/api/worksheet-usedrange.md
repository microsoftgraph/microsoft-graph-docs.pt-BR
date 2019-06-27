---
title: 'Worksheet: UsedRange'
description: O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: db61f1ac9533933a83382cd520eb91d690f755fb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269297"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="f3419-104">Worksheet: UsedRange</span><span class="sxs-lookup"><span data-stu-id="f3419-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="f3419-p102">O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.</span><span class="sxs-lookup"><span data-stu-id="f3419-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="f3419-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f3419-107">Permissions</span></span>
<span data-ttu-id="f3419-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3419-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3419-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3419-110">Permission type</span></span>      | <span data-ttu-id="f3419-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3419-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3419-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3419-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f3419-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3419-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f3419-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3419-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3419-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3419-115">Not supported.</span></span>    |
|<span data-ttu-id="f3419-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3419-116">Application</span></span> | <span data-ttu-id="f3419-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3419-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3419-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3419-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/UsedRange

```

## <a name="function-parameters"></a><span data-ttu-id="f3419-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f3419-119">Function parameters</span></span>
<span data-ttu-id="f3419-120">Na URL da solicitação, forneça um parâmetro de consulta opcional.</span><span class="sxs-lookup"><span data-stu-id="f3419-120">In the request URL, provide an optional query parameter.</span></span>

| <span data-ttu-id="f3419-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f3419-121">Parameter</span></span>    | <span data-ttu-id="f3419-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3419-122">Type</span></span>   |<span data-ttu-id="f3419-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3419-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3419-124">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="f3419-124">valuesOnly</span></span>|<span data-ttu-id="f3419-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3419-125">Boolean</span></span>|<span data-ttu-id="f3419-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f3419-126">Optional.</span></span> <span data-ttu-id="f3419-127">Considera apenas as células com valores como células usadas (ignora a formatação).</span><span class="sxs-lookup"><span data-stu-id="f3419-127">Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="f3419-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3419-128">Request headers</span></span>
| <span data-ttu-id="f3419-129">Nome</span><span class="sxs-lookup"><span data-stu-id="f3419-129">Name</span></span>       | <span data-ttu-id="f3419-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3419-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f3419-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3419-131">Authorization</span></span>  | <span data-ttu-id="f3419-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3419-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f3419-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f3419-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="f3419-p106">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f3419-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3419-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3419-137">Request body</span></span>
<span data-ttu-id="f3419-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f3419-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3419-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3419-139">Response</span></span>

<span data-ttu-id="f3419-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3419-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3419-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3419-141">Example</span></span>
<span data-ttu-id="f3419-142">Veja a seguir um exemplo que mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f3419-142">Here is an example that shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f3419-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3419-143">Request</span></span>
<span data-ttu-id="f3419-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3419-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="f3419-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3419-145">Response</span></span>
<span data-ttu-id="f3419-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3419-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f3419-149">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f3419-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f3419-150">C#</span><span class="sxs-lookup"><span data-stu-id="f3419-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/worksheet_usedrange-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f3419-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="f3419-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/worksheet_usedrange-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f3419-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f3419-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/worksheet_usedrange-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-usedrange.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/worksheet-usedrange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/worksheet-usedrange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
