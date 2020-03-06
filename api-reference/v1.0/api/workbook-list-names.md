---
title: Listar nomes
description: Recupere uma lista de objetos nameditem.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8d3a6d0ce1ae4dd9807f92e5f8af12e83fcff275
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508860"
---
# <a name="list-names"></a><span data-ttu-id="7fa31-103">Listar nomes</span><span class="sxs-lookup"><span data-stu-id="7fa31-103">List names</span></span>

<span data-ttu-id="7fa31-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fa31-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7fa31-105">Recupere uma lista de objetos nameditem.</span><span class="sxs-lookup"><span data-stu-id="7fa31-105">Retrieve a list of nameditem objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="7fa31-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7fa31-106">Permissions</span></span>
<span data-ttu-id="7fa31-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fa31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fa31-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fa31-109">Permission type</span></span>      | <span data-ttu-id="7fa31-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7fa31-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fa31-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fa31-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7fa31-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7fa31-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7fa31-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fa31-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fa31-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fa31-114">Not supported.</span></span>    |
|<span data-ttu-id="7fa31-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fa31-115">Application</span></span> | <span data-ttu-id="7fa31-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fa31-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fa31-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fa31-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7fa31-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7fa31-118">Optional query parameters</span></span>
<span data-ttu-id="7fa31-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7fa31-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7fa31-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fa31-120">Request headers</span></span>
| <span data-ttu-id="7fa31-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7fa31-121">Name</span></span>      |<span data-ttu-id="7fa31-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fa31-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7fa31-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fa31-123">Authorization</span></span>  | <span data-ttu-id="7fa31-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fa31-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7fa31-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7fa31-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="7fa31-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7fa31-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fa31-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fa31-129">Request body</span></span>
<span data-ttu-id="7fa31-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7fa31-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fa31-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fa31-131">Response</span></span>

<span data-ttu-id="7fa31-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [WorkbookNamedItem](../resources/nameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fa31-132">If successful, this method returns a `200 OK` response code and collection of [WorkbookNamedItem](../resources/nameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7fa31-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7fa31-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7fa31-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fa31-134">Request</span></span>
<span data-ttu-id="7fa31-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fa31-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7fa31-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fa31-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_names"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names
```
# <a name="c"></a>[<span data-ttu-id="7fa31-137">C#</span><span class="sxs-lookup"><span data-stu-id="7fa31-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-names-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7fa31-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fa31-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-names-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7fa31-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fa31-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-names-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7fa31-140">Java</span><span class="sxs-lookup"><span data-stu-id="7fa31-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-names-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7fa31-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fa31-141">Response</span></span>
<span data-ttu-id="7fa31-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fa31-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "value": [
    {
      "name": "name-value",
      "type": "type-value",
      "value": {
      },
      "visible": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List names",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
