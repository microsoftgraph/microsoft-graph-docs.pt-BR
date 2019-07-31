---
title: List pivotTables
description: Recupere uma lista de objetos workbookpivottable.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2132766c43538f50ce2eb9f177581e9964d391e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35995850"
---
# <a name="list-pivottables"></a><span data-ttu-id="58c10-103">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="58c10-103">List pivotTables</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58c10-104">Recupere uma lista de objetos workbookpivottable.</span><span class="sxs-lookup"><span data-stu-id="58c10-104">Retrieve a list of workbookpivottable objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="58c10-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="58c10-105">Permissions</span></span>
<span data-ttu-id="58c10-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58c10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="58c10-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58c10-108">Permission type</span></span>      | <span data-ttu-id="58c10-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58c10-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58c10-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58c10-110">Delegated (work or school account)</span></span> | <span data-ttu-id="58c10-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58c10-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="58c10-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58c10-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58c10-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58c10-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="58c10-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58c10-114">Application</span></span> | <span data-ttu-id="58c10-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58c10-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="58c10-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58c10-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="58c10-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="58c10-117">Optional query parameters</span></span>
<span data-ttu-id="58c10-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="58c10-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58c10-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58c10-119">Request headers</span></span>
| <span data-ttu-id="58c10-120">Nome</span><span class="sxs-lookup"><span data-stu-id="58c10-120">Name</span></span>      |<span data-ttu-id="58c10-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="58c10-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="58c10-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="58c10-122">Authorization</span></span>  | <span data-ttu-id="58c10-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58c10-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="58c10-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="58c10-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="58c10-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="58c10-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="58c10-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58c10-128">Request body</span></span>
<span data-ttu-id="58c10-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="58c10-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58c10-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="58c10-130">Response</span></span>

<span data-ttu-id="58c10-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [workbookPivotTable](../resources/workbookpivottable.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58c10-131">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/workbookpivottable.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="58c10-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58c10-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58c10-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58c10-133">Request</span></span>
<span data-ttu-id="58c10-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58c10-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="58c10-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="58c10-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_pivottables"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="58c10-136">C#</span><span class="sxs-lookup"><span data-stu-id="58c10-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-pivottables-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="58c10-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="58c10-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-pivottables-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="58c10-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="58c10-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-pivottables-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="58c10-139">Java</span><span class="sxs-lookup"><span data-stu-id="58c10-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-pivottables-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="58c10-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="58c10-140">Response</span></span>
<span data-ttu-id="58c10-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58c10-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
