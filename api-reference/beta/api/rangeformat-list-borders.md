---
title: Listar bordas
description: Recupere uma lista de objetos rangeborder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ab55d5f33c7be588d2e32e5f7840d12e9fdf0ec6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454589"
---
# <a name="list-borders"></a><span data-ttu-id="b6f53-103">Listar bordas</span><span class="sxs-lookup"><span data-stu-id="b6f53-103">List borders</span></span>

<span data-ttu-id="b6f53-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b6f53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6f53-105">Recupere uma lista de objetos rangeborder.</span><span class="sxs-lookup"><span data-stu-id="b6f53-105">Retrieve a list of rangeborder objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b6f53-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6f53-106">Permissions</span></span>
<span data-ttu-id="b6f53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6f53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6f53-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6f53-109">Permission type</span></span>      | <span data-ttu-id="b6f53-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6f53-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6f53-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6f53-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b6f53-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6f53-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b6f53-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6f53-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6f53-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6f53-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b6f53-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6f53-115">Application</span></span> | <span data-ttu-id="b6f53-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6f53-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6f53-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6f53-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/borders
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/borders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b6f53-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b6f53-118">Optional query parameters</span></span>
<span data-ttu-id="b6f53-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6f53-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6f53-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f53-120">Request headers</span></span>
| <span data-ttu-id="b6f53-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b6f53-121">Name</span></span>      |<span data-ttu-id="b6f53-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6f53-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b6f53-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6f53-123">Authorization</span></span>  | <span data-ttu-id="b6f53-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6f53-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b6f53-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b6f53-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="b6f53-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b6f53-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6f53-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f53-129">Request body</span></span>
<span data-ttu-id="b6f53-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6f53-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6f53-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6f53-131">Response</span></span>

<span data-ttu-id="b6f53-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [workbookRangeBorder](../resources/workbookrangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6f53-132">If successful, this method returns a `200 OK` response code and collection of [workbookRangeBorder](../resources/workbookrangeborder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b6f53-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6f53-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6f53-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f53-134">Request</span></span>
<span data-ttu-id="b6f53-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6f53-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b6f53-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6f53-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_borders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/borders
```
# <a name="c"></a>[<span data-ttu-id="b6f53-137">C#</span><span class="sxs-lookup"><span data-stu-id="b6f53-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-borders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6f53-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6f53-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-borders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6f53-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6f53-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-borders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b6f53-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6f53-140">Response</span></span>
<span data-ttu-id="b6f53-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6f53-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 185

{
  "value": [
    {
      "id": "id-value",
      "color": "color-value",
      "style": "style-value",
      "sideIndex": "sideIndex-value",
      "weight": "weight-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List borders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
