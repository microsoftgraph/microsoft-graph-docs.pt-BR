---
title: Obter riskyUsers
description: Recupere as propriedades e relacionamentos de um objeto **riskyUsers** .
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 586e76cd57e720741c6a63bc00374cd0973a1cf3
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642342"
---
# <a name="get-riskyusers"></a><span data-ttu-id="e34ea-103">Obter riskyUsers</span><span class="sxs-lookup"><span data-stu-id="e34ea-103">Get riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e34ea-104">Recupere as propriedades e relacionamentos de um objeto **riskyUsers** .</span><span class="sxs-lookup"><span data-stu-id="e34ea-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="e34ea-105">**Observação:** Esta API requer uma licença de P2 Premium do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e34ea-105">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="e34ea-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e34ea-106">Permissions</span></span>
<span data-ttu-id="e34ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e34ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e34ea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e34ea-109">Permission type</span></span>      | <span data-ttu-id="e34ea-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e34ea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e34ea-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e34ea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e34ea-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="e34ea-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="e34ea-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e34ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e34ea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e34ea-114">Not supported.</span></span>    |
|<span data-ttu-id="e34ea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e34ea-115">Application</span></span> | <span data-ttu-id="e34ea-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="e34ea-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e34ea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e34ea-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="e34ea-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e34ea-118">Request headers</span></span>
| <span data-ttu-id="e34ea-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e34ea-119">Name</span></span>      |<span data-ttu-id="e34ea-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e34ea-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e34ea-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e34ea-121">Authorization</span></span>  | <span data-ttu-id="e34ea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e34ea-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e34ea-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e34ea-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e34ea-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e34ea-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e34ea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e34ea-127">Request body</span></span>
<span data-ttu-id="e34ea-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e34ea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e34ea-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e34ea-129">Response</span></span>

<span data-ttu-id="e34ea-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [riskyUser](../resources/riskyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e34ea-130">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e34ea-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e34ea-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e34ea-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e34ea-132">Request</span></span>
<span data-ttu-id="e34ea-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e34ea-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="e34ea-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e34ea-134">Response</span></span>
<span data-ttu-id="e34ea-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e34ea-135">Here is an example of the response.</span></span>
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
