---
title: Listar licenseDetails
description: Recupere uma lista de objetos licenseDetails.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f5fd5c332983e20b4988205eb01a150ce59c625b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888851"
---
# <a name="list-licensedetails"></a><span data-ttu-id="e4c4c-103">Listar licenseDetails</span><span class="sxs-lookup"><span data-stu-id="e4c4c-103">List licenseDetails</span></span>

<span data-ttu-id="e4c4c-104">Recupere uma lista de objetos licenseDetails.</span><span class="sxs-lookup"><span data-stu-id="e4c4c-104">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4c4c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4c4c-105">Permissions</span></span>
<span data-ttu-id="e4c4c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4c4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4c4c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4c4c-108">Permission type</span></span>      | <span data-ttu-id="e4c4c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4c4c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4c4c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4c4c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e4c4c-111">User. Read, User. Read. All, User. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="e4c4c-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e4c4c-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4c4c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4c4c-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="e4c4c-113">User.Read</span></span>    |
|<span data-ttu-id="e4c4c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4c4c-114">Application</span></span> | <span data-ttu-id="e4c4c-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4c4c-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4c4c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4c4c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e4c4c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e4c4c-117">Optional query parameters</span></span>
<span data-ttu-id="e4c4c-118">Este método não \*\*\*\* oferece suporte a [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="e4c4c-118">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4c4c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4c4c-119">Request headers</span></span>
| <span data-ttu-id="e4c4c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e4c4c-120">Name</span></span>      |<span data-ttu-id="e4c4c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4c4c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e4c4c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4c4c-122">Authorization</span></span>  | <span data-ttu-id="e4c4c-123">&lt;Código do portador&gt;</span><span class="sxs-lookup"><span data-stu-id="e4c4c-123">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4c4c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4c4c-124">Request body</span></span>
<span data-ttu-id="e4c4c-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4c4c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4c4c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4c4c-126">Response</span></span>

<span data-ttu-id="e4c4c-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [licenseDetails](../resources/licensedetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4c4c-127">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e4c4c-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4c4c-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4c4c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4c4c-129">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e4c4c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4c4c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/licenseDetails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e4c4c-131">C#</span><span class="sxs-lookup"><span data-stu-id="e4c4c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-licensedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e4c4c-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="e4c4c-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-licensedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e4c4c-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e4c4c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-licensedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e4c4c-134">Java</span><span class="sxs-lookup"><span data-stu-id="e4c4c-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-licensedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e4c4c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4c4c-135">Response</span></span>
<span data-ttu-id="e4c4c-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4c4c-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
