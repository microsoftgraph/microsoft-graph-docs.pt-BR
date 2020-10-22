---
title: Listar nomes
description: Recupere uma lista de objetos nameditem.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1e030676d941ab012049bf91c8ae564155c2d0da
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634590"
---
# <a name="list-names"></a><span data-ttu-id="d6e69-103">Listar nomes</span><span class="sxs-lookup"><span data-stu-id="d6e69-103">List names</span></span>

<span data-ttu-id="d6e69-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6e69-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d6e69-105">Recupere uma lista de objetos nameditem.</span><span class="sxs-lookup"><span data-stu-id="d6e69-105">Retrieve a list of nameditem objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="d6e69-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6e69-106">Permissions</span></span>
<span data-ttu-id="d6e69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6e69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6e69-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6e69-109">Permission type</span></span>      | <span data-ttu-id="d6e69-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6e69-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6e69-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6e69-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d6e69-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6e69-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d6e69-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6e69-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6e69-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6e69-114">Not supported.</span></span>    |
|<span data-ttu-id="d6e69-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6e69-115">Application</span></span> | <span data-ttu-id="d6e69-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6e69-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6e69-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6e69-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d6e69-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d6e69-118">Optional query parameters</span></span>
<span data-ttu-id="d6e69-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d6e69-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6e69-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6e69-120">Request headers</span></span>
| <span data-ttu-id="d6e69-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d6e69-121">Name</span></span>      |<span data-ttu-id="d6e69-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6e69-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d6e69-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6e69-123">Authorization</span></span>  | <span data-ttu-id="d6e69-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6e69-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d6e69-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d6e69-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="d6e69-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d6e69-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6e69-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6e69-129">Request body</span></span>
<span data-ttu-id="d6e69-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d6e69-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6e69-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6e69-131">Response</span></span>

<span data-ttu-id="d6e69-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [WorkbookNamedItem](../resources/nameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6e69-132">If successful, this method returns a `200 OK` response code and collection of [WorkbookNamedItem](../resources/nameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d6e69-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6e69-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6e69-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6e69-134">Request</span></span>
<span data-ttu-id="d6e69-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6e69-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d6e69-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6e69-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_names"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names
```
# <a name="c"></a>[<span data-ttu-id="d6e69-137">C#</span><span class="sxs-lookup"><span data-stu-id="d6e69-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-names-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6e69-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6e69-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-names-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6e69-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6e69-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-names-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6e69-140">Java</span><span class="sxs-lookup"><span data-stu-id="d6e69-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-names-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d6e69-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6e69-141">Response</span></span>
<span data-ttu-id="d6e69-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6e69-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
