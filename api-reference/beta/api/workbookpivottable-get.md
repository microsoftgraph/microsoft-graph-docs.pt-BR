---
title: Obter workbookPivotTable
description: Recupere as propriedades e relações do objeto workbookPivotTable.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 3cdeb0ba5cb4ad854672c327d4c0edfe69a770ec
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421621"
---
# <a name="get-workbookpivottable"></a><span data-ttu-id="0e544-103">Obter workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="0e544-103">Get workbookPivotTable</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e544-104">Recupere as propriedades e relações do objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="0e544-104">Retrieve the properties and relationships of workbookPivotTable object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e544-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e544-105">Permissions</span></span>
<span data-ttu-id="0e544-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e544-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0e544-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e544-108">Permission type</span></span>      | <span data-ttu-id="0e544-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e544-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e544-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e544-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0e544-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e544-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e544-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e544-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e544-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e544-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e544-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e544-114">Application</span></span> | <span data-ttu-id="0e544-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e544-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e544-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e544-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0e544-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0e544-117">Optional query parameters</span></span>
<span data-ttu-id="0e544-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0e544-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e544-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e544-119">Request headers</span></span>
| <span data-ttu-id="0e544-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0e544-120">Name</span></span>      |<span data-ttu-id="0e544-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e544-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0e544-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e544-122">Authorization</span></span>  | <span data-ttu-id="0e544-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e544-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e544-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0e544-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="0e544-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0e544-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e544-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e544-128">Request body</span></span>
<span data-ttu-id="0e544-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0e544-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e544-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e544-130">Response</span></span>

<span data-ttu-id="0e544-131">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [workbookPivotTable](../resources/workbookpivottable.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e544-131">If successful, this method returns a `200 OK` response code and [workbookPivotTable](../resources/workbookpivottable.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0e544-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e544-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e544-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e544-133">Request</span></span>
<span data-ttu-id="0e544-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e544-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0e544-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e544-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookpivottable"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0e544-136">C#</span><span class="sxs-lookup"><span data-stu-id="0e544-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookpivottable-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e544-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e544-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookpivottable-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0e544-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0e544-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookpivottable-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0e544-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e544-139">Response</span></span>
<span data-ttu-id="0e544-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e544-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookPivotTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
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
