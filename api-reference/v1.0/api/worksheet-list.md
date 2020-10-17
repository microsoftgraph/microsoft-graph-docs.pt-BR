---
title: Listar WorksheetCollection
description: Recupere uma lista de objetos de planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 88009e81a2892a8a0aebc26bfdfee81c296cf0c1
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582209"
---
# <a name="list-worksheetcollection"></a><span data-ttu-id="fc5fb-103">Listar WorksheetCollection</span><span class="sxs-lookup"><span data-stu-id="fc5fb-103">List WorksheetCollection</span></span>

<span data-ttu-id="fc5fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc5fb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc5fb-105">Recupere uma lista de objetos de planilha.</span><span class="sxs-lookup"><span data-stu-id="fc5fb-105">Retrieve a list of worksheet objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc5fb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc5fb-106">Permissions</span></span>
<span data-ttu-id="fc5fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc5fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc5fb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc5fb-109">Permission type</span></span>      | <span data-ttu-id="fc5fb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc5fb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc5fb-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc5fb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fc5fb-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc5fb-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fc5fb-113">Delegada (conta Microsoft pessoal)</span><span class="sxs-lookup"><span data-stu-id="fc5fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc5fb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc5fb-114">Not supported.</span></span>    |
|<span data-ttu-id="fc5fb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc5fb-115">Application</span></span> | <span data-ttu-id="fc5fb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc5fb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc5fb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc5fb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fc5fb-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fc5fb-118">Optional query parameters</span></span>
<span data-ttu-id="fc5fb-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fc5fb-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc5fb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc5fb-120">Request headers</span></span>
| <span data-ttu-id="fc5fb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fc5fb-121">Name</span></span>      |<span data-ttu-id="fc5fb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc5fb-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fc5fb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc5fb-123">Authorization</span></span>  | <span data-ttu-id="fc5fb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc5fb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc5fb-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fc5fb-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="fc5fb-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="fc5fb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc5fb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc5fb-129">Request body</span></span>
<span data-ttu-id="fc5fb-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc5fb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc5fb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc5fb-131">Response</span></span>

<span data-ttu-id="fc5fb-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [WorkbookWorksheet](../resources/worksheet.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc5fb-132">If successful, this method returns a `200 OK` response code and collection of [WorkbookWorksheet](../resources/worksheet.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fc5fb-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc5fb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc5fb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc5fb-134">Request</span></span>
<span data-ttu-id="fc5fb-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc5fb-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fc5fb-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc5fb-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_worksheetcollection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets
```
# <a name="c"></a>[<span data-ttu-id="fc5fb-137">C#</span><span class="sxs-lookup"><span data-stu-id="fc5fb-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-worksheetcollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc5fb-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc5fb-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-worksheetcollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc5fb-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc5fb-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-worksheetcollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc5fb-140">Java</span><span class="sxs-lookup"><span data-stu-id="fc5fb-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-worksheetcollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fc5fb-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc5fb-141">Response</span></span>
<span data-ttu-id="fc5fb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc5fb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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