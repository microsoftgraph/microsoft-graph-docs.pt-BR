---
title: Listar riskyUsers
description: Recupere as propriedades e os relacionamentos de uma coleção de objetos **riskyUser** .
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e9c9543321e8fcf0c86d5a8be6948dcafe5eee68
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336352"
---
# <a name="list-riskyusers"></a><span data-ttu-id="58258-103">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="58258-103">List riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58258-104">Recupere as propriedades e os relacionamentos de uma coleção de objetos **riskyUser** .</span><span class="sxs-lookup"><span data-stu-id="58258-104">Retrieve the properties and relationships of a collection of **riskyUser** objects.</span></span>

><span data-ttu-id="58258-105">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="58258-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="58258-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="58258-106">Permissions</span></span>
<span data-ttu-id="58258-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58258-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58258-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58258-109">Permission type</span></span>      | <span data-ttu-id="58258-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58258-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58258-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58258-111">Delegated (work or school account)</span></span> | <span data-ttu-id="58258-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="58258-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="58258-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58258-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58258-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58258-114">Not supported.</span></span>    |
|<span data-ttu-id="58258-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58258-115">Application</span></span> | <span data-ttu-id="58258-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="58258-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58258-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58258-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="58258-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="58258-118">Optional query parameters</span></span>
<span data-ttu-id="58258-119">Este método oferece `$filter` suporte para personalizar a resposta de consulta.</span><span class="sxs-lookup"><span data-stu-id="58258-119">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="58258-120">Consulte o exemplo mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="58258-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="58258-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58258-121">Request headers</span></span>
| <span data-ttu-id="58258-122">Nome</span><span class="sxs-lookup"><span data-stu-id="58258-122">Name</span></span>      |<span data-ttu-id="58258-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="58258-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="58258-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="58258-124">Authorization</span></span>  | <span data-ttu-id="58258-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58258-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="58258-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="58258-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="58258-128">ID da sessão da pasta de trabalho que determina se as alterações são persistentes.</span><span class="sxs-lookup"><span data-stu-id="58258-128">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="58258-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="58258-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="58258-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58258-130">Request body</span></span>
<span data-ttu-id="58258-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="58258-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58258-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="58258-132">Response</span></span>
<span data-ttu-id="58258-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [riskyUser](../resources/riskyUser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58258-133">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyUser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="58258-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="58258-134">Examples</span></span>
### <a name="example-1-list-risky-users"></a><span data-ttu-id="58258-135">Exemplo 1: listar usuários arriscados</span><span class="sxs-lookup"><span data-stu-id="58258-135">Example 1: List risky users</span></span>
#### <a name="request"></a><span data-ttu-id="58258-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58258-136">Request</span></span>
<span data-ttu-id="58258-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58258-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
#### <a name="response"></a><span data-ttu-id="58258-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="58258-138">Response</span></span>
<span data-ttu-id="58258-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58258-139">Here is an example of the response.</span></span>
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

### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="58258-140">Exemplo 2: listar usuários arriscados e filtrar os resultados</span><span class="sxs-lookup"><span data-stu-id="58258-140">Example 2: List risky users and filter the results</span></span>
#### <a name="request"></a><span data-ttu-id="58258-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58258-141">Request</span></span>
<span data-ttu-id="58258-142">O exemplo a seguir mostra como usar `$filter` o para obter a coleção de riskyUser cujo nível de risco agregado é médio.</span><span class="sxs-lookup"><span data-stu-id="58258-142">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_filter_riskyusers"
} -->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```

#### <a name="response"></a><span data-ttu-id="58258-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="58258-143">Response</span></span>
<span data-ttu-id="58258-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58258-144">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->
