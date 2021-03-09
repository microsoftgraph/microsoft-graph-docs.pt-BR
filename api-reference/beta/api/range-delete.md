---
title: 'Range: delete'
description: Exclui as células associadas ao intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a3183e393d66c75afd05ccc2226e5217dd6b4a23
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573978"
---
# <a name="range-delete"></a><span data-ttu-id="3691e-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="3691e-103">Range: delete</span></span>

<span data-ttu-id="3691e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3691e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3691e-105">Exclui as células associadas ao intervalo.</span><span class="sxs-lookup"><span data-stu-id="3691e-105">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="3691e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3691e-106">Permissions</span></span>
<span data-ttu-id="3691e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3691e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3691e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3691e-109">Permission type</span></span>      | <span data-ttu-id="3691e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3691e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3691e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3691e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3691e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3691e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3691e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3691e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3691e-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3691e-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3691e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3691e-115">Application</span></span> | <span data-ttu-id="3691e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3691e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3691e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3691e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/delete
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/delete
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/delete
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="3691e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3691e-118">Request headers</span></span>
| <span data-ttu-id="3691e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3691e-119">Name</span></span>       | <span data-ttu-id="3691e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3691e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3691e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3691e-121">Authorization</span></span>  | <span data-ttu-id="3691e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3691e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3691e-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3691e-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="3691e-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="3691e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3691e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3691e-127">Request body</span></span>
<span data-ttu-id="3691e-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3691e-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3691e-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3691e-129">Parameter</span></span>    | <span data-ttu-id="3691e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3691e-130">Type</span></span>   |<span data-ttu-id="3691e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3691e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3691e-132">shift</span><span class="sxs-lookup"><span data-stu-id="3691e-132">shift</span></span>|<span data-ttu-id="3691e-133">string</span><span class="sxs-lookup"><span data-stu-id="3691e-133">string</span></span>|<span data-ttu-id="3691e-p104">Especifica como deslocar as células.  Os valores possíveis são: `Up` e `Left`.</span><span class="sxs-lookup"><span data-stu-id="3691e-p104">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="3691e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3691e-136">Response</span></span>

<span data-ttu-id="3691e-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3691e-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3691e-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3691e-139">Example</span></span>
<span data-ttu-id="3691e-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3691e-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3691e-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3691e-141">Request</span></span>
<span data-ttu-id="3691e-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3691e-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3691e-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="3691e-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3691e-144">C#</span><span class="sxs-lookup"><span data-stu-id="3691e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3691e-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3691e-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3691e-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3691e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3691e-147">Java</span><span class="sxs-lookup"><span data-stu-id="3691e-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3691e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="3691e-148">Response</span></span>
<span data-ttu-id="3691e-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3691e-149">Here is an example of the response.</span></span> 
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


