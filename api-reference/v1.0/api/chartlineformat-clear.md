---
title: 'ChartLineFormat: clear'
description: Limpe a formatação da linha de um elemento do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d8f720ea49309921cb19727f74817a3c782bb3f0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272391"
---
# <a name="chartlineformat-clear"></a><span data-ttu-id="227ce-103">ChartLineFormat: clear</span><span class="sxs-lookup"><span data-stu-id="227ce-103">ChartLineFormat: clear</span></span>

<span data-ttu-id="227ce-104">Limpe a formatação da linha de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="227ce-104">Clear the line format of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="227ce-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="227ce-105">Permissions</span></span>
<span data-ttu-id="227ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="227ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="227ce-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="227ce-108">Permission type</span></span>      | <span data-ttu-id="227ce-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="227ce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="227ce-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="227ce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="227ce-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="227ce-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="227ce-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="227ce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="227ce-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="227ce-113">Not supported.</span></span>    |
|<span data-ttu-id="227ce-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="227ce-114">Application</span></span> | <span data-ttu-id="227ce-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="227ce-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="227ce-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="227ce-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorgridlines/format/line/clear

```
## <a name="request-headers"></a><span data-ttu-id="227ce-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="227ce-117">Request headers</span></span>
| <span data-ttu-id="227ce-118">Nome</span><span class="sxs-lookup"><span data-stu-id="227ce-118">Name</span></span>       | <span data-ttu-id="227ce-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="227ce-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="227ce-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="227ce-120">Authorization</span></span>  | <span data-ttu-id="227ce-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="227ce-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="227ce-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="227ce-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="227ce-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="227ce-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="227ce-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="227ce-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="227ce-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="227ce-127">Response</span></span>

<span data-ttu-id="227ce-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="227ce-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="227ce-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="227ce-130">Example</span></span>
<span data-ttu-id="227ce-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="227ce-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="227ce-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="227ce-132">Request</span></span>
<span data-ttu-id="227ce-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="227ce-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartlineformat_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line/clear
```

##### <a name="response"></a><span data-ttu-id="227ce-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="227ce-134">Response</span></span>
<span data-ttu-id="227ce-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="227ce-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="227ce-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="227ce-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="227ce-137">C#</span><span class="sxs-lookup"><span data-stu-id="227ce-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/chartlineformat_clear-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="227ce-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="227ce-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/chartlineformat_clear-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="227ce-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="227ce-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/chartlineformat_clear-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/chartlineformat-clear.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/chartlineformat-clear.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/chartlineformat-clear.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
