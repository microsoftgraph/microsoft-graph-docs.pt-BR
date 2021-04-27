---
title: 'TableRowCollection: ItemAt'
description: Obtém uma linha com base em sua posição na coleção.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1fcb87a1422b28c8f086dc619076dba6ddd578c5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054781"
---
# <a name="tablerowcollection-itemat"></a><span data-ttu-id="a9b7a-103">TableRowCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="a9b7a-103">TableRowCollection: ItemAt</span></span>

<span data-ttu-id="a9b7a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9b7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9b7a-105">Obtém uma linha com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="a9b7a-105">Gets a row based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="a9b7a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9b7a-106">Permissions</span></span>
<span data-ttu-id="a9b7a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9b7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9b7a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9b7a-109">Permission type</span></span>      | <span data-ttu-id="a9b7a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9b7a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9b7a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9b7a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a9b7a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9b7a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a9b7a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9b7a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9b7a-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9b7a-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a9b7a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9b7a-115">Application</span></span> | <span data-ttu-id="a9b7a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9b7a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9b7a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9b7a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/rows/ItemAt
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/rows/ItemAt
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/rows/ItemAt
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/rows/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="a9b7a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9b7a-118">Request headers</span></span>
| <span data-ttu-id="a9b7a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a9b7a-119">Name</span></span>       | <span data-ttu-id="a9b7a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9b7a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a9b7a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9b7a-121">Authorization</span></span>  | <span data-ttu-id="a9b7a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9b7a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a9b7a-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a9b7a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="a9b7a-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a9b7a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9b7a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9b7a-127">Request body</span></span>
<span data-ttu-id="a9b7a-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9b7a-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a9b7a-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a9b7a-129">Parameter</span></span>    | <span data-ttu-id="a9b7a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9b7a-130">Type</span></span>   |<span data-ttu-id="a9b7a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9b7a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9b7a-132">index</span><span class="sxs-lookup"><span data-stu-id="a9b7a-132">index</span></span>|<span data-ttu-id="a9b7a-133">number</span><span class="sxs-lookup"><span data-stu-id="a9b7a-133">number</span></span>|<span data-ttu-id="a9b7a-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="a9b7a-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="a9b7a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9b7a-136">Response</span></span>

<span data-ttu-id="a9b7a-137">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [workbookTableRow](../resources/workbooktablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9b7a-137">If successful, this method returns `200 OK` response code and [workbookTableRow](../resources/workbooktablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9b7a-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9b7a-138">Example</span></span>
<span data-ttu-id="a9b7a-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a9b7a-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a9b7a-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9b7a-140">Request</span></span>
<span data-ttu-id="a9b7a-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9b7a-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9b7a-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9b7a-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="a9b7a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9b7a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9b7a-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9b7a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablerowcollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a9b7a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9b7a-145">Response</span></span>
<span data-ttu-id="a9b7a-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9b7a-146">Here is an example of the response.</span></span> <span data-ttu-id="a9b7a-147">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a9b7a-147">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableRowCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


