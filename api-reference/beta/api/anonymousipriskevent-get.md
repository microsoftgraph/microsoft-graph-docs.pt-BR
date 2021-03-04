---
title: Obter anonymousIpRiskEvent
description: Recupere as propriedades e as relações de um objeto anonymousipriskevent.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: 41c861a77b5c87ad9289a8e0db3ca697a08fc9e4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438635"
---
# <a name="get-anonymousipriskevent-deprecated"></a><span data-ttu-id="dffaa-103">Obter anonymousIpRiskEvent (preterido)</span><span class="sxs-lookup"><span data-stu-id="dffaa-103">Get anonymousIpRiskEvent (deprecated)</span></span>

<span data-ttu-id="dffaa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dffaa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="dffaa-105">A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="dffaa-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="dffaa-106">Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="dffaa-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="dffaa-107">Recupere as propriedades e as relações de um objeto anonymousipriskevent.</span><span class="sxs-lookup"><span data-stu-id="dffaa-107">Retrieve the properties and relationships of an anonymousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dffaa-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="dffaa-108">Permissions</span></span>
<span data-ttu-id="dffaa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dffaa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dffaa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dffaa-111">Permission type</span></span>      | <span data-ttu-id="dffaa-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dffaa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dffaa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dffaa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dffaa-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="dffaa-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="dffaa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dffaa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dffaa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dffaa-116">Not supported.</span></span>    |
|<span data-ttu-id="dffaa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dffaa-117">Application</span></span> | <span data-ttu-id="dffaa-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="dffaa-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dffaa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dffaa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dffaa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dffaa-120">Request headers</span></span>
| <span data-ttu-id="dffaa-121">Nome</span><span class="sxs-lookup"><span data-stu-id="dffaa-121">Name</span></span>      |<span data-ttu-id="dffaa-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="dffaa-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dffaa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dffaa-123">Authorization</span></span>  | <span data-ttu-id="dffaa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dffaa-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dffaa-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dffaa-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="dffaa-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="dffaa-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dffaa-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dffaa-129">Request body</span></span>
<span data-ttu-id="dffaa-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dffaa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dffaa-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dffaa-131">Response</span></span>

<span data-ttu-id="dffaa-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto anonymousIpRiskEvent](../resources/anonymousipriskevent.md) no valor do corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dffaa-132">If successful, this method returns a `200 OK` response code and [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object in the value of response body.</span></span>
## <a name="example"></a><span data-ttu-id="dffaa-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dffaa-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dffaa-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dffaa-134">Request</span></span>
<span data-ttu-id="dffaa-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dffaa-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents/2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71
```
##### <a name="response"></a><span data-ttu-id="dffaa-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="dffaa-136">Response</span></span>
<span data-ttu-id="dffaa-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dffaa-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71",
  "ipAddress": null,
  "location": null,
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "AnonymousIpRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "6a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get anonymousIpRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


