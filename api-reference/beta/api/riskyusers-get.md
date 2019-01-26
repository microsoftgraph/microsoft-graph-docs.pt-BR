---
title: Obter riskyUsers
description: Recupere as propriedades e relacionamentos de um objeto **riskyUsers** .
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 18798df27ebccb3e56afa4e0f479ced4b4029863
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575297"
---
# <a name="get-riskyusers"></a><span data-ttu-id="f59f4-103">Obter riskyUsers</span><span class="sxs-lookup"><span data-stu-id="f59f4-103">Get riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f59f4-104">Recupere as propriedades e relacionamentos de um objeto **riskyUsers** .</span><span class="sxs-lookup"><span data-stu-id="f59f4-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="f59f4-105">**Observação:** Esta API requer uma licença de P2 Premium do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f59f4-105">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="f59f4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f59f4-106">Permissions</span></span>
<span data-ttu-id="f59f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f59f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f59f4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f59f4-109">Permission type</span></span>      | <span data-ttu-id="f59f4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f59f4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f59f4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f59f4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f59f4-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="f59f4-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="f59f4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f59f4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f59f4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f59f4-114">Not supported.</span></span>    |
|<span data-ttu-id="f59f4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f59f4-115">Application</span></span> | <span data-ttu-id="f59f4-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="f59f4-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f59f4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f59f4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="f59f4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f59f4-118">Request headers</span></span>
| <span data-ttu-id="f59f4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f59f4-119">Name</span></span>      |<span data-ttu-id="f59f4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f59f4-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f59f4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f59f4-121">Authorization</span></span>  | <span data-ttu-id="f59f4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f59f4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f59f4-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f59f4-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="f59f4-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f59f4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f59f4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f59f4-127">Request body</span></span>
<span data-ttu-id="f59f4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f59f4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f59f4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f59f4-129">Response</span></span>

<span data-ttu-id="f59f4-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [riskyUser](../resources/riskyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f59f4-130">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f59f4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f59f4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f59f4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f59f4-132">Request</span></span>
<span data-ttu-id="f59f4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f59f4-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
##### <a name="response"></a><span data-ttu-id="f59f4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f59f4-134">Response</span></span>
<span data-ttu-id="f59f4-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f59f4-135">Here is an example of the response.</span></span>
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
  "isDeleted": true,
  "riskDetail": "adminConfirmedSigninCompromised",
  "riskLevel": "high",
  "riskState": "atRisk",
  "userDisplayName": "Jon Doe",
  "userPrincipalName": "jon@contoso.com"
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
    "Error: /api-reference/beta/api/riskyusers-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
