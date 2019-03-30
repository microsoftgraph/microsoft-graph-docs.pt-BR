---
title: Listar riskyUsers
description: Recupere as propriedades e os relacionamentos de um objeto **riskyUsers** .
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a902daf00f80470e1ac9a83a287eac507d55e171
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/30/2019
ms.locfileid: "31003724"
---
# <a name="list-riskyusers"></a><span data-ttu-id="c7c62-103">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="c7c62-103">List riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7c62-104">Recupere as propriedades e os relacionamentos de um objeto **riskyUsers** .</span><span class="sxs-lookup"><span data-stu-id="c7c62-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

><span data-ttu-id="c7c62-105">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="c7c62-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7c62-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7c62-106">Permissions</span></span>
<span data-ttu-id="c7c62-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7c62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7c62-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7c62-109">Permission type</span></span>      | <span data-ttu-id="c7c62-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7c62-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7c62-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7c62-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c7c62-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7c62-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="c7c62-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7c62-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7c62-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7c62-114">Not supported.</span></span>    |
|<span data-ttu-id="c7c62-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7c62-115">Application</span></span> | <span data-ttu-id="c7c62-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7c62-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7c62-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7c62-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c7c62-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c7c62-118">Optional query parameters</span></span>
<span data-ttu-id="c7c62-119">Este método oferece `$filter` suporte para personalizar a resposta de consulta.</span><span class="sxs-lookup"><span data-stu-id="c7c62-119">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="c7c62-120">Consulte o exemplo mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="c7c62-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="c7c62-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7c62-121">Request headers</span></span>
| <span data-ttu-id="c7c62-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c7c62-122">Name</span></span>      |<span data-ttu-id="c7c62-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7c62-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c7c62-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7c62-124">Authorization</span></span>  | <span data-ttu-id="c7c62-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7c62-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7c62-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c7c62-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="c7c62-128">ID da sessão da pasta de trabalho que determina se as alterações são persistentes.</span><span class="sxs-lookup"><span data-stu-id="c7c62-128">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="c7c62-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c7c62-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7c62-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7c62-130">Request body</span></span>
<span data-ttu-id="c7c62-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7c62-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7c62-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7c62-132">Response</span></span>

<span data-ttu-id="c7c62-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [identityRiskEvent](../resources/identityriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7c62-133">If successful, this method returns a `200 OK` response code and an [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="c7c62-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c7c62-134">Examples</span></span>
#### <a name="example-1-list-risky-users"></a><span data-ttu-id="c7c62-135">Exemplo 1: listar usuários arriscados</span><span class="sxs-lookup"><span data-stu-id="c7c62-135">Example 1: List risky users</span></span>
<span data-ttu-id="c7c62-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7c62-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```

<span data-ttu-id="c7c62-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7c62-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 200 OK
{
  "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
  "isGuest": "true",
  "isProcessing": true,
  "isDeleted": "true",
  "riskDetail": "adminConfirmedSigninCompromised",
  "riskLevel": "high",
  "riskState": "atRisk"
  "userDisplayName": "Jon Doe",
  "userPrincipalName": "jon@contoso.com"
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
#### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="c7c62-138">Exemplo 2: listar usuários arriscados e filtrar os resultados</span><span class="sxs-lookup"><span data-stu-id="c7c62-138">Example 2: List risky users and filter the results</span></span>
<span data-ttu-id="c7c62-139">O exemplo a seguir mostra como usar `$filter` o para obter a coleção de riskyUser cujo nível de risco agregado é médio.</span><span class="sxs-lookup"><span data-stu-id="c7c62-139">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
<span data-ttu-id="c7c62-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7c62-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 200 OK
{
      "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
      "riskLastUpdatedDateTime": "2018-09-22T00:04:49.1195968Z",
      "isGuest": false,
      "isProcessing": true,
      "isDeleted": false,
      "riskDetail": "none",
      "riskLevel": "medium",
      "riskState": "atRisk",
      "userDisplayName": "Jon Doe",
      "userPrincipalName": "jon@contoso.com",
      }
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
