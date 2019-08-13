---
title: 'ChartFill: clear'
description: Limpe a cor de preenchimento de um elemento do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 36ad1d8d2d79fa9f1873ccc83f6001659162e2a4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317183"
---
# <a name="chartfill-clear"></a><span data-ttu-id="8babd-103">ChartFill: clear</span><span class="sxs-lookup"><span data-stu-id="8babd-103">ChartFill: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8babd-104">Limpe a cor de preenchimento de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="8babd-104">Clear the fill color of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="8babd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8babd-105">Permissions</span></span>
<span data-ttu-id="8babd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8babd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8babd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8babd-108">Permission type</span></span>      | <span data-ttu-id="8babd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8babd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8babd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8babd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8babd-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8babd-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8babd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8babd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8babd-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8babd-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8babd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8babd-114">Application</span></span> | <span data-ttu-id="8babd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8babd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8babd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8babd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="8babd-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8babd-117">Request headers</span></span>
| <span data-ttu-id="8babd-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8babd-118">Name</span></span>       | <span data-ttu-id="8babd-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8babd-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8babd-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8babd-120">Authorization</span></span>  | <span data-ttu-id="8babd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8babd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8babd-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8babd-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8babd-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="8babd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8babd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8babd-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8babd-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8babd-127">Response</span></span>

<span data-ttu-id="8babd-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8babd-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8babd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8babd-130">Example</span></span>
<span data-ttu-id="8babd-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8babd-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8babd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8babd-132">Request</span></span>
<span data-ttu-id="8babd-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8babd-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8babd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8babd-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartfill_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8babd-135">C#</span><span class="sxs-lookup"><span data-stu-id="8babd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartfill-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8babd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8babd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartfill-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8babd-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8babd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartfill-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8babd-138">Java</span><span class="sxs-lookup"><span data-stu-id="8babd-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartfill-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8babd-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8babd-139">Response</span></span>
<span data-ttu-id="8babd-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8babd-140">Here is an example of the response.</span></span> 
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
  "description": "ChartFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
