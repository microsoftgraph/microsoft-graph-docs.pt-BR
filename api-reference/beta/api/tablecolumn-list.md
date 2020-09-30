---
title: Listar TableColumnCollection
description: Recupere uma lista de objetos tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 004dd5dda8270f012ab27d40b18b365169729e10
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315102"
---
# <a name="list-tablecolumncollection"></a><span data-ttu-id="24f6b-103">Listar TableColumnCollection</span><span class="sxs-lookup"><span data-stu-id="24f6b-103">List TableColumnCollection</span></span>

<span data-ttu-id="24f6b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24f6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24f6b-105">Recupere uma lista de objetos tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="24f6b-105">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="24f6b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="24f6b-106">Permissions</span></span>
<span data-ttu-id="24f6b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24f6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24f6b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24f6b-109">Permission type</span></span>      | <span data-ttu-id="24f6b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24f6b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24f6b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24f6b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="24f6b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24f6b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="24f6b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24f6b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24f6b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24f6b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="24f6b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24f6b-115">Application</span></span> | <span data-ttu-id="24f6b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24f6b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24f6b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24f6b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="24f6b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="24f6b-118">Optional query parameters</span></span>
<span data-ttu-id="24f6b-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="24f6b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24f6b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24f6b-120">Request headers</span></span>
| <span data-ttu-id="24f6b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="24f6b-121">Name</span></span>      |<span data-ttu-id="24f6b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="24f6b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="24f6b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="24f6b-123">Authorization</span></span>  | <span data-ttu-id="24f6b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24f6b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="24f6b-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="24f6b-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="24f6b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="24f6b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24f6b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24f6b-129">Request body</span></span>
<span data-ttu-id="24f6b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24f6b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24f6b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="24f6b-131">Response</span></span>

<span data-ttu-id="24f6b-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [workbookTableColumn](../resources/workbooktablecolumn.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24f6b-132">If successful, this method returns a `200 OK` response code and collection of [workbookTableColumn](../resources/workbooktablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="24f6b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24f6b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24f6b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24f6b-134">Request</span></span>
<span data-ttu-id="24f6b-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24f6b-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="24f6b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="24f6b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tablecolumncollection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns
```
# <a name="c"></a>[<span data-ttu-id="24f6b-137">C#</span><span class="sxs-lookup"><span data-stu-id="24f6b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tablecolumncollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="24f6b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24f6b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tablecolumncollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24f6b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24f6b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tablecolumncollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="24f6b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="24f6b-140">Response</span></span>
<span data-ttu-id="24f6b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24f6b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 126

{
  "value": [
    {
      "id": 99,
      "name": "name-value",
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List TableColumnCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->