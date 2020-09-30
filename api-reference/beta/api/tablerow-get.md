---
title: Obter TableRow
description: Recupere as propriedades e os relacionamentos do objeto tablerow.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: aa3186e9ed37c2491bfc8b267c927ce81f3b4445
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314691"
---
# <a name="get-tablerow"></a><span data-ttu-id="c5f2b-103">Obter TableRow</span><span class="sxs-lookup"><span data-stu-id="c5f2b-103">Get TableRow</span></span>

<span data-ttu-id="c5f2b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5f2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5f2b-105">Recupere as propriedades e os relacionamentos do objeto tablerow.</span><span class="sxs-lookup"><span data-stu-id="c5f2b-105">Retrieve the properties and relationships of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5f2b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5f2b-106">Permissions</span></span>
<span data-ttu-id="c5f2b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5f2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5f2b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5f2b-109">Permission type</span></span>      | <span data-ttu-id="c5f2b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5f2b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5f2b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5f2b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c5f2b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5f2b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c5f2b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5f2b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5f2b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5f2b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c5f2b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5f2b-115">Application</span></span> | <span data-ttu-id="c5f2b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5f2b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5f2b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5f2b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows/{index}
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c5f2b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c5f2b-118">Optional query parameters</span></span>
<span data-ttu-id="c5f2b-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c5f2b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5f2b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5f2b-120">Request headers</span></span>
| <span data-ttu-id="c5f2b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c5f2b-121">Name</span></span>      |<span data-ttu-id="c5f2b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5f2b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c5f2b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5f2b-123">Authorization</span></span>  | <span data-ttu-id="c5f2b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5f2b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c5f2b-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c5f2b-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="c5f2b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c5f2b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5f2b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5f2b-129">Request body</span></span>
<span data-ttu-id="c5f2b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5f2b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5f2b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5f2b-131">Response</span></span>

<span data-ttu-id="c5f2b-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookTableRow](../resources/workbooktablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5f2b-132">If successful, this method returns a `200 OK` response code and [workbookTableRow](../resources/workbooktablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5f2b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5f2b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5f2b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5f2b-134">Request</span></span>
<span data-ttu-id="c5f2b-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5f2b-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c5f2b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5f2b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tablerow"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}
```
# <a name="c"></a>[<span data-ttu-id="c5f2b-137">C#</span><span class="sxs-lookup"><span data-stu-id="c5f2b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tablerow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5f2b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5f2b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tablerow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5f2b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5f2b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tablerow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c5f2b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5f2b-140">Response</span></span>
<span data-ttu-id="c5f2b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5f2b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get TableRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->