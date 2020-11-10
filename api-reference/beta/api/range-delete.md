---
title: 'Range: delete'
description: Exclui as células associadas ao intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d6de79f2e0395899f0c2061eddcd9b5e9e14bad7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974529"
---
# <a name="range-delete"></a><span data-ttu-id="fc596-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="fc596-103">Range: delete</span></span>

<span data-ttu-id="fc596-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc596-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc596-105">Exclui as células associadas ao intervalo.</span><span class="sxs-lookup"><span data-stu-id="fc596-105">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc596-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc596-106">Permissions</span></span>
<span data-ttu-id="fc596-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc596-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc596-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc596-109">Permission type</span></span>      | <span data-ttu-id="fc596-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc596-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc596-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc596-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fc596-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc596-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fc596-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc596-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc596-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc596-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fc596-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc596-115">Application</span></span> | <span data-ttu-id="fc596-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc596-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc596-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc596-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="fc596-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc596-118">Request headers</span></span>
| <span data-ttu-id="fc596-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fc596-119">Name</span></span>       | <span data-ttu-id="fc596-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc596-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fc596-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc596-121">Authorization</span></span>  | <span data-ttu-id="fc596-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc596-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc596-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fc596-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="fc596-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="fc596-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc596-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc596-127">Request body</span></span>
<span data-ttu-id="fc596-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc596-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fc596-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fc596-129">Parameter</span></span>    | <span data-ttu-id="fc596-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc596-130">Type</span></span>   |<span data-ttu-id="fc596-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc596-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc596-132">shift</span><span class="sxs-lookup"><span data-stu-id="fc596-132">shift</span></span>|<span data-ttu-id="fc596-133">string</span><span class="sxs-lookup"><span data-stu-id="fc596-133">string</span></span>|<span data-ttu-id="fc596-p104">Especifica como deslocar as células.  Os valores possíveis são: `Up` e `Left`.</span><span class="sxs-lookup"><span data-stu-id="fc596-p104">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="fc596-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc596-136">Response</span></span>

<span data-ttu-id="fc596-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc596-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc596-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc596-139">Example</span></span>
<span data-ttu-id="fc596-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="fc596-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fc596-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc596-141">Request</span></span>
<span data-ttu-id="fc596-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc596-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fc596-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc596-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```
# <a name="c"></a>[<span data-ttu-id="fc596-144">C#</span><span class="sxs-lookup"><span data-stu-id="fc596-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc596-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc596-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc596-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc596-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc596-147">Java</span><span class="sxs-lookup"><span data-stu-id="fc596-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fc596-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc596-148">Response</span></span>
<span data-ttu-id="fc596-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc596-149">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


