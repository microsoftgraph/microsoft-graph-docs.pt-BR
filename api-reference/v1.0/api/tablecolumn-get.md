---
title: Obter TableColumn
description: Recupere as propriedades e os relacionamentos do objeto tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e7b86effb3dc28414dd45653cd3caabaf801434c
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50033899"
---
# <a name="get-tablecolumn"></a><span data-ttu-id="e7141-103">Obter TableColumn</span><span class="sxs-lookup"><span data-stu-id="e7141-103">Get TableColumn</span></span>

<span data-ttu-id="e7141-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7141-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e7141-105">Recupere as propriedades e os relacionamentos do objeto tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="e7141-105">Retrieve the properties and relationships of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e7141-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7141-106">Permissions</span></span>
<span data-ttu-id="e7141-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7141-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7141-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7141-109">Permission type</span></span>      | <span data-ttu-id="e7141-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7141-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7141-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7141-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e7141-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7141-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e7141-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7141-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7141-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7141-114">Not supported.</span></span>    |
|<span data-ttu-id="e7141-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7141-115">Application</span></span> | <span data-ttu-id="e7141-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7141-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7141-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7141-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns/{id|name}
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e7141-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e7141-118">Optional query parameters</span></span>
<span data-ttu-id="e7141-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e7141-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7141-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7141-120">Request headers</span></span>
| <span data-ttu-id="e7141-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e7141-121">Name</span></span>      |<span data-ttu-id="e7141-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7141-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e7141-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7141-123">Authorization</span></span>  | <span data-ttu-id="e7141-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7141-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7141-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e7141-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="e7141-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e7141-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7141-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7141-129">Request body</span></span>
<span data-ttu-id="e7141-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7141-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7141-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7141-131">Response</span></span>

<span data-ttu-id="e7141-132">Se bem-sucedido, este método retorna um código de resposta e um `200 OK` [objeto WorkbookTableColumn](../resources/workbooktablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7141-132">If successful, this method returns a `200 OK` response code and [WorkbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e7141-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7141-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7141-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7141-134">Request</span></span>
<span data-ttu-id="e7141-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7141-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e7141-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7141-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tablecolumn"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
```
# <a name="c"></a>[<span data-ttu-id="e7141-137">C#</span><span class="sxs-lookup"><span data-stu-id="e7141-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tablecolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7141-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7141-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tablecolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7141-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7141-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tablecolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e7141-140">Java</span><span class="sxs-lookup"><span data-stu-id="e7141-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tablecolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e7141-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7141-141">Response</span></span>
<span data-ttu-id="e7141-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7141-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": "99",
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
