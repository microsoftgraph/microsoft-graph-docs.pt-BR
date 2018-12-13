---
title: Lista riskyUsers
description: Recupere as propriedades e relacionamentos de um objeto **riskyUsers** .
ms.openlocfilehash: d800f37c1e7e2d03edc0273d30e2be37c799d0d4
ms.sourcegitcommit: ba6b1d1a12dcb54916b4d3e529c856f6514e01e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/12/2018
ms.locfileid: "27241038"
---
# <a name="list-riskyusers"></a><span data-ttu-id="40867-103">Lista riskyUsers</span><span class="sxs-lookup"><span data-stu-id="40867-103">List riskyUsers</span></span>

> <span data-ttu-id="40867-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="40867-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40867-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="40867-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="40867-106">Recupere as propriedades e relacionamentos de um objeto **riskyUsers** .</span><span class="sxs-lookup"><span data-stu-id="40867-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="40867-107">**Observação:** Esta API requer uma licença de P2 Premium do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="40867-107">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="40867-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="40867-108">Permissions</span></span>
<span data-ttu-id="40867-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40867-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40867-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40867-111">Permission type</span></span>      | <span data-ttu-id="40867-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40867-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40867-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40867-113">Delegated (work or school account)</span></span> | <span data-ttu-id="40867-114">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="40867-114">IdentityriskyUser.Read.All</span></span>    |
|<span data-ttu-id="40867-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40867-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40867-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40867-116">Not supported.</span></span>    |
|<span data-ttu-id="40867-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40867-117">Application</span></span> | <span data-ttu-id="40867-118">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="40867-118">IdentityriskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40867-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40867-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="40867-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="40867-120">Optional query parameters</span></span>
<span data-ttu-id="40867-121">Este método oferece suporte `$filter` para personalizar a resposta da consulta.</span><span class="sxs-lookup"><span data-stu-id="40867-121">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="40867-122">Consulte o exemplo mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="40867-122">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="40867-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40867-123">Request headers</span></span>
| <span data-ttu-id="40867-124">Nome</span><span class="sxs-lookup"><span data-stu-id="40867-124">Name</span></span>      |<span data-ttu-id="40867-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="40867-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="40867-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="40867-126">Authorization</span></span>  | <span data-ttu-id="40867-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40867-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="40867-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="40867-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="40867-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="40867-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40867-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40867-132">Request body</span></span>
<span data-ttu-id="40867-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40867-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40867-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="40867-134">Response</span></span>

<span data-ttu-id="40867-135">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [identityRiskEvent](../resources/identityriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40867-135">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40867-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40867-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="40867-137">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="40867-137">Request 1</span></span>
<span data-ttu-id="40867-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40867-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
##### <a name="response-1"></a><span data-ttu-id="40867-139">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="40867-139">Response 1</span></span>
<span data-ttu-id="40867-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40867-140">Here is an example of the response.</span></span>
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
##### <a name="request-2"></a><span data-ttu-id="40867-141">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="40867-141">Request 2</span></span>
<span data-ttu-id="40867-142">O exemplo a seguir mostra como usar `$filter` para obter a coleção de riskyUser cujo risco agregado nível é médio.</span><span class="sxs-lookup"><span data-stu-id="40867-142">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
##### <a name="response-2"></a><span data-ttu-id="40867-143">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="40867-143">Response 2</span></span>
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
