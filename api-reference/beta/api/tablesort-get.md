---
title: Obter TableSort
description: Recupere as propriedades e os relacionamentos do objeto tablesort.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 6d51560e1e57cd156326c3b1b56148234a9e0c7f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362903"
---
# <a name="get-tablesort"></a><span data-ttu-id="0a2fb-103">Obter TableSort</span><span class="sxs-lookup"><span data-stu-id="0a2fb-103">Get TableSort</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a2fb-104">Recupere as propriedades e os relacionamentos do objeto tablesort.</span><span class="sxs-lookup"><span data-stu-id="0a2fb-104">Retrieve the properties and relationships of tablesort object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0a2fb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0a2fb-105">Permissions</span></span>
<span data-ttu-id="0a2fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a2fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a2fb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a2fb-108">Permission type</span></span>      | <span data-ttu-id="0a2fb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a2fb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a2fb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a2fb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0a2fb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a2fb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0a2fb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a2fb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a2fb-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a2fb-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0a2fb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a2fb-114">Application</span></span> | <span data-ttu-id="0a2fb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a2fb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a2fb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a2fb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0a2fb-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0a2fb-117">Optional query parameters</span></span>
<span data-ttu-id="0a2fb-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0a2fb-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a2fb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a2fb-119">Request headers</span></span>
| <span data-ttu-id="0a2fb-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0a2fb-120">Name</span></span>      |<span data-ttu-id="0a2fb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a2fb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0a2fb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a2fb-122">Authorization</span></span>  | <span data-ttu-id="0a2fb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a2fb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0a2fb-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0a2fb-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="0a2fb-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0a2fb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a2fb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a2fb-128">Request body</span></span>
<span data-ttu-id="0a2fb-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0a2fb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a2fb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a2fb-130">Response</span></span>

<span data-ttu-id="0a2fb-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookTableSort](../resources/workbooktablesort.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a2fb-131">If successful, this method returns a `200 OK` response code and [workbookTableSort](../resources/workbooktablesort.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0a2fb-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a2fb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a2fb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a2fb-133">Request</span></span>
<span data-ttu-id="0a2fb-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a2fb-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0a2fb-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a2fb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tablesort"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0a2fb-136">C#</span><span class="sxs-lookup"><span data-stu-id="0a2fb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tablesort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a2fb-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a2fb-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tablesort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0a2fb-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0a2fb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tablesort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0a2fb-139">Java</span><span class="sxs-lookup"><span data-stu-id="0a2fb-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tablesort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0a2fb-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a2fb-140">Response</span></span>
<span data-ttu-id="0a2fb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a2fb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableSort"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "matchCase": true,
  "method": "method-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get TableSort",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
