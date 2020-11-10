---
title: Listar linhas
description: Recupere uma lista de objetos tablerow.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 74d0017d78caa35b203284dfb4da2e2041e4ac22
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969412"
---
# <a name="list-rows"></a><span data-ttu-id="2dafb-103">Listar linhas</span><span class="sxs-lookup"><span data-stu-id="2dafb-103">List rows</span></span>

<span data-ttu-id="2dafb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dafb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2dafb-105">Recupere uma lista de objetos tablerow.</span><span class="sxs-lookup"><span data-stu-id="2dafb-105">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="2dafb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2dafb-106">Permissions</span></span>
<span data-ttu-id="2dafb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2dafb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dafb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2dafb-109">Permission type</span></span>      | <span data-ttu-id="2dafb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2dafb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2dafb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2dafb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2dafb-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2dafb-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2dafb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2dafb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2dafb-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2dafb-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2dafb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2dafb-115">Application</span></span> | <span data-ttu-id="2dafb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2dafb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2dafb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2dafb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2dafb-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2dafb-118">Optional query parameters</span></span>
<span data-ttu-id="2dafb-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2dafb-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="2dafb-120">Para resultados confiáveis, use os parâmetros de consulta [$top](/graph/query-parameters#top) e [$skip](/graph/query-parameters#skip-parameter) para navegar pelos resultados.</span><span class="sxs-lookup"><span data-stu-id="2dafb-120">For reliable results, use the [$top](/graph/query-parameters#top) and [$skip](/graph/query-parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="2dafb-121">Isso ajudará a evitar problemas de desempenho relacionados a grandes conjuntos de resultados.</span><span class="sxs-lookup"><span data-stu-id="2dafb-121">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2dafb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2dafb-122">Request headers</span></span>
| <span data-ttu-id="2dafb-123">Nome</span><span class="sxs-lookup"><span data-stu-id="2dafb-123">Name</span></span>      |<span data-ttu-id="2dafb-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dafb-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2dafb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2dafb-125">Authorization</span></span>  | <span data-ttu-id="2dafb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2dafb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2dafb-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2dafb-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="2dafb-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2dafb-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2dafb-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2dafb-131">Request body</span></span>
<span data-ttu-id="2dafb-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2dafb-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2dafb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2dafb-133">Response</span></span>

<span data-ttu-id="2dafb-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [workbookTableRow](../resources/workbooktablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2dafb-134">If successful, this method returns a `200 OK` response code and collection of [workbookTableRow](../resources/workbooktablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2dafb-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2dafb-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2dafb-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2dafb-136">Request</span></span>
<span data-ttu-id="2dafb-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2dafb-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2dafb-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="2dafb-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_table_rows"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
# <a name="c"></a>[<span data-ttu-id="2dafb-139">C#</span><span class="sxs-lookup"><span data-stu-id="2dafb-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-table-rows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2dafb-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2dafb-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-table-rows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2dafb-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2dafb-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-table-rows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2dafb-142">Java</span><span class="sxs-lookup"><span data-stu-id="2dafb-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-table-rows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2dafb-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="2dafb-143">Response</span></span>
<span data-ttu-id="2dafb-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2dafb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

> <span data-ttu-id="2dafb-147">
  \*\*Observação:\*\* use os parâmetros de consulta [$top](/graph/query-parameters#top) e [$skip](/graph/query-parameters#skip-parameter) para navegar por um grande número de linhas.</span><span class="sxs-lookup"><span data-stu-id="2dafb-147">**Note:** Use the [$top](/graph/query-parameters#top) and [$skip](/graph/query-parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="2dafb-148">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="2dafb-148">Example:</span></span> 

`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5`
`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List rows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
