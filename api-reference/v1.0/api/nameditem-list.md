---
title: Listar NamedItemCollection
description: Recupere uma lista de objetos nameditem.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 6793a2679b65b29228a11774d0980e04fc6b53a3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055894"
---
# <a name="list-nameditemcollection"></a><span data-ttu-id="ddc92-103">Listar NamedItemCollection</span><span class="sxs-lookup"><span data-stu-id="ddc92-103">List NamedItemCollection</span></span>

<span data-ttu-id="ddc92-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddc92-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ddc92-105">Recupere uma lista de objetos nameditem.</span><span class="sxs-lookup"><span data-stu-id="ddc92-105">Retrieve a list of nameditem objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ddc92-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ddc92-106">Permissions</span></span>
<span data-ttu-id="ddc92-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddc92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddc92-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddc92-109">Permission type</span></span>      | <span data-ttu-id="ddc92-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ddc92-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddc92-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddc92-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ddc92-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddc92-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ddc92-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddc92-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddc92-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddc92-114">Not supported.</span></span>    |
|<span data-ttu-id="ddc92-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddc92-115">Application</span></span> | <span data-ttu-id="ddc92-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddc92-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddc92-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddc92-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names
GET /me/drive/root:/{item-path}:/workbook/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ddc92-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ddc92-118">Optional query parameters</span></span>
<span data-ttu-id="ddc92-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ddc92-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddc92-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddc92-120">Request headers</span></span>
| <span data-ttu-id="ddc92-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ddc92-121">Name</span></span>      |<span data-ttu-id="ddc92-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddc92-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ddc92-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddc92-123">Authorization</span></span>  | <span data-ttu-id="ddc92-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddc92-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ddc92-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ddc92-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="ddc92-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ddc92-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddc92-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddc92-129">Request body</span></span>
<span data-ttu-id="ddc92-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ddc92-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddc92-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddc92-131">Response</span></span>

<span data-ttu-id="ddc92-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [WorkbookNamedItem](../resources/nameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddc92-132">If successful, this method returns a `200 OK` response code and collection of [WorkbookNamedItem](../resources/nameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ddc92-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ddc92-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ddc92-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddc92-134">Request</span></span>
<span data-ttu-id="ddc92-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddc92-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ddc92-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddc92-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_nameditemcollection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names
```
# <a name="c"></a>[<span data-ttu-id="ddc92-137">C#</span><span class="sxs-lookup"><span data-stu-id="ddc92-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-nameditemcollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddc92-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddc92-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-nameditemcollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddc92-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddc92-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-nameditemcollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ddc92-140">Java</span><span class="sxs-lookup"><span data-stu-id="ddc92-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-nameditemcollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ddc92-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddc92-141">Response</span></span>
<span data-ttu-id="ddc92-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddc92-142">Here is an example of the response.</span></span> <span data-ttu-id="ddc92-143">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ddc92-143">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "List NamedItemCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
