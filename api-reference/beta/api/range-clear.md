---
title: 'Range: clear'
description: Limpa valores de intervalo, formatação, preenchimento, borda, etc.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2f0755416fd36a76c938b3a45cc1534011a2dbd8
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412310"
---
# <a name="range-clear"></a><span data-ttu-id="05426-103">Range: clear</span><span class="sxs-lookup"><span data-stu-id="05426-103">Range: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05426-104">Limpa valores de intervalo, formatação, preenchimento, borda, etc.</span><span class="sxs-lookup"><span data-stu-id="05426-104">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="05426-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="05426-105">Permissions</span></span>
<span data-ttu-id="05426-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05426-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05426-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05426-108">Permission type</span></span>      | <span data-ttu-id="05426-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05426-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05426-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05426-110">Delegated (work or school account)</span></span> | <span data-ttu-id="05426-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05426-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="05426-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05426-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05426-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05426-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="05426-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05426-114">Application</span></span> | <span data-ttu-id="05426-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05426-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="05426-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05426-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="05426-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05426-117">Request headers</span></span>
| <span data-ttu-id="05426-118">Nome</span><span class="sxs-lookup"><span data-stu-id="05426-118">Name</span></span>       | <span data-ttu-id="05426-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="05426-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="05426-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="05426-120">Authorization</span></span>  | <span data-ttu-id="05426-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05426-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="05426-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="05426-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="05426-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="05426-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="05426-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05426-126">Request body</span></span>
<span data-ttu-id="05426-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05426-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="05426-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="05426-128">Parameter</span></span>    | <span data-ttu-id="05426-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="05426-129">Type</span></span>   |<span data-ttu-id="05426-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="05426-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05426-131">applyTo</span><span class="sxs-lookup"><span data-stu-id="05426-131">applyTo</span></span>|<span data-ttu-id="05426-132">string</span><span class="sxs-lookup"><span data-stu-id="05426-132">string</span></span>|<span data-ttu-id="05426-p104">Opcional. Determina o tipo de ação de limpeza.  Os valores possíveis são: `All`, `Formats` e `Contents`.</span><span class="sxs-lookup"><span data-stu-id="05426-p104">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="05426-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="05426-136">Response</span></span>

<span data-ttu-id="05426-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05426-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05426-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05426-139">Example</span></span>
<span data-ttu-id="05426-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="05426-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="05426-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05426-141">Request</span></span>
<span data-ttu-id="05426-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05426-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="05426-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="05426-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="05426-144">C#</span><span class="sxs-lookup"><span data-stu-id="05426-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="05426-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05426-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="05426-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="05426-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="05426-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="05426-147">Response</span></span>
<span data-ttu-id="05426-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05426-148">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
