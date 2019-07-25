---
title: Listar WorksheetCollection
description: Recupere uma lista de objetos de planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6c7f0d6d6a46d5f2e4643158164081d6fe63c3c8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885933"
---
# <a name="list-worksheetcollection"></a><span data-ttu-id="59a2c-103">Listar WorksheetCollection</span><span class="sxs-lookup"><span data-stu-id="59a2c-103">List WorksheetCollection</span></span>

<span data-ttu-id="59a2c-104">Recupere uma lista de objetos de planilha.</span><span class="sxs-lookup"><span data-stu-id="59a2c-104">Retrieve a list of worksheet objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="59a2c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="59a2c-105">Permissions</span></span>
<span data-ttu-id="59a2c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59a2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59a2c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59a2c-108">Permission type</span></span>      | <span data-ttu-id="59a2c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59a2c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59a2c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59a2c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="59a2c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59a2c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="59a2c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59a2c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59a2c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59a2c-113">Not supported.</span></span>    |
|<span data-ttu-id="59a2c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59a2c-114">Application</span></span> | <span data-ttu-id="59a2c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59a2c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59a2c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59a2c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59a2c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="59a2c-117">Optional query parameters</span></span>
<span data-ttu-id="59a2c-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="59a2c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59a2c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59a2c-119">Request headers</span></span>
| <span data-ttu-id="59a2c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="59a2c-120">Name</span></span>      |<span data-ttu-id="59a2c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="59a2c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="59a2c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="59a2c-122">Authorization</span></span>  | <span data-ttu-id="59a2c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59a2c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59a2c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="59a2c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="59a2c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="59a2c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59a2c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59a2c-128">Request body</span></span>
<span data-ttu-id="59a2c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="59a2c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59a2c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="59a2c-130">Response</span></span>

<span data-ttu-id="59a2c-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [WorkbookWorksheet](../resources/worksheet.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59a2c-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookWorksheet](../resources/worksheet.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59a2c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59a2c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59a2c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59a2c-133">Request</span></span>
<span data-ttu-id="59a2c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59a2c-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="59a2c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="59a2c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_worksheetcollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="59a2c-136">C#</span><span class="sxs-lookup"><span data-stu-id="59a2c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-worksheetcollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59a2c-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="59a2c-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-worksheetcollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="59a2c-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="59a2c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-worksheetcollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="59a2c-139">Java</span><span class="sxs-lookup"><span data-stu-id="59a2c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-worksheetcollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="59a2c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="59a2c-140">Response</span></span>
<span data-ttu-id="59a2c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59a2c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
