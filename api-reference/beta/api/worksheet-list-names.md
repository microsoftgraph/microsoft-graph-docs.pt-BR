---
title: Listar nomes
description: 'Recupere uma lista de itens nomeados associados à planilha. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 6dba3992e6e2bf7a9562cd63ee6019a5184ae669
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051652"
---
# <a name="list-names"></a><span data-ttu-id="c14e0-103">Listar nomes</span><span class="sxs-lookup"><span data-stu-id="c14e0-103">List names</span></span>

<span data-ttu-id="c14e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c14e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c14e0-105">Recupere uma lista de itens nomeados associados à planilha.</span><span class="sxs-lookup"><span data-stu-id="c14e0-105">Retrieve a list of named item associated with the worksheet.</span></span> 
## <a name="permissions"></a><span data-ttu-id="c14e0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c14e0-106">Permissions</span></span>
<span data-ttu-id="c14e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c14e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c14e0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c14e0-109">Permission type</span></span>      | <span data-ttu-id="c14e0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c14e0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c14e0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c14e0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c14e0-112">Files.Read, Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c14e0-112">Files.Read, Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="c14e0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c14e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c14e0-114">Files.Read, Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c14e0-114">Files.Read, Files.ReadWrite</span></span>    |
|<span data-ttu-id="c14e0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c14e0-115">Application</span></span> | <span data-ttu-id="c14e0-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c14e0-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c14e0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c14e0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/names
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c14e0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c14e0-118">Optional query parameters</span></span>
<span data-ttu-id="c14e0-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c14e0-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c14e0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c14e0-120">Request headers</span></span>
| <span data-ttu-id="c14e0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c14e0-121">Name</span></span>      |<span data-ttu-id="c14e0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c14e0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c14e0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c14e0-123">Authorization</span></span>  | <span data-ttu-id="c14e0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c14e0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c14e0-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c14e0-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="c14e0-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c14e0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c14e0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c14e0-129">Request body</span></span>
<span data-ttu-id="c14e0-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c14e0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c14e0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c14e0-131">Response</span></span>

<span data-ttu-id="c14e0-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [workbookNamedItem](../resources/workbooknameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c14e0-132">If successful, this method returns a `200 OK` response code and collection of [workbookNamedItem](../resources/workbooknameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c14e0-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c14e0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c14e0-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c14e0-134">Request</span></span>
<span data-ttu-id="c14e0-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c14e0-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c14e0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c14e0-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tables_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/names
```
# <a name="c"></a>[<span data-ttu-id="c14e0-137">C#</span><span class="sxs-lookup"><span data-stu-id="c14e0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tables-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c14e0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c14e0-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tables-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c14e0-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c14e0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tables-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c14e0-140">Java</span><span class="sxs-lookup"><span data-stu-id="c14e0-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tables-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c14e0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c14e0-141">Response</span></span>
<span data-ttu-id="c14e0-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c14e0-142">Here is an example of the response.</span></span> <span data-ttu-id="c14e0-143">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c14e0-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "name": "myrange",
      "scope": "worksheet"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List tables",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
