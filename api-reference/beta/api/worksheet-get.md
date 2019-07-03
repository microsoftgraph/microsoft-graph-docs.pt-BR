---
title: Get Worksheet
description: Recupere as propriedades e os relacionamentos do objeto de planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4816f7bc55bb597c112bc1a25c9563c7d8120080
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446280"
---
# <a name="get-worksheet"></a><span data-ttu-id="ef8e9-103">Get Worksheet</span><span class="sxs-lookup"><span data-stu-id="ef8e9-103">Get Worksheet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef8e9-104">Recupere as propriedades e os relacionamentos do objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="ef8e9-104">Retrieve the properties and relationships of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ef8e9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef8e9-105">Permissions</span></span>
<span data-ttu-id="ef8e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef8e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef8e9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef8e9-108">Permission type</span></span>      | <span data-ttu-id="ef8e9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef8e9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef8e9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef8e9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ef8e9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef8e9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ef8e9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef8e9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef8e9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef8e9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ef8e9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef8e9-114">Application</span></span> | <span data-ttu-id="ef8e9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef8e9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef8e9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef8e9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ef8e9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ef8e9-117">Optional query parameters</span></span>
<span data-ttu-id="ef8e9-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ef8e9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef8e9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef8e9-119">Request headers</span></span>
| <span data-ttu-id="ef8e9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ef8e9-120">Name</span></span>      |<span data-ttu-id="ef8e9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef8e9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ef8e9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef8e9-122">Authorization</span></span>  | <span data-ttu-id="ef8e9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef8e9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ef8e9-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ef8e9-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ef8e9-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ef8e9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef8e9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef8e9-128">Request body</span></span>
<span data-ttu-id="ef8e9-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ef8e9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef8e9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef8e9-130">Response</span></span>

<span data-ttu-id="ef8e9-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookWorksheet](../resources/workbookworksheet.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef8e9-131">If successful, this method returns a `200 OK` response code and [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ef8e9-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef8e9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef8e9-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef8e9-133">Request</span></span>
<span data-ttu-id="ef8e9-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef8e9-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ef8e9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef8e9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_worksheet"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ef8e9-136">C#</span><span class="sxs-lookup"><span data-stu-id="ef8e9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef8e9-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="ef8e9-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ef8e9-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ef8e9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ef8e9-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef8e9-139">Response</span></span>
<span data-ttu-id="ef8e9-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef8e9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
