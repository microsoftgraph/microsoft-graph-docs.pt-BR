---
title: Linhas da lista rangeView
description: Recupere uma lista de objetos da exibição de intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b3c1f8a053172d5313b8f2be6d07d21203e4b6cf
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889690"
---
# <a name="list-rangeview-rows"></a><span data-ttu-id="962b3-103">Linhas da lista rangeView</span><span class="sxs-lookup"><span data-stu-id="962b3-103">List rangeView rows</span></span>

<span data-ttu-id="962b3-104">Recupere uma lista de objetos da exibição de intervalo.</span><span class="sxs-lookup"><span data-stu-id="962b3-104">Retrieve a list of range view objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="962b3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="962b3-105">Permissions</span></span>
<span data-ttu-id="962b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="962b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="962b3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="962b3-108">Permission type</span></span>      | <span data-ttu-id="962b3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="962b3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="962b3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="962b3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="962b3-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="962b3-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="962b3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="962b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="962b3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="962b3-113">Not supported.</span></span>    |
|<span data-ttu-id="962b3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="962b3-114">Application</span></span> | <span data-ttu-id="962b3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="962b3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="962b3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="962b3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/rows

```
## <a name="optional-query-parameters"></a><span data-ttu-id="962b3-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="962b3-117">Optional query parameters</span></span>
<span data-ttu-id="962b3-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="962b3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="962b3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="962b3-119">Request headers</span></span>
| <span data-ttu-id="962b3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="962b3-120">Name</span></span>      |<span data-ttu-id="962b3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="962b3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="962b3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="962b3-122">Authorization</span></span>  | <span data-ttu-id="962b3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="962b3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="962b3-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="962b3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="962b3-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="962b3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="962b3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="962b3-128">Request body</span></span>
<span data-ttu-id="962b3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="962b3-129">Do not supply a request body for this method.</span></span>
### <a name="response"></a><span data-ttu-id="962b3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="962b3-130">Response</span></span>
<span data-ttu-id="962b3-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="962b3-131">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/workbookrangeview.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="962b3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="962b3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="962b3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="962b3-133">Request</span></span>
<span data-ttu-id="962b3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="962b3-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="962b3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="962b3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/rows
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="962b3-136">C#</span><span class="sxs-lookup"><span data-stu-id="962b3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="962b3-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="962b3-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="962b3-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="962b3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="962b3-139">Java</span><span class="sxs-lookup"><span data-stu-id="962b3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="962b3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="962b3-140">Response</span></span>
<span data-ttu-id="962b3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="962b3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
