---
title: Criar RangeBorder
description: Use essa API para criar uma nova RangeBorder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 01aa529e38f5eb5868a0a8d8a620343c0d74df0a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055782"
---
# <a name="create-rangeborder"></a><span data-ttu-id="dac38-103">Criar RangeBorder</span><span class="sxs-lookup"><span data-stu-id="dac38-103">Create RangeBorder</span></span>

<span data-ttu-id="dac38-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dac38-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dac38-105">Use essa API para criar uma nova RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="dac38-105">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="dac38-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dac38-106">Permissions</span></span>
<span data-ttu-id="dac38-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dac38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dac38-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dac38-109">Permission type</span></span>      | <span data-ttu-id="dac38-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dac38-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dac38-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dac38-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dac38-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dac38-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dac38-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dac38-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dac38-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dac38-114">Not supported.</span></span>    |
|<span data-ttu-id="dac38-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dac38-115">Application</span></span> | <span data-ttu-id="dac38-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dac38-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dac38-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dac38-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/format/borders
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/borders
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/borders
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="dac38-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dac38-118">Request headers</span></span>
| <span data-ttu-id="dac38-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dac38-119">Name</span></span>       | <span data-ttu-id="dac38-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dac38-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dac38-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dac38-121">Authorization</span></span>  | <span data-ttu-id="dac38-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dac38-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dac38-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dac38-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="dac38-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="dac38-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dac38-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dac38-127">Request body</span></span>
<span data-ttu-id="dac38-128">No corpo da solicitação, fornece uma representação JSON [do objeto WorkbookRangeBorder.](../resources/rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="dac38-128">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dac38-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dac38-129">Response</span></span>

<span data-ttu-id="dac38-130">Se tiver êxito, este método retornará `201 Created` o código de resposta e o objeto [WorkbookRangeBorder](../resources/rangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dac38-130">If successful, this method returns `201 Created` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dac38-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dac38-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dac38-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dac38-132">Request</span></span>
<span data-ttu-id="dac38-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dac38-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dac38-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dac38-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
# <a name="c"></a>[<span data-ttu-id="dac38-135">C#</span><span class="sxs-lookup"><span data-stu-id="dac38-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-rangeborder-from-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dac38-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dac38-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-rangeborder-from-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dac38-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dac38-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-rangeborder-from-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dac38-138">Java</span><span class="sxs-lookup"><span data-stu-id="dac38-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-rangeborder-from-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="dac38-139">No corpo da solicitação, fornece uma representação JSON [do objeto WorkbookRangeBorder.](../resources/rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="dac38-139">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="dac38-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="dac38-140">Response</span></span>
<span data-ttu-id="dac38-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dac38-141">Here is an example of the response.</span></span> <span data-ttu-id="dac38-142">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dac38-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

