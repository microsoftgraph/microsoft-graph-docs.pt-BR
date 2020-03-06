---
title: Listar linhas
description: Recupere uma lista de objetos tablerow.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f9ed8c200422746a5b768eaf456eb812c7f1af59
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509665"
---
# <a name="list-rows"></a><span data-ttu-id="749fa-103">Listar linhas</span><span class="sxs-lookup"><span data-stu-id="749fa-103">List rows</span></span>

<span data-ttu-id="749fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="749fa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="749fa-105">Recupere uma lista de objetos tablerow.</span><span class="sxs-lookup"><span data-stu-id="749fa-105">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="749fa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="749fa-106">Permissions</span></span>
<span data-ttu-id="749fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="749fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="749fa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="749fa-109">Permission type</span></span>      | <span data-ttu-id="749fa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="749fa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="749fa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="749fa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="749fa-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="749fa-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="749fa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="749fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="749fa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="749fa-114">Not supported.</span></span>    |
|<span data-ttu-id="749fa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="749fa-115">Application</span></span> | <span data-ttu-id="749fa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="749fa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="749fa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="749fa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="749fa-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="749fa-118">Optional query parameters</span></span>
<span data-ttu-id="749fa-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="749fa-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>  <span data-ttu-id="749fa-120">Para resultados confiáveis, use os parâmetros de consulta [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) e [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) para navegar pelos resultados.</span><span class="sxs-lookup"><span data-stu-id="749fa-120">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="749fa-121">Isso ajudará a evitar problemas de desempenho relacionados a grandes conjuntos de resultados.</span><span class="sxs-lookup"><span data-stu-id="749fa-121">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="749fa-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="749fa-122">Request headers</span></span>
| <span data-ttu-id="749fa-123">Nome</span><span class="sxs-lookup"><span data-stu-id="749fa-123">Name</span></span>      |<span data-ttu-id="749fa-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="749fa-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="749fa-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="749fa-125">Authorization</span></span>  | <span data-ttu-id="749fa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="749fa-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="749fa-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="749fa-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="749fa-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="749fa-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="749fa-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="749fa-131">Request body</span></span>
<span data-ttu-id="749fa-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="749fa-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="749fa-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="749fa-133">Response</span></span>

<span data-ttu-id="749fa-134">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [WorkbookTableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="749fa-134">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableRow](../resources/tablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="749fa-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="749fa-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="749fa-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="749fa-136">Request</span></span>
<span data-ttu-id="749fa-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="749fa-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="749fa-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="749fa-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_table_rows"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
# <a name="c"></a>[<span data-ttu-id="749fa-139">C#</span><span class="sxs-lookup"><span data-stu-id="749fa-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-table-rows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="749fa-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="749fa-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-table-rows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="749fa-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="749fa-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-table-rows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="749fa-142">Java</span><span class="sxs-lookup"><span data-stu-id="749fa-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-table-rows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="749fa-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="749fa-143">Response</span></span>
<span data-ttu-id="749fa-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="749fa-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 82

{
  "value": [
    {
      "index": 99,
      "values": "values-value"
    }
  ]
}
```
> <span data-ttu-id="749fa-147">
  \*\*Observação:\*\* use os parâmetros de consulta [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) e [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) para navegar por um grande número de linhas.</span><span class="sxs-lookup"><span data-stu-id="749fa-147">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="749fa-148">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="749fa-148">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5`


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
