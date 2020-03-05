---
title: 'Range: delete'
description: Exclui as células associadas ao intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1900ae6f02414d177f2aea5a90d9c5d940cc6792
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454765"
---
# <a name="range-delete"></a><span data-ttu-id="d2e26-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="d2e26-103">Range: delete</span></span>

<span data-ttu-id="d2e26-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d2e26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2e26-105">Exclui as células associadas ao intervalo.</span><span class="sxs-lookup"><span data-stu-id="d2e26-105">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="d2e26-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2e26-106">Permissions</span></span>
<span data-ttu-id="d2e26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2e26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2e26-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2e26-109">Permission type</span></span>      | <span data-ttu-id="d2e26-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2e26-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2e26-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2e26-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d2e26-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2e26-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d2e26-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2e26-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2e26-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2e26-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d2e26-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2e26-115">Application</span></span> | <span data-ttu-id="d2e26-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2e26-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2e26-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2e26-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="d2e26-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2e26-118">Request headers</span></span>
| <span data-ttu-id="d2e26-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d2e26-119">Name</span></span>       | <span data-ttu-id="d2e26-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2e26-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d2e26-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2e26-121">Authorization</span></span>  | <span data-ttu-id="d2e26-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2e26-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2e26-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d2e26-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="d2e26-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d2e26-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2e26-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2e26-127">Request body</span></span>
<span data-ttu-id="d2e26-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2e26-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d2e26-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d2e26-129">Parameter</span></span>    | <span data-ttu-id="d2e26-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2e26-130">Type</span></span>   |<span data-ttu-id="d2e26-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2e26-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2e26-132">shift</span><span class="sxs-lookup"><span data-stu-id="d2e26-132">shift</span></span>|<span data-ttu-id="d2e26-133">string</span><span class="sxs-lookup"><span data-stu-id="d2e26-133">string</span></span>|<span data-ttu-id="d2e26-p104">Especifica como deslocar as células.  Os valores possíveis são: `Up` e `Left`.</span><span class="sxs-lookup"><span data-stu-id="d2e26-p104">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="d2e26-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2e26-136">Response</span></span>

<span data-ttu-id="d2e26-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2e26-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2e26-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2e26-139">Example</span></span>
<span data-ttu-id="d2e26-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d2e26-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d2e26-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2e26-141">Request</span></span>
<span data-ttu-id="d2e26-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2e26-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2e26-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2e26-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d2e26-144">C#</span><span class="sxs-lookup"><span data-stu-id="d2e26-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2e26-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2e26-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2e26-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2e26-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d2e26-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2e26-147">Response</span></span>
<span data-ttu-id="d2e26-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2e26-148">Here is an example of the response.</span></span> 
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
