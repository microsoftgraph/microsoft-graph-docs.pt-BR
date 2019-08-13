---
title: Listar riskyUsers
description: Recupere as propriedades e os relacionamentos de uma coleção de objetos **riskyUser** .
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cb29c5845c8243a046a563351d4b1e486d38c029
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358199"
---
# <a name="list-riskyusers"></a><span data-ttu-id="0ec09-103">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="0ec09-103">List riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ec09-104">Recupere as propriedades e os relacionamentos de uma coleção de objetos **riskyUser** .</span><span class="sxs-lookup"><span data-stu-id="0ec09-104">Retrieve the properties and relationships of a collection of **riskyUser** objects.</span></span>

><span data-ttu-id="0ec09-105">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="0ec09-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ec09-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ec09-106">Permissions</span></span>
<span data-ttu-id="0ec09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ec09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ec09-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ec09-109">Permission type</span></span>      | <span data-ttu-id="0ec09-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ec09-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ec09-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ec09-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0ec09-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ec09-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="0ec09-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ec09-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ec09-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ec09-114">Not supported.</span></span>    |
|<span data-ttu-id="0ec09-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ec09-115">Application</span></span> | <span data-ttu-id="0ec09-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ec09-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ec09-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ec09-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0ec09-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0ec09-118">Optional query parameters</span></span>
<span data-ttu-id="0ec09-119">Este método oferece `$filter` suporte para personalizar a resposta de consulta.</span><span class="sxs-lookup"><span data-stu-id="0ec09-119">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="0ec09-120">Consulte o exemplo mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="0ec09-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="0ec09-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ec09-121">Request headers</span></span>
| <span data-ttu-id="0ec09-122">Nome</span><span class="sxs-lookup"><span data-stu-id="0ec09-122">Name</span></span>      |<span data-ttu-id="0ec09-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ec09-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0ec09-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ec09-124">Authorization</span></span>  | <span data-ttu-id="0ec09-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ec09-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ec09-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0ec09-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="0ec09-128">ID da sessão da pasta de trabalho que determina se as alterações são persistentes.</span><span class="sxs-lookup"><span data-stu-id="0ec09-128">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="0ec09-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0ec09-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ec09-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ec09-130">Request body</span></span>
<span data-ttu-id="0ec09-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0ec09-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ec09-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ec09-132">Response</span></span>
<span data-ttu-id="0ec09-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [riskyUser](../resources/riskyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ec09-133">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ec09-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0ec09-134">Examples</span></span>
### <a name="example-1-list-risky-users"></a><span data-ttu-id="0ec09-135">Exemplo 1: listar usuários arriscados</span><span class="sxs-lookup"><span data-stu-id="0ec09-135">Example 1: List risky users</span></span>
#### <a name="request"></a><span data-ttu-id="0ec09-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ec09-136">Request</span></span>
<span data-ttu-id="0ec09-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ec09-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0ec09-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ec09-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0ec09-139">C#</span><span class="sxs-lookup"><span data-stu-id="0ec09-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ec09-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ec09-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0ec09-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0ec09-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0ec09-142">Java</span><span class="sxs-lookup"><span data-stu-id="0ec09-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskyusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="0ec09-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ec09-143">Response</span></span>
<span data-ttu-id="0ec09-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ec09-144">Here is an example of the response.</span></span>
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
            "isGuest": true,
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

### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="0ec09-145">Exemplo 2: listar usuários arriscados e filtrar os resultados</span><span class="sxs-lookup"><span data-stu-id="0ec09-145">Example 2: List risky users and filter the results</span></span>
#### <a name="request"></a><span data-ttu-id="0ec09-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ec09-146">Request</span></span>
<span data-ttu-id="0ec09-147">O exemplo a seguir mostra como usar `$filter` o para obter a coleção de riskyUser cujo nível de risco agregado é médio.</span><span class="sxs-lookup"><span data-stu-id="0ec09-147">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0ec09-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ec09-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskyusers"
} -->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0ec09-149">C#</span><span class="sxs-lookup"><span data-stu-id="0ec09-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ec09-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ec09-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0ec09-151">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0ec09-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0ec09-152">Java</span><span class="sxs-lookup"><span data-stu-id="0ec09-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-filter-riskyusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0ec09-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ec09-153">Response</span></span>
<span data-ttu-id="0ec09-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ec09-154">Here is an example of the response.</span></span>
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
            "isGuest": false,
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
