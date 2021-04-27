---
title: Listar gráficos
description: Recupere uma lista de objetos de gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 23cb5d346d4b4f3eb414476e5d67bd816c522620
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051659"
---
# <a name="list-charts"></a><span data-ttu-id="e8541-103">Listar gráficos</span><span class="sxs-lookup"><span data-stu-id="e8541-103">List charts</span></span>

<span data-ttu-id="e8541-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8541-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8541-105">Recupere uma lista de objetos de gráfico.</span><span class="sxs-lookup"><span data-stu-id="e8541-105">Retrieve a list of chart objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e8541-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8541-106">Permissions</span></span>
<span data-ttu-id="e8541-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8541-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8541-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8541-109">Permission type</span></span>      | <span data-ttu-id="e8541-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8541-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8541-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8541-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e8541-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8541-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e8541-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8541-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8541-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8541-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e8541-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8541-115">Application</span></span> | <span data-ttu-id="e8541-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8541-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8541-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8541-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e8541-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8541-118">Optional query parameters</span></span>
<span data-ttu-id="e8541-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8541-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8541-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8541-120">Request headers</span></span>
| <span data-ttu-id="e8541-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e8541-121">Name</span></span>      |<span data-ttu-id="e8541-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8541-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e8541-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8541-123">Authorization</span></span>  | <span data-ttu-id="e8541-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8541-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8541-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e8541-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="e8541-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e8541-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8541-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8541-129">Request body</span></span>
<span data-ttu-id="e8541-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8541-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8541-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8541-131">Response</span></span>

<span data-ttu-id="e8541-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [workbookChart](../resources/workbookchart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8541-132">If successful, this method returns a `200 OK` response code and collection of [workbookChart](../resources/workbookchart.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8541-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8541-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8541-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8541-134">Request</span></span>
<span data-ttu-id="e8541-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8541-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e8541-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8541-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_charts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
```
# <a name="c"></a>[<span data-ttu-id="e8541-137">C#</span><span class="sxs-lookup"><span data-stu-id="e8541-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-charts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8541-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8541-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-charts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8541-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8541-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-charts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8541-140">Java</span><span class="sxs-lookup"><span data-stu-id="e8541-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-charts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e8541-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8541-141">Response</span></span>
<span data-ttu-id="e8541-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8541-142">Here is an example of the response.</span></span> <span data-ttu-id="e8541-143">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e8541-143">Note: The response object shown here might be shortened for readability.</span></span>
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
