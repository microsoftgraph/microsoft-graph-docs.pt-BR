---
title: Listar riskyUsers
description: Recupere as propriedades e os relacionamentos de uma coleção de objetos **riskyUser** .
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dc67514b0047ed89faee62dcb864106829065160
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48047081"
---
# <a name="list-riskyusers"></a><span data-ttu-id="45c56-103">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="45c56-103">List riskyUsers</span></span>

<span data-ttu-id="45c56-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45c56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45c56-105">Recupere as propriedades e os relacionamentos de uma coleção de objetos **riskyUser** .</span><span class="sxs-lookup"><span data-stu-id="45c56-105">Retrieve the properties and relationships of a collection of **riskyUser** objects.</span></span>

><span data-ttu-id="45c56-106">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="45c56-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="45c56-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="45c56-107">Permissions</span></span>
<span data-ttu-id="45c56-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45c56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45c56-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45c56-110">Permission type</span></span>      | <span data-ttu-id="45c56-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45c56-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45c56-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45c56-112">Delegated (work or school account)</span></span> | <span data-ttu-id="45c56-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="45c56-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="45c56-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45c56-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45c56-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45c56-115">Not supported.</span></span>    |
|<span data-ttu-id="45c56-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45c56-116">Application</span></span> | <span data-ttu-id="45c56-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="45c56-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45c56-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45c56-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers
GET /identityProtection/riskyUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="45c56-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="45c56-119">Optional query parameters</span></span>
<span data-ttu-id="45c56-120">Este método oferece suporte `$filter` para personalizar a resposta de consulta.</span><span class="sxs-lookup"><span data-stu-id="45c56-120">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="45c56-121">Consulte o exemplo mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="45c56-121">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="45c56-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45c56-122">Request headers</span></span>
| <span data-ttu-id="45c56-123">Nome</span><span class="sxs-lookup"><span data-stu-id="45c56-123">Name</span></span>      |<span data-ttu-id="45c56-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="45c56-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="45c56-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="45c56-125">Authorization</span></span>  | <span data-ttu-id="45c56-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45c56-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="45c56-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="45c56-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="45c56-129">ID da sessão da pasta de trabalho que determina se as alterações são persistentes.</span><span class="sxs-lookup"><span data-stu-id="45c56-129">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="45c56-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="45c56-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45c56-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45c56-131">Request body</span></span>
<span data-ttu-id="45c56-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45c56-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45c56-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="45c56-133">Response</span></span>
<span data-ttu-id="45c56-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [riskyUser](../resources/riskyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45c56-134">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45c56-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="45c56-135">Examples</span></span>
### <a name="example-1-list-risky-users"></a><span data-ttu-id="45c56-136">Exemplo 1: listar usuários arriscados</span><span class="sxs-lookup"><span data-stu-id="45c56-136">Example 1: List risky users</span></span>
#### <a name="request"></a><span data-ttu-id="45c56-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45c56-137">Request</span></span>
<span data-ttu-id="45c56-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45c56-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="45c56-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="45c56-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers
```
# <a name="c"></a>[<span data-ttu-id="45c56-140">C#</span><span class="sxs-lookup"><span data-stu-id="45c56-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45c56-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45c56-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45c56-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45c56-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="45c56-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="45c56-143">Response</span></span>
<span data-ttu-id="45c56-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45c56-144">Here is an example of the response.</span></span>
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

### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="45c56-145">Exemplo 2: listar usuários arriscados e filtrar os resultados</span><span class="sxs-lookup"><span data-stu-id="45c56-145">Example 2: List risky users and filter the results</span></span>
#### <a name="request"></a><span data-ttu-id="45c56-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45c56-146">Request</span></span>
<span data-ttu-id="45c56-147">O exemplo a seguir mostra como usar `$filter` o para obter a coleção de riskyUser cujo nível de risco agregado é médio.</span><span class="sxs-lookup"><span data-stu-id="45c56-147">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>


# <a name="http"></a>[<span data-ttu-id="45c56-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="45c56-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskyusers"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
# <a name="c"></a>[<span data-ttu-id="45c56-149">C#</span><span class="sxs-lookup"><span data-stu-id="45c56-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45c56-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45c56-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45c56-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45c56-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="45c56-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="45c56-152">Response</span></span>
<span data-ttu-id="45c56-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45c56-153">Here is an example of the response.</span></span>
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


