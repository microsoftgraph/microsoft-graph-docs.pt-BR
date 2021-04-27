---
title: Listar impossibleTravelRiskEvents
description: Recupere uma lista de objetos impossibletravelriskevent.
localization_priority: Normal
doc_type: apiPageType
author: cloudhandler
ms.prod: identity-and-sign-in
ms.openlocfilehash: 6e3fe266556830bb6ebea3fccba0323f6bd7866b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040627"
---
# <a name="list-impossibletravelriskevents-deprecated"></a><span data-ttu-id="b8288-103">Listar impossibleTravelRiskEvents (preterido)</span><span class="sxs-lookup"><span data-stu-id="b8288-103">List impossibleTravelRiskEvents (deprecated)</span></span>

<span data-ttu-id="b8288-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8288-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="b8288-105">A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="b8288-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="b8288-106">Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="b8288-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="b8288-107">Recupere uma lista de objetos impossibletravelriskevent.</span><span class="sxs-lookup"><span data-stu-id="b8288-107">Retrieve a list of impossibletravelriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b8288-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8288-108">Permissions</span></span>
<span data-ttu-id="b8288-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8288-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8288-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8288-111">Permission type</span></span>      | <span data-ttu-id="b8288-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8288-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8288-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8288-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b8288-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8288-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="b8288-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8288-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8288-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8288-116">Not supported.</span></span>    |
|<span data-ttu-id="b8288-117">Application</span><span class="sxs-lookup"><span data-stu-id="b8288-117">Application</span></span> | <span data-ttu-id="b8288-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8288-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8288-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8288-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /impossibleTravelRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="b8288-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8288-120">Request headers</span></span>
| <span data-ttu-id="b8288-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b8288-121">Name</span></span>      |<span data-ttu-id="b8288-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8288-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b8288-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8288-123">Authorization</span></span>  | <span data-ttu-id="b8288-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8288-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b8288-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b8288-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="b8288-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b8288-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8288-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8288-129">Request body</span></span>
<span data-ttu-id="b8288-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8288-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8288-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8288-131">Response</span></span>

<span data-ttu-id="b8288-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8288-132">If successful, this method returns a `200 OK` response code and collection of [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b8288-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8288-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8288-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8288-134">Request</span></span>
<span data-ttu-id="b8288-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8288-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_impossibletravelriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/impossibleTravelRiskEvents
```
##### <a name="response"></a><span data-ttu-id="b8288-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8288-136">Response</span></span>
<span data-ttu-id="b8288-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8288-137">Here is an example of the response.</span></span> <span data-ttu-id="b8288-138">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b8288-138">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 313

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.impossibleTravelRiskEvent",
      "closedDateTime": "2016-01-29T20:03:57.7872426Z",
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "22e65c1f-909a-42b5-c0d2-075f30e27887-0bfdc7a8-6a16-c33e-7de9-a60a28ae533b-15475553-dbc1-8879-5079-23b1edd25bab",
      "ipAddress": "176.10.104.240",
      "isAtypicalLocation": true,
      "location": "Bern, CH",
      "previousIPAddress": "95.31.18.119",
      "previousLocation": "Moskva, Russia, RU",
      "previousSigninDateTime": "2016-01-29T00:00:55.3859274Z",
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "remediated",
      "riskLevel": "medium",
      "riskType": "ImpossibleTravelRiskEvent",
      "userAgent": "Mozilla",
      "userDisplayName": "Jon Doe",
      "userId": "0bfdc7a8-6a16-c33e-7de9-a60a28ae533b",
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
  "description": "List impossibleTravelRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


