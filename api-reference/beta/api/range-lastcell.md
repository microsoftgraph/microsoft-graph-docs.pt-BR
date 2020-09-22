---
title: 'Range: LastCell'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f0856134f9e86d2e888368d528cf775a18c68c52
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067927"
---
# <a name="range-lastcell"></a><span data-ttu-id="be72f-103">Range: LastCell</span><span class="sxs-lookup"><span data-stu-id="be72f-103">Range: LastCell</span></span>

<span data-ttu-id="be72f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be72f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be72f-p101">Obtém a última célula do intervalo. Por exemplo, a última célula de "B2:D5" é "D5".</span><span class="sxs-lookup"><span data-stu-id="be72f-p101">Gets the last cell within the range. For example, the last cell of "B2:D5" is "D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="be72f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="be72f-107">Permissions</span></span>
<span data-ttu-id="be72f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be72f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be72f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be72f-110">Permission type</span></span>      | <span data-ttu-id="be72f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be72f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be72f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be72f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="be72f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be72f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be72f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be72f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be72f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be72f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be72f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be72f-116">Application</span></span> | <span data-ttu-id="be72f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be72f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be72f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be72f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/LastCell
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastCell
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastCell

```
## <a name="request-headers"></a><span data-ttu-id="be72f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be72f-119">Request headers</span></span>
| <span data-ttu-id="be72f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="be72f-120">Name</span></span>       | <span data-ttu-id="be72f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="be72f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="be72f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="be72f-122">Authorization</span></span>  | <span data-ttu-id="be72f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be72f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="be72f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="be72f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="be72f-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="be72f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be72f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be72f-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="be72f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="be72f-129">Response</span></span>

<span data-ttu-id="be72f-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be72f-130">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be72f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be72f-131">Example</span></span>
<span data-ttu-id="be72f-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="be72f-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="be72f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be72f-133">Request</span></span>
<span data-ttu-id="be72f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be72f-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="be72f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="be72f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_lastcell"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/LastCell
```
# <a name="c"></a>[<span data-ttu-id="be72f-136">C#</span><span class="sxs-lookup"><span data-stu-id="be72f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-lastcell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be72f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be72f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-lastcell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be72f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be72f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-lastcell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="be72f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="be72f-139">Response</span></span>
<span data-ttu-id="be72f-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be72f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: LastCell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


