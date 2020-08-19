---
title: Obter FormatProtection
description: Recupere as propriedades e os relacionamentos do objeto formatprotection.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: bbc7337675e55799615f201d6655dc85e864d7e9
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806167"
---
# <a name="get-formatprotection"></a><span data-ttu-id="5aa2e-103">Get FormatProtection</span><span class="sxs-lookup"><span data-stu-id="5aa2e-103">Get FormatProtection</span></span>

<span data-ttu-id="5aa2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5aa2e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5aa2e-105">Recupere as propriedades e os relacionamentos do objeto formatprotection.</span><span class="sxs-lookup"><span data-stu-id="5aa2e-105">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5aa2e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5aa2e-106">Permissions</span></span>
<span data-ttu-id="5aa2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5aa2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5aa2e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5aa2e-109">Permission type</span></span>      | <span data-ttu-id="5aa2e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5aa2e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5aa2e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5aa2e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5aa2e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5aa2e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5aa2e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5aa2e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5aa2e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5aa2e-114">Not supported.</span></span>    |
|<span data-ttu-id="5aa2e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5aa2e-115">Application</span></span> | <span data-ttu-id="5aa2e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5aa2e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5aa2e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5aa2e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/protection
GET /workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5aa2e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5aa2e-118">Optional query parameters</span></span>
<span data-ttu-id="5aa2e-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5aa2e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5aa2e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5aa2e-120">Request headers</span></span>
| <span data-ttu-id="5aa2e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5aa2e-121">Name</span></span>      |<span data-ttu-id="5aa2e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5aa2e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5aa2e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5aa2e-123">Authorization</span></span>  | <span data-ttu-id="5aa2e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5aa2e-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5aa2e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5aa2e-126">Request body</span></span>
<span data-ttu-id="5aa2e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5aa2e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5aa2e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aa2e-128">Response</span></span>

<span data-ttu-id="5aa2e-129">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [FormatProtection](../resources/formatprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5aa2e-129">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5aa2e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5aa2e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5aa2e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5aa2e-131">Request</span></span>
<span data-ttu-id="5aa2e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5aa2e-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5aa2e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5aa2e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/protection
```
# <a name="c"></a>[<span data-ttu-id="5aa2e-134">C#</span><span class="sxs-lookup"><span data-stu-id="5aa2e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-formatprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5aa2e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5aa2e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-formatprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5aa2e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5aa2e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-formatprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5aa2e-137">Java</span><span class="sxs-lookup"><span data-stu-id="5aa2e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-formatprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5aa2e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aa2e-138">Response</span></span>
<span data-ttu-id="5aa2e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5aa2e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookFormatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get FormatProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
