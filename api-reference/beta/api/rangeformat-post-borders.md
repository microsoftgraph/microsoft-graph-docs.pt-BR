---
title: Criar RangeBorder
description: Use essa API para criar uma nova RangeBorder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b4c58b7cf9c2a4ee4cb5d7840160c36573c23a71
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454560"
---
# <a name="create-rangeborder"></a><span data-ttu-id="607e8-103">Criar RangeBorder</span><span class="sxs-lookup"><span data-stu-id="607e8-103">Create RangeBorder</span></span>

<span data-ttu-id="607e8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="607e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="607e8-105">Use essa API para criar uma nova RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="607e8-105">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="607e8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="607e8-106">Permissions</span></span>
<span data-ttu-id="607e8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="607e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="607e8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="607e8-109">Permission type</span></span>      | <span data-ttu-id="607e8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="607e8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="607e8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="607e8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="607e8-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="607e8-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="607e8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="607e8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="607e8-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="607e8-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="607e8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="607e8-115">Application</span></span> | <span data-ttu-id="607e8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="607e8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="607e8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="607e8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="607e8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="607e8-118">Request headers</span></span>
| <span data-ttu-id="607e8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="607e8-119">Name</span></span>       | <span data-ttu-id="607e8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="607e8-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="607e8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="607e8-121">Authorization</span></span>  | <span data-ttu-id="607e8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="607e8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="607e8-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="607e8-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="607e8-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="607e8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="607e8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="607e8-127">Request body</span></span>
<span data-ttu-id="607e8-128">No corpo da solicitação, forneça uma representação JSON do objeto [workbookRangeBorder](../resources/workbookrangeborder.md) .</span><span class="sxs-lookup"><span data-stu-id="607e8-128">In the request body, supply a JSON representation of [workbookRangeBorder](../resources/workbookrangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="607e8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="607e8-129">Response</span></span>

<span data-ttu-id="607e8-130">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [workbookRangeBorder](../resources/workbookrangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="607e8-130">If successful, this method returns `201 Created` response code and [workbookRangeBorder](../resources/workbookrangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="607e8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="607e8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="607e8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="607e8-132">Request</span></span>
<span data-ttu-id="607e8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="607e8-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="607e8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="607e8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/borders
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
# <a name="c"></a>[<span data-ttu-id="607e8-135">C#</span><span class="sxs-lookup"><span data-stu-id="607e8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-rangeborder-from-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="607e8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="607e8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-rangeborder-from-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="607e8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="607e8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-rangeborder-from-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="607e8-138">No corpo da solicitação, forneça uma representação JSON do objeto [workbookRangeBorder](../resources/workbookrangeborder.md) .</span><span class="sxs-lookup"><span data-stu-id="607e8-138">In the request body, supply a JSON representation of [workbookRangeBorder](../resources/workbookrangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="607e8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="607e8-139">Response</span></span>
<span data-ttu-id="607e8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="607e8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
