---
title: Listar licenseDetails
description: Recupere uma lista de objetos licenseDetails.
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 60462c865352a7391f3448280b85cce0fc3b21a8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982200"
---
# <a name="list-licensedetails"></a><span data-ttu-id="73584-103">Listar licenseDetails</span><span class="sxs-lookup"><span data-stu-id="73584-103">List licenseDetails</span></span>

<span data-ttu-id="73584-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73584-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73584-105">Recupere uma lista de objetos **licenseDetails** para usuários empresariais.</span><span class="sxs-lookup"><span data-stu-id="73584-105">Retrieve a list of **licenseDetails** objects for enterprise users.</span></span>

## <a name="permissions"></a><span data-ttu-id="73584-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="73584-106">Permissions</span></span>
<span data-ttu-id="73584-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73584-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73584-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73584-109">Permission type</span></span>      | <span data-ttu-id="73584-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73584-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73584-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73584-111">Delegated (work or school account)</span></span> | <span data-ttu-id="73584-112">User. Read, User. Read. All, User. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="73584-112">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="73584-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73584-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73584-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="73584-114">User.Read</span></span>    |
|<span data-ttu-id="73584-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73584-115">Application</span></span> | <span data-ttu-id="73584-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73584-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73584-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73584-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="73584-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="73584-118">Optional query parameters</span></span>
<span data-ttu-id="73584-119">Este método dá suporte ao `$select` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="73584-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="73584-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="73584-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="73584-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73584-121">Request headers</span></span>
| <span data-ttu-id="73584-122">Nome</span><span class="sxs-lookup"><span data-stu-id="73584-122">Name</span></span>      |<span data-ttu-id="73584-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="73584-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="73584-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="73584-124">Authorization</span></span>  | <span data-ttu-id="73584-125">Código do portador &lt;&gt;</span><span class="sxs-lookup"><span data-stu-id="73584-125">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="73584-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73584-126">Request body</span></span>
<span data-ttu-id="73584-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="73584-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73584-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="73584-128">Response</span></span>

<span data-ttu-id="73584-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [licenseDetails](../resources/licensedetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73584-129">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="73584-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73584-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73584-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73584-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="73584-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="73584-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/licenseDetails
```
# <a name="c"></a>[<span data-ttu-id="73584-133">C#</span><span class="sxs-lookup"><span data-stu-id="73584-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-licensedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73584-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73584-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-licensedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73584-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73584-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-licensedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73584-136">Java</span><span class="sxs-lookup"><span data-stu-id="73584-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-licensedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="73584-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="73584-137">Response</span></span>
<span data-ttu-id="73584-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73584-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


