---
title: Obter gráfico
description: Recupera as propriedades e os relacionamentos do objeto de gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 722dc16b73cdbef53ea090413dee3df80eec025b
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726442"
---
# <a name="get-chart"></a><span data-ttu-id="ad1ca-103">Obter gráfico</span><span class="sxs-lookup"><span data-stu-id="ad1ca-103">Get Chart</span></span>

<span data-ttu-id="ad1ca-104">Recupera as propriedades e os relacionamentos do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="ad1ca-104">Retrieve the properties and relationships of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ad1ca-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad1ca-105">Permissions</span></span>
<span data-ttu-id="ad1ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad1ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad1ca-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad1ca-108">Permission type</span></span>      | <span data-ttu-id="ad1ca-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad1ca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad1ca-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad1ca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ad1ca-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad1ca-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ad1ca-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad1ca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad1ca-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad1ca-113">Not supported.</span></span>    |
|<span data-ttu-id="ad1ca-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad1ca-114">Application</span></span> | <span data-ttu-id="ad1ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad1ca-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad1ca-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad1ca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ad1ca-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ad1ca-117">Optional query parameters</span></span>
<span data-ttu-id="ad1ca-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ad1ca-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad1ca-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad1ca-119">Request headers</span></span>
| <span data-ttu-id="ad1ca-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ad1ca-120">Name</span></span>      |<span data-ttu-id="ad1ca-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad1ca-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ad1ca-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad1ca-122">Authorization</span></span>  | <span data-ttu-id="ad1ca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad1ca-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ad1ca-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ad1ca-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ad1ca-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ad1ca-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad1ca-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad1ca-128">Request body</span></span>
<span data-ttu-id="ad1ca-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ad1ca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad1ca-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad1ca-130">Response</span></span>

<span data-ttu-id="ad1ca-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookChart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad1ca-131">If successful, this method returns a `200 OK` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ad1ca-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad1ca-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad1ca-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad1ca-133">Request</span></span>
<span data-ttu-id="ad1ca-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad1ca-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ad1ca-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad1ca-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chart"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ad1ca-136">C#</span><span class="sxs-lookup"><span data-stu-id="ad1ca-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad1ca-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad1ca-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ad1ca-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ad1ca-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ad1ca-139">Java</span><span class="sxs-lookup"><span data-stu-id="ad1ca-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chart-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ad1ca-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad1ca-140">Response</span></span>
<span data-ttu-id="ad1ca-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad1ca-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
