---
title: Listar licenseDetails
description: Recupere uma lista de objetos licenseDetails.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 48c2a6ce218b5e71fc58d5529f9301ba18265797
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082410"
---
# <a name="list-licensedetails"></a><span data-ttu-id="875cc-103">Listar licenseDetails</span><span class="sxs-lookup"><span data-stu-id="875cc-103">List licenseDetails</span></span>

<span data-ttu-id="875cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="875cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="875cc-105">Recupere uma lista de objetos **licenseDetails** para usuários empresariais.</span><span class="sxs-lookup"><span data-stu-id="875cc-105">Retrieve a list of **licenseDetails** objects for enterprise users.</span></span>

## <a name="permissions"></a><span data-ttu-id="875cc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="875cc-106">Permissions</span></span>
<span data-ttu-id="875cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="875cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="875cc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="875cc-109">Permission type</span></span>      | <span data-ttu-id="875cc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="875cc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="875cc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="875cc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="875cc-112">User. Read, User. Read. All, User. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="875cc-112">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="875cc-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="875cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="875cc-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="875cc-114">User.Read</span></span>    |
|<span data-ttu-id="875cc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="875cc-115">Application</span></span> | <span data-ttu-id="875cc-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="875cc-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="875cc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="875cc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="875cc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="875cc-118">Optional query parameters</span></span>
<span data-ttu-id="875cc-119">Este **método não oferece suporte a** parâmetros de [consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="875cc-119">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="875cc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="875cc-120">Request headers</span></span>
| <span data-ttu-id="875cc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="875cc-121">Name</span></span>      |<span data-ttu-id="875cc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="875cc-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="875cc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="875cc-123">Authorization</span></span>  | <span data-ttu-id="875cc-124">&lt;Código do portador&gt;</span><span class="sxs-lookup"><span data-stu-id="875cc-124">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="875cc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="875cc-125">Request body</span></span>
<span data-ttu-id="875cc-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="875cc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="875cc-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="875cc-127">Response</span></span>

<span data-ttu-id="875cc-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [licenseDetails](../resources/licensedetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="875cc-128">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="875cc-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="875cc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="875cc-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="875cc-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="875cc-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="875cc-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/licenseDetails
```
# <a name="c"></a>[<span data-ttu-id="875cc-132">C#</span><span class="sxs-lookup"><span data-stu-id="875cc-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-licensedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="875cc-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="875cc-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-licensedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="875cc-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="875cc-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-licensedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="875cc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="875cc-135">Response</span></span>
<span data-ttu-id="875cc-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="875cc-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licenseDetails",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "value": [
    {
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
