---
title: Obter RangeFormat
description: Recupere as propriedades e os relacionamentos do objeto rangeformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9e4188453538375696a2e59faec449662f8bdbbd
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313790"
---
# <a name="get-rangeformat"></a><span data-ttu-id="e52db-103">Obter RangeFormat</span><span class="sxs-lookup"><span data-stu-id="e52db-103">Get RangeFormat</span></span>

<span data-ttu-id="e52db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e52db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e52db-105">Recupere as propriedades e os relacionamentos do objeto rangeformat.</span><span class="sxs-lookup"><span data-stu-id="e52db-105">Retrieve the properties and relationships of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e52db-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e52db-106">Permissions</span></span>
<span data-ttu-id="e52db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e52db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e52db-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e52db-109">Permission type</span></span>      | <span data-ttu-id="e52db-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e52db-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e52db-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e52db-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e52db-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e52db-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e52db-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e52db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e52db-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e52db-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e52db-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e52db-115">Application</span></span> | <span data-ttu-id="e52db-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e52db-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e52db-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e52db-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format
GET /workbook/worksheets/{id|name}/range(address='<address>')/format
GET /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e52db-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e52db-118">Optional query parameters</span></span>
<span data-ttu-id="e52db-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e52db-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e52db-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e52db-120">Request headers</span></span>
| <span data-ttu-id="e52db-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e52db-121">Name</span></span>      |<span data-ttu-id="e52db-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e52db-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e52db-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e52db-123">Authorization</span></span>  | <span data-ttu-id="e52db-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e52db-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e52db-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e52db-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="e52db-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e52db-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e52db-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e52db-129">Request body</span></span>
<span data-ttu-id="e52db-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e52db-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e52db-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e52db-131">Response</span></span>

<span data-ttu-id="e52db-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookRangeFormat](../resources/workbookrangeformat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e52db-132">If successful, this method returns a `200 OK` response code and [workbookRangeFormat](../resources/workbookrangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e52db-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e52db-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e52db-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e52db-134">Request</span></span>
<span data-ttu-id="e52db-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e52db-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e52db-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e52db-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rangeformat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format
```
# <a name="c"></a>[<span data-ttu-id="e52db-137">C#</span><span class="sxs-lookup"><span data-stu-id="e52db-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e52db-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e52db-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e52db-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e52db-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e52db-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e52db-140">Response</span></span>
<span data-ttu-id="e52db-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e52db-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 96

{
  "columnWidth": 99,
  "horizontalAlignment": "horizontalAlignment-value",
  "rowHeight": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get RangeFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->