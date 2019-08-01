---
title: 'ChartLineFormat: clear'
description: Limpe a formatação da linha de um elemento do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d7db49aa6f20914c51eddc7ea0990843140d77b6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003473"
---
# <a name="chartlineformat-clear"></a><span data-ttu-id="e9d38-103">ChartLineFormat: clear</span><span class="sxs-lookup"><span data-stu-id="e9d38-103">ChartLineFormat: clear</span></span>

<span data-ttu-id="e9d38-104">Limpe a formatação da linha de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="e9d38-104">Clear the line format of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="e9d38-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9d38-105">Permissions</span></span>
<span data-ttu-id="e9d38-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9d38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9d38-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9d38-108">Permission type</span></span>      | <span data-ttu-id="e9d38-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9d38-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9d38-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9d38-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e9d38-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9d38-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e9d38-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9d38-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9d38-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9d38-113">Not supported.</span></span>    |
|<span data-ttu-id="e9d38-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9d38-114">Application</span></span> | <span data-ttu-id="e9d38-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9d38-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9d38-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9d38-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorgridlines/format/line/clear

```
## <a name="request-headers"></a><span data-ttu-id="e9d38-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9d38-117">Request headers</span></span>
| <span data-ttu-id="e9d38-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e9d38-118">Name</span></span>       | <span data-ttu-id="e9d38-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9d38-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e9d38-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9d38-120">Authorization</span></span>  | <span data-ttu-id="e9d38-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9d38-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9d38-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e9d38-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e9d38-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e9d38-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9d38-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9d38-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e9d38-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9d38-127">Response</span></span>

<span data-ttu-id="e9d38-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9d38-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9d38-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9d38-130">Example</span></span>
<span data-ttu-id="e9d38-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e9d38-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e9d38-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9d38-132">Request</span></span>
<span data-ttu-id="e9d38-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9d38-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e9d38-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9d38-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartlineformat_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e9d38-135">C#</span><span class="sxs-lookup"><span data-stu-id="e9d38-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartlineformat-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9d38-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="e9d38-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartlineformat-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e9d38-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e9d38-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartlineformat-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e9d38-138">Java</span><span class="sxs-lookup"><span data-stu-id="e9d38-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartlineformat-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e9d38-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9d38-139">Response</span></span>
<span data-ttu-id="e9d38-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9d38-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
