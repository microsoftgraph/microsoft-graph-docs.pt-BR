---
title: Listar nomes
description: 'Recupere uma lista de itens nomeados associados à planilha. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ae128c10393b4cabf40086f9fabc2eabfeaee62b
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460485"
---
# <a name="list-names"></a><span data-ttu-id="b23ea-103">Listar nomes</span><span class="sxs-lookup"><span data-stu-id="b23ea-103">List names</span></span>

<span data-ttu-id="b23ea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b23ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b23ea-105">Recupere uma lista de itens nomeados associados à planilha.</span><span class="sxs-lookup"><span data-stu-id="b23ea-105">Retrieve a list of named item associated with the worksheet.</span></span> 
## <a name="permissions"></a><span data-ttu-id="b23ea-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b23ea-106">Permissions</span></span>
<span data-ttu-id="b23ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b23ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b23ea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b23ea-109">Permission type</span></span>      | <span data-ttu-id="b23ea-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b23ea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b23ea-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b23ea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b23ea-112">Files. Read, files. ReadWrite, sites. Read. All</span><span class="sxs-lookup"><span data-stu-id="b23ea-112">Files.Read, Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="b23ea-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b23ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b23ea-114">Files. Read, files. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b23ea-114">Files.Read, Files.ReadWrite</span></span>    |
|<span data-ttu-id="b23ea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b23ea-115">Application</span></span> | <span data-ttu-id="b23ea-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="b23ea-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b23ea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b23ea-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b23ea-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b23ea-118">Optional query parameters</span></span>
<span data-ttu-id="b23ea-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b23ea-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b23ea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b23ea-120">Request headers</span></span>
| <span data-ttu-id="b23ea-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b23ea-121">Name</span></span>      |<span data-ttu-id="b23ea-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b23ea-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b23ea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b23ea-123">Authorization</span></span>  | <span data-ttu-id="b23ea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b23ea-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b23ea-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b23ea-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="b23ea-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b23ea-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b23ea-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b23ea-129">Request body</span></span>
<span data-ttu-id="b23ea-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b23ea-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b23ea-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b23ea-131">Response</span></span>

<span data-ttu-id="b23ea-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [workbookNamedItem](../resources/workbooknameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b23ea-132">If successful, this method returns a `200 OK` response code and collection of [workbookNamedItem](../resources/workbooknameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b23ea-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b23ea-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b23ea-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b23ea-134">Request</span></span>
<span data-ttu-id="b23ea-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b23ea-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b23ea-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b23ea-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tables"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/names
```
# <a name="c"></a>[<span data-ttu-id="b23ea-137">C#</span><span class="sxs-lookup"><span data-stu-id="b23ea-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tables-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b23ea-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b23ea-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tables-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b23ea-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b23ea-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tables-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b23ea-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b23ea-140">Response</span></span>
<span data-ttu-id="b23ea-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b23ea-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
