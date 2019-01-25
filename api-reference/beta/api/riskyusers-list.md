---
title: Lista riskyUsers
description: Recupere as propriedades e relacionamentos de um objeto **riskyUsers** .
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 5c0c0557a5cd84312ef9d6381d8cf3018ab8ce7d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519315"
---
# <a name="list-riskyusers"></a><span data-ttu-id="d93f8-103">Lista riskyUsers</span><span class="sxs-lookup"><span data-stu-id="d93f8-103">List riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d93f8-104">Recupere as propriedades e relacionamentos de um objeto **riskyUsers** .</span><span class="sxs-lookup"><span data-stu-id="d93f8-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="d93f8-105">**Observação:** Esta API requer uma licença de P2 Premium do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d93f8-105">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="d93f8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d93f8-106">Permissions</span></span>
<span data-ttu-id="d93f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d93f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d93f8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d93f8-109">Permission type</span></span>      | <span data-ttu-id="d93f8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d93f8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d93f8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d93f8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d93f8-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="d93f8-112">IdentityriskyUser.Read.All</span></span>    |
|<span data-ttu-id="d93f8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d93f8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d93f8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d93f8-114">Not supported.</span></span>    |
|<span data-ttu-id="d93f8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d93f8-115">Application</span></span> | <span data-ttu-id="d93f8-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="d93f8-116">IdentityriskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d93f8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d93f8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d93f8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d93f8-118">Optional query parameters</span></span>
<span data-ttu-id="d93f8-119">Este método oferece suporte `$filter` para personalizar a resposta da consulta.</span><span class="sxs-lookup"><span data-stu-id="d93f8-119">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="d93f8-120">Consulte o exemplo mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="d93f8-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="d93f8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d93f8-121">Request headers</span></span>
| <span data-ttu-id="d93f8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d93f8-122">Name</span></span>      |<span data-ttu-id="d93f8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d93f8-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d93f8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d93f8-124">Authorization</span></span>  | <span data-ttu-id="d93f8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d93f8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d93f8-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d93f8-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="d93f8-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d93f8-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d93f8-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d93f8-130">Request body</span></span>
<span data-ttu-id="d93f8-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d93f8-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d93f8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d93f8-132">Response</span></span>

<span data-ttu-id="d93f8-133">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [identityRiskEvent](../resources/identityriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d93f8-133">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d93f8-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d93f8-134">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="d93f8-135">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="d93f8-135">Request 1</span></span>
<span data-ttu-id="d93f8-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d93f8-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
##### <a name="response-1"></a><span data-ttu-id="d93f8-137">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="d93f8-137">Response 1</span></span>
<span data-ttu-id="d93f8-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d93f8-138">Here is an example of the response.</span></span>
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
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
##### <a name="request-2"></a><span data-ttu-id="d93f8-139">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="d93f8-139">Request 2</span></span>
<span data-ttu-id="d93f8-140">O exemplo a seguir mostra como usar `$filter` para obter a coleção de riskyUser cujo risco agregado nível é médio.</span><span class="sxs-lookup"><span data-stu-id="d93f8-140">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
##### <a name="response-2"></a><span data-ttu-id="d93f8-141">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="d93f8-141">Response 2</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
