---
title: 'ChartLineFormat: clear'
description: Limpe a formatação da linha de um elemento do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 82de6a4e424490d6d7e9b332232d6890e8c7471c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958580"
---
# <a name="chartlineformat-clear"></a><span data-ttu-id="49c2b-103">ChartLineFormat: clear</span><span class="sxs-lookup"><span data-stu-id="49c2b-103">ChartLineFormat: clear</span></span>

<span data-ttu-id="49c2b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49c2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49c2b-105">Limpe a formatação da linha de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="49c2b-105">Clear the line format of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="49c2b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="49c2b-106">Permissions</span></span>
<span data-ttu-id="49c2b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49c2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49c2b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49c2b-109">Permission type</span></span>      | <span data-ttu-id="49c2b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49c2b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49c2b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49c2b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="49c2b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49c2b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="49c2b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49c2b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49c2b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49c2b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="49c2b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49c2b-115">Application</span></span> | <span data-ttu-id="49c2b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49c2b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49c2b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49c2b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/majorgridlines/format/line/clear

```
## <a name="request-headers"></a><span data-ttu-id="49c2b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49c2b-118">Request headers</span></span>
| <span data-ttu-id="49c2b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="49c2b-119">Name</span></span>       | <span data-ttu-id="49c2b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="49c2b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="49c2b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="49c2b-121">Authorization</span></span>  | <span data-ttu-id="49c2b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49c2b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49c2b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="49c2b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="49c2b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="49c2b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49c2b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49c2b-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="49c2b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="49c2b-128">Response</span></span>

<span data-ttu-id="49c2b-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49c2b-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49c2b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49c2b-131">Example</span></span>
<span data-ttu-id="49c2b-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="49c2b-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="49c2b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49c2b-133">Request</span></span>
<span data-ttu-id="49c2b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49c2b-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49c2b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="49c2b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartlineformat_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line/clear
```
# <a name="c"></a>[<span data-ttu-id="49c2b-136">C#</span><span class="sxs-lookup"><span data-stu-id="49c2b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartlineformat-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49c2b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49c2b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartlineformat-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49c2b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49c2b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartlineformat-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49c2b-139">Java</span><span class="sxs-lookup"><span data-stu-id="49c2b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartlineformat-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="49c2b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="49c2b-140">Response</span></span>
<span data-ttu-id="49c2b-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49c2b-141">Here is an example of the response.</span></span> 
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
  "description": "ChartLineFormat: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


