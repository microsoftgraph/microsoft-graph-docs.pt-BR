---
title: Obter tabela
description: Recupere as propriedades e os relacionamentos do objeto de tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1ea871bf16f3ba767471e03fbd585afdf00f63db
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48461585"
---
# <a name="get-table"></a><span data-ttu-id="138c9-103">Obter tabela</span><span class="sxs-lookup"><span data-stu-id="138c9-103">Get Table</span></span>

<span data-ttu-id="138c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="138c9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="138c9-105">Recupere as propriedades e os relacionamentos do objeto de tabela.</span><span class="sxs-lookup"><span data-stu-id="138c9-105">Retrieve the properties and relationships of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="138c9-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="138c9-106">Permissions</span></span>
<span data-ttu-id="138c9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="138c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="138c9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="138c9-109">Permission type</span></span>      | <span data-ttu-id="138c9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="138c9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="138c9-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="138c9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="138c9-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="138c9-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="138c9-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="138c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="138c9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="138c9-114">Not supported.</span></span>    |
|<span data-ttu-id="138c9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="138c9-115">Application</span></span> | <span data-ttu-id="138c9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="138c9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="138c9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="138c9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}
GET /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="138c9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="138c9-118">Optional query parameters</span></span>
<span data-ttu-id="138c9-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="138c9-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="138c9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="138c9-120">Request headers</span></span>
| <span data-ttu-id="138c9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="138c9-121">Name</span></span>      |<span data-ttu-id="138c9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="138c9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="138c9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="138c9-123">Authorization</span></span>  | <span data-ttu-id="138c9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="138c9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="138c9-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="138c9-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="138c9-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="138c9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="138c9-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="138c9-129">Request body</span></span>
<span data-ttu-id="138c9-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="138c9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="138c9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="138c9-131">Response</span></span>

<span data-ttu-id="138c9-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbooktable](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="138c9-132">If successful, this method returns a `200 OK` response code and [WorkbookTable](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="138c9-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="138c9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="138c9-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="138c9-134">Request</span></span>
<span data-ttu-id="138c9-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="138c9-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="138c9-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="138c9-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_table"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}
```
# <a name="c"></a>[<span data-ttu-id="138c9-137">C#</span><span class="sxs-lookup"><span data-stu-id="138c9-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-table-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="138c9-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="138c9-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-table-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="138c9-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="138c9-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-table-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="138c9-140">Java</span><span class="sxs-lookup"><span data-stu-id="138c9-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-table-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="138c9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="138c9-141">Response</span></span>
<span data-ttu-id="138c9-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="138c9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
