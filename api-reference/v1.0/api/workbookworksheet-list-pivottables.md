---
title: List pivotTables
description: Recupere uma lista de objetos workbookpivottable.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1016bd4443b575fb62eb0c4aa31194a0a29df186
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581992"
---
# <a name="list-pivottables"></a><span data-ttu-id="57cea-103">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="57cea-103">List pivotTables</span></span>

<span data-ttu-id="57cea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57cea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="57cea-105">Recupere uma lista de objetos workbookpivottable.</span><span class="sxs-lookup"><span data-stu-id="57cea-105">Retrieve a list of workbookpivottable objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="57cea-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="57cea-106">Permissions</span></span>
<span data-ttu-id="57cea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57cea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="57cea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57cea-109">Permission type</span></span>      | <span data-ttu-id="57cea-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57cea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57cea-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57cea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="57cea-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57cea-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="57cea-113">Delegada (conta Microsoft pessoal)</span><span class="sxs-lookup"><span data-stu-id="57cea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57cea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57cea-114">Not supported.</span></span>    |
|<span data-ttu-id="57cea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57cea-115">Application</span></span> | <span data-ttu-id="57cea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57cea-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="57cea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57cea-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="57cea-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="57cea-118">Optional query parameters</span></span>
<span data-ttu-id="57cea-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="57cea-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="57cea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57cea-120">Request headers</span></span>
| <span data-ttu-id="57cea-121">Nome</span><span class="sxs-lookup"><span data-stu-id="57cea-121">Name</span></span>      |<span data-ttu-id="57cea-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="57cea-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="57cea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="57cea-123">Authorization</span></span>  | <span data-ttu-id="57cea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57cea-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="57cea-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="57cea-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="57cea-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="57cea-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57cea-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57cea-129">Request body</span></span>
<span data-ttu-id="57cea-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57cea-130">Do not supply a request body for this method.</span></span>
### <a name="response"></a><span data-ttu-id="57cea-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="57cea-131">Response</span></span>
<span data-ttu-id="57cea-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [workbookPivotTable](../resources/workbookpivottable.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57cea-132">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/workbookpivottable.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="57cea-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57cea-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="57cea-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57cea-134">Request</span></span>
<span data-ttu-id="57cea-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57cea-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="57cea-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="57cea-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_pivottables"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables
```
# <a name="c"></a>[<span data-ttu-id="57cea-137">C#</span><span class="sxs-lookup"><span data-stu-id="57cea-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-pivottables-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57cea-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57cea-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-pivottables-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57cea-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57cea-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-pivottables-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57cea-140">Java</span><span class="sxs-lookup"><span data-stu-id="57cea-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-pivottables-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="57cea-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="57cea-141">Response</span></span>
<span data-ttu-id="57cea-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57cea-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookPivotTable",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->