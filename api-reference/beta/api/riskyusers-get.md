---
title: Obter riskyUser
description: Recupere as propriedades e os relacionamentos de um objeto **riskyUser** .
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f20615692853ca662a5a2c9ccb5eb26cc80e2528
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017225"
---
# <a name="get-riskyuser"></a><span data-ttu-id="6ed1e-103">Obter riskyUser</span><span class="sxs-lookup"><span data-stu-id="6ed1e-103">Get riskyUser</span></span>

<span data-ttu-id="6ed1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ed1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ed1e-105">Recupere as propriedades e os relacionamentos de um objeto **riskyUser** .</span><span class="sxs-lookup"><span data-stu-id="6ed1e-105">Retrieve the properties and relationships of a **riskyUser** object.</span></span>

><span data-ttu-id="6ed1e-106">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="6ed1e-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ed1e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6ed1e-107">Permissions</span></span>
<span data-ttu-id="6ed1e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ed1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ed1e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ed1e-110">Permission type</span></span>      | <span data-ttu-id="6ed1e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ed1e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ed1e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ed1e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6ed1e-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ed1e-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="6ed1e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ed1e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ed1e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ed1e-115">Not supported.</span></span>    |
|<span data-ttu-id="6ed1e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ed1e-116">Application</span></span> | <span data-ttu-id="6ed1e-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ed1e-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ed1e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ed1e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}
GET /identityProtection/riskyUsers/{id}
```


## <a name="request-headers"></a><span data-ttu-id="6ed1e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ed1e-119">Request headers</span></span>
| <span data-ttu-id="6ed1e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6ed1e-120">Name</span></span>      |<span data-ttu-id="6ed1e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ed1e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6ed1e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ed1e-122">Authorization</span></span>  | <span data-ttu-id="6ed1e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ed1e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6ed1e-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6ed1e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6ed1e-126">ID da sessão da pasta de trabalho que determina se as alterações são persistentes.</span><span class="sxs-lookup"><span data-stu-id="6ed1e-126">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="6ed1e-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6ed1e-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ed1e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ed1e-128">Request body</span></span>
<span data-ttu-id="6ed1e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6ed1e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ed1e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ed1e-130">Response</span></span>

<span data-ttu-id="6ed1e-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [riskyUser](../resources/riskyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ed1e-131">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="6ed1e-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6ed1e-132">Examples</span></span>
### <a name="example-1-get-a-risky-user"></a><span data-ttu-id="6ed1e-133">Exemplo 1: obter um usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="6ed1e-133">Example 1: Get a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="6ed1e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ed1e-134">Request</span></span>
<span data-ttu-id="6ed1e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ed1e-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6ed1e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ed1e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="c"></a>[<span data-ttu-id="6ed1e-137">C#</span><span class="sxs-lookup"><span data-stu-id="6ed1e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ed1e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ed1e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ed1e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ed1e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6ed1e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ed1e-140">Response</span></span>
<span data-ttu-id="6ed1e-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ed1e-141">Here is an example of the response.</span></span>
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
  "isProcessing": true,
  "isDeleted": true,
  "riskDetail": "adminConfirmedSigninCompromised",
  "riskLevel": "high",
  "riskState": "atRisk",
  "userDisplayName": "Alex Wilbur",
  "userPrincipalName": "alexw@contoso.com"
}
```
### <a name="example-2-get-risky-users"></a><span data-ttu-id="6ed1e-142">Exemplo 2: obter usuários arriscados</span><span class="sxs-lookup"><span data-stu-id="6ed1e-142">Example 2: Get risky users</span></span>
#### <a name="request"></a><span data-ttu-id="6ed1e-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ed1e-143">Request</span></span>
<span data-ttu-id="6ed1e-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ed1e-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6ed1e-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ed1e-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers
```
# <a name="c"></a>[<span data-ttu-id="6ed1e-146">C#</span><span class="sxs-lookup"><span data-stu-id="6ed1e-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ed1e-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ed1e-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ed1e-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ed1e-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6ed1e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ed1e-149">Response</span></span>
<span data-ttu-id="6ed1e-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ed1e-150">Here is an example of the response.</span></span>
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



