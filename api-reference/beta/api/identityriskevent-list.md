---
title: Listar identityRiskEvents
description: Recupere uma lista de objetos identityriskevent.
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: a5f6bf6936cda127fdc10970182d05e036a321c7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32501337"
---
# <a name="list-identityriskevents"></a><span data-ttu-id="6e52c-103">Listar identityRiskEvents</span><span class="sxs-lookup"><span data-stu-id="6e52c-103">List identityRiskEvents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e52c-104">Recupere uma lista de objetos identityriskevent.</span><span class="sxs-lookup"><span data-stu-id="6e52c-104">Retrieve a list of identityriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="6e52c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6e52c-105">Permissions</span></span>
<span data-ttu-id="6e52c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e52c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e52c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e52c-108">Permission type</span></span>      | <span data-ttu-id="6e52c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e52c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e52c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e52c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6e52c-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e52c-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="6e52c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e52c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e52c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e52c-113">Not supported.</span></span>    |
|<span data-ttu-id="6e52c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e52c-114">Application</span></span> | <span data-ttu-id="6e52c-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e52c-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e52c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e52c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="6e52c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e52c-117">Request headers</span></span>
| <span data-ttu-id="6e52c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6e52c-118">Name</span></span>      |<span data-ttu-id="6e52c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e52c-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6e52c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e52c-120">Authorization</span></span>  | <span data-ttu-id="6e52c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e52c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6e52c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6e52c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="6e52c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="6e52c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e52c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e52c-126">Request body</span></span>
<span data-ttu-id="6e52c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6e52c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e52c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e52c-128">Response</span></span>

<span data-ttu-id="6e52c-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [identityRiskEvent](../resources/identityriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e52c-129">If successful, this method returns a `200 OK` response code and collection of [identityRiskEvent](../resources/identityriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6e52c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e52c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e52c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e52c-131">Request</span></span>
<span data-ttu-id="6e52c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e52c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityRiskEvents
```
##### <a name="response"></a><span data-ttu-id="6e52c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e52c-133">Response</span></span>
<span data-ttu-id="6e52c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e52c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.malwareRiskEvent",
      "malwareName": "CONFICKER",
      "closedDateTime": null,
      "createdDateTime": "2016-02-03T06:06:01.940814Z",
      "deviceInformation": "B62XYZ13OX",
      "id": "74ceb0af-2271-9167-ffa0-b6ac3b4e8781-9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89-0fdc2304-ba4c-ac0c-bdd7-da2d10e93849",
      "ipAddress": "95.31.18.119",
      "location": "Moskva, Russia, RU",
      "riskEventDateTime": "2016-02-03T05:20:33.7208156Z",
      "riskEventStatus": "active",
      "riskLevel": "low",
      "riskType": "MalwareRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89",
      "userPrincipalName": "jon@contoso.com"
    },
    {
      "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
      "closedDateTime": "2016-01-29T20:03:57.7872426Z",
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89-db69711e-9324-ec99-f010-6e63fb972e98",
      "ipAddress": "176.10.104.240",
      "location": "Bern, CH",
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "remediated",
      "riskLevel": "medium",
      "riskType": "UnfamiliarLocationRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List identityRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityriskevent-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
