---
title: Listar WorksheetCollection
description: Recupere uma lista de objetos de planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2ed967d04c15e060588a582cb12e25239eb56602
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508650"
---
# <a name="list-worksheetcollection"></a><span data-ttu-id="7d0ad-103">Listar WorksheetCollection</span><span class="sxs-lookup"><span data-stu-id="7d0ad-103">List WorksheetCollection</span></span>

<span data-ttu-id="7d0ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d0ad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7d0ad-105">Recupere uma lista de objetos de planilha.</span><span class="sxs-lookup"><span data-stu-id="7d0ad-105">Retrieve a list of worksheet objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d0ad-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d0ad-106">Permissions</span></span>
<span data-ttu-id="7d0ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d0ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d0ad-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d0ad-109">Permission type</span></span>      | <span data-ttu-id="7d0ad-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d0ad-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d0ad-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d0ad-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7d0ad-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d0ad-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7d0ad-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d0ad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d0ad-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d0ad-114">Not supported.</span></span>    |
|<span data-ttu-id="7d0ad-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d0ad-115">Application</span></span> | <span data-ttu-id="7d0ad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d0ad-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d0ad-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d0ad-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7d0ad-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7d0ad-118">Optional query parameters</span></span>
<span data-ttu-id="7d0ad-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7d0ad-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d0ad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d0ad-120">Request headers</span></span>
| <span data-ttu-id="7d0ad-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7d0ad-121">Name</span></span>      |<span data-ttu-id="7d0ad-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d0ad-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7d0ad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d0ad-123">Authorization</span></span>  | <span data-ttu-id="7d0ad-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d0ad-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7d0ad-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7d0ad-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="7d0ad-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7d0ad-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d0ad-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d0ad-129">Request body</span></span>
<span data-ttu-id="7d0ad-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d0ad-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d0ad-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d0ad-131">Response</span></span>

<span data-ttu-id="7d0ad-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [WorkbookWorksheet](../resources/worksheet.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d0ad-132">If successful, this method returns a `200 OK` response code and collection of [WorkbookWorksheet](../resources/worksheet.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7d0ad-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d0ad-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d0ad-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d0ad-134">Request</span></span>
<span data-ttu-id="7d0ad-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d0ad-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7d0ad-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d0ad-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_worksheetcollection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets
```
# <a name="c"></a>[<span data-ttu-id="7d0ad-137">C#</span><span class="sxs-lookup"><span data-stu-id="7d0ad-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-worksheetcollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d0ad-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d0ad-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-worksheetcollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d0ad-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d0ad-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-worksheetcollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d0ad-140">Java</span><span class="sxs-lookup"><span data-stu-id="7d0ad-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-worksheetcollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7d0ad-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d0ad-141">Response</span></span>
<span data-ttu-id="7d0ad-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d0ad-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "id": "id-value",
      "position": 99,
      "name": "name-value",
      "visibility": "visibility-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List WorksheetCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
