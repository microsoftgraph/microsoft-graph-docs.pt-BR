---
title: Listar riskyUsers
description: Recupere as propriedades e os relacionamentos de uma coleção de objetos **riskyUser** .
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d3b7f0e41525d1847ba3217f6e35ffc72028e888
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979169"
---
# <a name="list-riskyusers"></a><span data-ttu-id="78d86-103">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="78d86-103">List riskyUsers</span></span>

<span data-ttu-id="78d86-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78d86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78d86-105">Recupere as propriedades e os relacionamentos de uma coleção de objetos **riskyUser** .</span><span class="sxs-lookup"><span data-stu-id="78d86-105">Retrieve the properties and relationships of a collection of **riskyUser** objects.</span></span>

><span data-ttu-id="78d86-106">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="78d86-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="78d86-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="78d86-107">Permissions</span></span>
<span data-ttu-id="78d86-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78d86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78d86-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78d86-110">Permission type</span></span>      | <span data-ttu-id="78d86-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78d86-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78d86-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78d86-112">Delegated (work or school account)</span></span> | <span data-ttu-id="78d86-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="78d86-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="78d86-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78d86-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78d86-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78d86-115">Not supported.</span></span>    |
|<span data-ttu-id="78d86-116">Application</span><span class="sxs-lookup"><span data-stu-id="78d86-116">Application</span></span> | <span data-ttu-id="78d86-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="78d86-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="78d86-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78d86-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers
GET /identityProtection/riskyUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="78d86-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="78d86-119">Optional query parameters</span></span>
<span data-ttu-id="78d86-120">Este método oferece suporte `$filter` para personalizar a resposta de consulta.</span><span class="sxs-lookup"><span data-stu-id="78d86-120">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="78d86-121">Consulte o exemplo mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="78d86-121">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="78d86-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78d86-122">Request headers</span></span>
| <span data-ttu-id="78d86-123">Nome</span><span class="sxs-lookup"><span data-stu-id="78d86-123">Name</span></span>      |<span data-ttu-id="78d86-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="78d86-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="78d86-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="78d86-125">Authorization</span></span>  | <span data-ttu-id="78d86-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78d86-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="78d86-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="78d86-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="78d86-129">ID da sessão da pasta de trabalho que determina se as alterações são persistentes.</span><span class="sxs-lookup"><span data-stu-id="78d86-129">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="78d86-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="78d86-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="78d86-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78d86-131">Request body</span></span>
<span data-ttu-id="78d86-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78d86-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78d86-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="78d86-133">Response</span></span>
<span data-ttu-id="78d86-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [riskyUser](../resources/riskyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78d86-134">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="78d86-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="78d86-135">Examples</span></span>
### <a name="example-1-list-risky-users"></a><span data-ttu-id="78d86-136">Exemplo 1: listar usuários arriscados</span><span class="sxs-lookup"><span data-stu-id="78d86-136">Example 1: List risky users</span></span>
#### <a name="request"></a><span data-ttu-id="78d86-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78d86-137">Request</span></span>
<span data-ttu-id="78d86-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78d86-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="78d86-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="78d86-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers
```
# <a name="c"></a>[<span data-ttu-id="78d86-140">C#</span><span class="sxs-lookup"><span data-stu-id="78d86-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78d86-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78d86-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78d86-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78d86-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="78d86-143">Java</span><span class="sxs-lookup"><span data-stu-id="78d86-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskyusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="78d86-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="78d86-144">Response</span></span>
<span data-ttu-id="78d86-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78d86-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
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
    ]
}
```

### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="78d86-146">Exemplo 2: listar usuários arriscados e filtrar os resultados</span><span class="sxs-lookup"><span data-stu-id="78d86-146">Example 2: List risky users and filter the results</span></span>
#### <a name="request"></a><span data-ttu-id="78d86-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78d86-147">Request</span></span>
<span data-ttu-id="78d86-148">O exemplo a seguir mostra como usar `$filter` o para obter a coleção de riskyUser cujo nível de risco agregado é médio.</span><span class="sxs-lookup"><span data-stu-id="78d86-148">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>


# <a name="http"></a>[<span data-ttu-id="78d86-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="78d86-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskyusers"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
# <a name="c"></a>[<span data-ttu-id="78d86-150">C#</span><span class="sxs-lookup"><span data-stu-id="78d86-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78d86-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78d86-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78d86-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78d86-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="78d86-153">Java</span><span class="sxs-lookup"><span data-stu-id="78d86-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-filter-riskyusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="78d86-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="78d86-154">Response</span></span>
<span data-ttu-id="78d86-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78d86-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
            "riskLastUpdatedDateTime": "2018-09-22T00:04:49.1195968Z",
            "isProcessing": true,
            "isDeleted": false,
            "riskDetail": "none",
            "riskLevel": "medium",
            "riskState": "atRisk",
            "userDisplayName": "Alex Wilbur",
            "userPrincipalName": "alexw@contoso.com",
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


