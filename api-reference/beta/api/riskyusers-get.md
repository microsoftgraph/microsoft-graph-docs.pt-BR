---
title: Obter riskyUser
description: Recupere as propriedades e os relacionamentos de um objeto **riskyUser** .
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cbbb05f34b66b97dbaeeb55da4dececbeabe01ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991748"
---
# <a name="get-riskyuser"></a><span data-ttu-id="c0d00-103">Obter riskyUser</span><span class="sxs-lookup"><span data-stu-id="c0d00-103">Get riskyUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0d00-104">Recupere as propriedades e os relacionamentos de um objeto **riskyUser** .</span><span class="sxs-lookup"><span data-stu-id="c0d00-104">Retrieve the properties and relationships of a **riskyUser** object.</span></span>

><span data-ttu-id="c0d00-105">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="c0d00-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0d00-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0d00-106">Permissions</span></span>
<span data-ttu-id="c0d00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0d00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0d00-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0d00-109">Permission type</span></span>      | <span data-ttu-id="c0d00-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0d00-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0d00-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0d00-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c0d00-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0d00-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="c0d00-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0d00-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0d00-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0d00-114">Not supported.</span></span>    |
|<span data-ttu-id="c0d00-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0d00-115">Application</span></span> | <span data-ttu-id="c0d00-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0d00-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0d00-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0d00-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}
```


## <a name="request-headers"></a><span data-ttu-id="c0d00-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0d00-118">Request headers</span></span>
| <span data-ttu-id="c0d00-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c0d00-119">Name</span></span>      |<span data-ttu-id="c0d00-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0d00-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c0d00-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0d00-121">Authorization</span></span>  | <span data-ttu-id="c0d00-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0d00-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c0d00-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c0d00-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c0d00-125">ID da sessão da pasta de trabalho que determina se as alterações são persistentes.</span><span class="sxs-lookup"><span data-stu-id="c0d00-125">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="c0d00-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c0d00-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0d00-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0d00-127">Request body</span></span>
<span data-ttu-id="c0d00-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0d00-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0d00-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0d00-129">Response</span></span>

<span data-ttu-id="c0d00-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [riskyUser](../resources/riskyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0d00-130">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0d00-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0d00-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0d00-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0d00-132">Request</span></span>
<span data-ttu-id="c0d00-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0d00-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c0d00-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0d00-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c0d00-135">C#</span><span class="sxs-lookup"><span data-stu-id="c0d00-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0d00-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0d00-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c0d00-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c0d00-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c0d00-138">Java</span><span class="sxs-lookup"><span data-stu-id="c0d00-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c0d00-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0d00-139">Response</span></span>
<span data-ttu-id="c0d00-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0d00-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
  "isGuest": true,
  "isProcessing": true,
  "isDeleted": true,
  "riskDetail": "adminConfirmedSigninCompromised",
  "riskLevel": "high",
  "riskState": "atRisk",
  "userDisplayName": "Alex Wilbur",
  "userPrincipalName": "alexw@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

