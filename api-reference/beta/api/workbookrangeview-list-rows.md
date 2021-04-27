---
title: Linhas da lista rangeView
description: Recupere uma lista de objetos da exibição de intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 02d20166119580c69326a3e8fa9e4f7e74845145
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053297"
---
# <a name="list-rangeview-rows"></a><span data-ttu-id="84978-103">Linhas da lista rangeView</span><span class="sxs-lookup"><span data-stu-id="84978-103">List rangeView rows</span></span>

<span data-ttu-id="84978-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84978-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84978-105">Recupere uma lista de objetos da exibição de intervalo.</span><span class="sxs-lookup"><span data-stu-id="84978-105">Retrieve a list of range view objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="84978-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="84978-106">Permissions</span></span>
<span data-ttu-id="84978-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84978-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84978-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84978-109">Permission type</span></span>      | <span data-ttu-id="84978-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="84978-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84978-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84978-111">Delegated (work or school account)</span></span> | <span data-ttu-id="84978-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84978-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="84978-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84978-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84978-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84978-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="84978-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84978-115">Application</span></span> | <span data-ttu-id="84978-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84978-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84978-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84978-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range(address={address})/visibleView/rows
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range(address={address})/visibleView/rows

```
## <a name="optional-query-parameters"></a><span data-ttu-id="84978-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="84978-118">Optional query parameters</span></span>
<span data-ttu-id="84978-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="84978-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84978-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84978-120">Request headers</span></span>
| <span data-ttu-id="84978-121">Nome</span><span class="sxs-lookup"><span data-stu-id="84978-121">Name</span></span>      |<span data-ttu-id="84978-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="84978-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="84978-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="84978-123">Authorization</span></span>  | <span data-ttu-id="84978-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84978-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="84978-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="84978-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="84978-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="84978-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="84978-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84978-129">Request body</span></span>
<span data-ttu-id="84978-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="84978-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84978-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="84978-131">Response</span></span>

<span data-ttu-id="84978-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84978-132">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/workbookrangeview.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="84978-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84978-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84978-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84978-134">Request</span></span>
<span data-ttu-id="84978-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84978-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="84978-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="84978-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/rows 
```
# <a name="c"></a>[<span data-ttu-id="84978-137">C#</span><span class="sxs-lookup"><span data-stu-id="84978-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84978-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84978-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84978-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84978-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84978-140">Java</span><span class="sxs-lookup"><span data-stu-id="84978-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="84978-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="84978-141">Response</span></span>
<span data-ttu-id="84978-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84978-142">Here is an example of the response.</span></span> <span data-ttu-id="84978-143">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="84978-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 247

{
  "value": [
    {
      "cellAddresses": "cellAddresses-value",
      "columnCount": 99,
      "formulas": "formulas-value",
      "formulasLocal": "formulasLocal-value",
      "formulasR1C1": "formulasR1C1-value",
      "index": 99
    }
  ]
}
```
