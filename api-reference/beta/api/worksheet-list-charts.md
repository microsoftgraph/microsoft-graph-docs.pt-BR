---
title: Listar gráficos
description: Recupere uma lista de objetos de gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 059542d693645dd9ec6e10cb98e54b7de2d4bc29
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721824"
---
# <a name="list-charts"></a><span data-ttu-id="5b367-103">Listar gráficos</span><span class="sxs-lookup"><span data-stu-id="5b367-103">List charts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b367-104">Recupere uma lista de objetos de gráfico.</span><span class="sxs-lookup"><span data-stu-id="5b367-104">Retrieve a list of chart objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="5b367-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b367-105">Permissions</span></span>
<span data-ttu-id="5b367-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b367-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b367-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b367-108">Permission type</span></span>      | <span data-ttu-id="5b367-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b367-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b367-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b367-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5b367-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b367-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5b367-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b367-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b367-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b367-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5b367-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b367-114">Application</span></span> | <span data-ttu-id="5b367-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b367-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b367-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b367-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5b367-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5b367-117">Optional query parameters</span></span>
<span data-ttu-id="5b367-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5b367-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b367-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b367-119">Request headers</span></span>
| <span data-ttu-id="5b367-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5b367-120">Name</span></span>      |<span data-ttu-id="5b367-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b367-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5b367-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b367-122">Authorization</span></span>  | <span data-ttu-id="5b367-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b367-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5b367-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5b367-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="5b367-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5b367-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b367-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b367-128">Request body</span></span>
<span data-ttu-id="5b367-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b367-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b367-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b367-130">Response</span></span>

<span data-ttu-id="5b367-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [workbookChart](../resources/workbookchart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b367-131">If successful, this method returns a `200 OK` response code and collection of [workbookChart](../resources/workbookchart.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5b367-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b367-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b367-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b367-133">Request</span></span>
<span data-ttu-id="5b367-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b367-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5b367-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b367-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_charts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5b367-136">C#</span><span class="sxs-lookup"><span data-stu-id="5b367-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-charts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b367-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b367-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-charts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5b367-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5b367-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-charts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5b367-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b367-139">Response</span></span>
<span data-ttu-id="5b367-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b367-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 93

{
  "value": [
    {
      "id": "id-value",
      "height": 99,
      "left": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List charts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
