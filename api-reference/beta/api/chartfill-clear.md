---
title: 'ChartFill: clear'
description: Limpe a cor de preenchimento de um elemento do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9630d8d35e12256b7d01c89b996333e5eaefc84e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42439489"
---
# <a name="chartfill-clear"></a><span data-ttu-id="2fb8b-103">ChartFill: clear</span><span class="sxs-lookup"><span data-stu-id="2fb8b-103">ChartFill: clear</span></span>

<span data-ttu-id="2fb8b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2fb8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fb8b-105">Limpe a cor de preenchimento de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="2fb8b-105">Clear the fill color of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="2fb8b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2fb8b-106">Permissions</span></span>
<span data-ttu-id="2fb8b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fb8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fb8b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fb8b-109">Permission type</span></span>      | <span data-ttu-id="2fb8b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2fb8b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fb8b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fb8b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2fb8b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fb8b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2fb8b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fb8b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fb8b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fb8b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2fb8b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fb8b-115">Application</span></span> | <span data-ttu-id="2fb8b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fb8b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fb8b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fb8b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="2fb8b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fb8b-118">Request headers</span></span>
| <span data-ttu-id="2fb8b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2fb8b-119">Name</span></span>       | <span data-ttu-id="2fb8b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fb8b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2fb8b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fb8b-121">Authorization</span></span>  | <span data-ttu-id="2fb8b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fb8b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2fb8b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2fb8b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="2fb8b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2fb8b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fb8b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fb8b-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2fb8b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fb8b-128">Response</span></span>

<span data-ttu-id="2fb8b-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fb8b-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fb8b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fb8b-131">Example</span></span>
<span data-ttu-id="2fb8b-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2fb8b-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2fb8b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fb8b-133">Request</span></span>
<span data-ttu-id="2fb8b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fb8b-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2fb8b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fb8b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartfill_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
```
# <a name="c"></a>[<span data-ttu-id="2fb8b-136">C#</span><span class="sxs-lookup"><span data-stu-id="2fb8b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartfill-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2fb8b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fb8b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartfill-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fb8b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fb8b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartfill-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2fb8b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fb8b-139">Response</span></span>
<span data-ttu-id="2fb8b-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fb8b-140">Here is an example of the response.</span></span> 
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
