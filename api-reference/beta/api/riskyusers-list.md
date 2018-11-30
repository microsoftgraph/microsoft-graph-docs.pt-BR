---
title: Lista riskyUsers
description: Recupere as propriedades e relacionamentos de um objeto **riskyUsers** .
ms.openlocfilehash: 152171ff098bb58e8cbb247ca687841e77594ead
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041128"
---
# <a name="list-riskyusers"></a><span data-ttu-id="793fc-103">Lista riskyUsers</span><span class="sxs-lookup"><span data-stu-id="793fc-103">List riskyUsers</span></span>

> <span data-ttu-id="793fc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="793fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="793fc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="793fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="793fc-106">Recupere as propriedades e relacionamentos de um objeto **riskyUsers** .</span><span class="sxs-lookup"><span data-stu-id="793fc-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="793fc-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="793fc-107">Permissions</span></span>
<span data-ttu-id="793fc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="793fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="793fc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="793fc-110">Permission type</span></span>      | <span data-ttu-id="793fc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="793fc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="793fc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="793fc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="793fc-113">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="793fc-113">IdentityriskyUser.Read.All</span></span>    |
|<span data-ttu-id="793fc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="793fc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="793fc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="793fc-115">Not supported.</span></span>    |
|<span data-ttu-id="793fc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="793fc-116">Application</span></span> | <span data-ttu-id="793fc-117">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="793fc-117">IdentityriskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="793fc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="793fc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="793fc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="793fc-119">Optional query parameters</span></span>
<span data-ttu-id="793fc-120">Este método oferece suporte `$filter` para personalizar a resposta da consulta.</span><span class="sxs-lookup"><span data-stu-id="793fc-120">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="793fc-121">Consulte o exemplo mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="793fc-121">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="793fc-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="793fc-122">Request headers</span></span>
| <span data-ttu-id="793fc-123">Nome</span><span class="sxs-lookup"><span data-stu-id="793fc-123">Name</span></span>      |<span data-ttu-id="793fc-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="793fc-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="793fc-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="793fc-125">Authorization</span></span>  | <span data-ttu-id="793fc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="793fc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="793fc-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="793fc-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="793fc-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="793fc-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="793fc-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="793fc-131">Request body</span></span>
<span data-ttu-id="793fc-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="793fc-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="793fc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="793fc-133">Response</span></span>

<span data-ttu-id="793fc-134">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [identityRiskEvent](../resources/identityriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="793fc-134">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="793fc-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="793fc-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="793fc-136">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="793fc-136">Request 1</span></span>
<span data-ttu-id="793fc-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="793fc-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
##### <a name="response-1"></a><span data-ttu-id="793fc-138">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="793fc-138">Response 1</span></span>
<span data-ttu-id="793fc-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="793fc-139">Here is an example of the response.</span></span>
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
##### <a name="request-2"></a><span data-ttu-id="793fc-140">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="793fc-140">Request 2</span></span>
<span data-ttu-id="793fc-141">O exemplo a seguir mostra como usar `$filter` para obter a coleção de riskyUser cujo risco agregado nível é médio.</span><span class="sxs-lookup"><span data-stu-id="793fc-141">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
##### <a name="response-2"></a><span data-ttu-id="793fc-142">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="793fc-142">Response 2</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
