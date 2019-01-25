---
title: Obter leakedCredentialsRiskEvent
description: Recupere as propriedades e relacionamentos de um objeto leakedcredentialsriskevent.
localization_priority: Normal
ms.openlocfilehash: eb7b7ca5ecac02a91c2e9733511cd0a384782bd3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509830"
---
# <a name="get-leakedcredentialsriskevent"></a><span data-ttu-id="e641d-103">Obter leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e641d-103">Get leakedCredentialsRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e641d-104">Recupere as propriedades e relacionamentos de um objeto leakedcredentialsriskevent.</span><span class="sxs-lookup"><span data-stu-id="e641d-104">Retrieve the properties and relationships of a leakedcredentialsriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e641d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e641d-105">Permissions</span></span>
<span data-ttu-id="e641d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e641d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e641d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e641d-108">Permission type</span></span>      | <span data-ttu-id="e641d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e641d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e641d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e641d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e641d-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e641d-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="e641d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e641d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e641d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e641d-113">Not supported.</span></span>    |
|<span data-ttu-id="e641d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e641d-114">Application</span></span> | <span data-ttu-id="e641d-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e641d-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e641d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e641d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e641d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e641d-117">Request headers</span></span>
| <span data-ttu-id="e641d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e641d-118">Name</span></span>      |<span data-ttu-id="e641d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e641d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e641d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e641d-120">Authorization</span></span>  | <span data-ttu-id="e641d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e641d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e641d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e641d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e641d-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e641d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e641d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e641d-126">Request body</span></span>
<span data-ttu-id="e641d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e641d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e641d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e641d-128">Response</span></span>

<span data-ttu-id="e641d-129">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e641d-129">If successful, this method returns a `200 OK` response code and [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e641d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e641d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e641d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e641d-131">Request</span></span>
<span data-ttu-id="e641d-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e641d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents/8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182
```
##### <a name="response"></a><span data-ttu-id="e641d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e641d-133">Response</span></span>
<span data-ttu-id="e641d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e641d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "closedDateTime": null,
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "active",
  "riskLevel": "high",
  "riskType": "LeakedCredentialsRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "278dc452-4163-dbc6-84eb-a050c37fc931",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get leakedCredentialsRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/leakedcredentialsriskevent-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
