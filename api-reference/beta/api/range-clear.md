---
title: 'Range: clear'
description: Limpa valores de intervalo, formatação, preenchimento, borda, etc.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 17fb072aad04678cc3ff7378b968b2ee81d79ea9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978483"
---
# <a name="range-clear"></a><span data-ttu-id="66757-103">Range: clear</span><span class="sxs-lookup"><span data-stu-id="66757-103">Range: clear</span></span>

<span data-ttu-id="66757-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66757-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66757-105">Limpa valores de intervalo, formatação, preenchimento, borda, etc.</span><span class="sxs-lookup"><span data-stu-id="66757-105">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="66757-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="66757-106">Permissions</span></span>
<span data-ttu-id="66757-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66757-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66757-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66757-109">Permission type</span></span>      | <span data-ttu-id="66757-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66757-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66757-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66757-111">Delegated (work or school account)</span></span> | <span data-ttu-id="66757-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66757-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="66757-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66757-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66757-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66757-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="66757-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66757-115">Application</span></span> | <span data-ttu-id="66757-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66757-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66757-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66757-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="66757-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66757-118">Request headers</span></span>
| <span data-ttu-id="66757-119">Nome</span><span class="sxs-lookup"><span data-stu-id="66757-119">Name</span></span>       | <span data-ttu-id="66757-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="66757-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="66757-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="66757-121">Authorization</span></span>  | <span data-ttu-id="66757-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66757-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66757-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="66757-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="66757-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="66757-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="66757-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66757-127">Request body</span></span>
<span data-ttu-id="66757-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66757-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="66757-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="66757-129">Parameter</span></span>    | <span data-ttu-id="66757-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="66757-130">Type</span></span>   |<span data-ttu-id="66757-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="66757-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66757-132">applyTo</span><span class="sxs-lookup"><span data-stu-id="66757-132">applyTo</span></span>|<span data-ttu-id="66757-133">string</span><span class="sxs-lookup"><span data-stu-id="66757-133">string</span></span>|<span data-ttu-id="66757-p104">Opcional. Determina o tipo de ação de limpeza.  Os valores possíveis são: `All`, `Formats` e `Contents`.</span><span class="sxs-lookup"><span data-stu-id="66757-p104">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="66757-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="66757-137">Response</span></span>

<span data-ttu-id="66757-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66757-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66757-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66757-140">Example</span></span>
<span data-ttu-id="66757-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="66757-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="66757-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66757-142">Request</span></span>
<span data-ttu-id="66757-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66757-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66757-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="66757-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="66757-145">C#</span><span class="sxs-lookup"><span data-stu-id="66757-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66757-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66757-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66757-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66757-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66757-148">Java</span><span class="sxs-lookup"><span data-stu-id="66757-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="66757-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="66757-149">Response</span></span>
<span data-ttu-id="66757-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66757-150">Here is an example of the response.</span></span> 
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


