---
title: Obter anonymousIpRiskEvent
description: Recupere as propriedades e os relacionamentos de um objeto anonymousipriskevent.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: cloudhandler
ms.openlocfilehash: 2fb493c35d6d26f3b1a7b4212cbe242da0062ba3
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43178941"
---
# <a name="get-anonymousipriskevent"></a><span data-ttu-id="fcdad-103">Obter anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="fcdad-103">Get anonymousIpRiskEvent</span></span>

<span data-ttu-id="fcdad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcdad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="fcdad-105">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="fcdad-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="fcdad-106">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="fcdad-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="fcdad-107">Recupere as propriedades e os relacionamentos de um objeto anonymousipriskevent.</span><span class="sxs-lookup"><span data-stu-id="fcdad-107">Retrieve the properties and relationships of an anonymousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fcdad-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="fcdad-108">Permissions</span></span>
<span data-ttu-id="fcdad-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcdad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcdad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fcdad-111">Permission type</span></span>      | <span data-ttu-id="fcdad-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fcdad-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcdad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fcdad-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fcdad-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcdad-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="fcdad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fcdad-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcdad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcdad-116">Not supported.</span></span>    |
|<span data-ttu-id="fcdad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fcdad-117">Application</span></span> | <span data-ttu-id="fcdad-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcdad-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fcdad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fcdad-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fcdad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fcdad-120">Request headers</span></span>
| <span data-ttu-id="fcdad-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fcdad-121">Name</span></span>      |<span data-ttu-id="fcdad-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcdad-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fcdad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fcdad-123">Authorization</span></span>  | <span data-ttu-id="fcdad-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fcdad-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fcdad-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fcdad-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="fcdad-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="fcdad-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcdad-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fcdad-129">Request body</span></span>
<span data-ttu-id="fcdad-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fcdad-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcdad-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcdad-131">Response</span></span>

<span data-ttu-id="fcdad-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) no valor do corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fcdad-132">If successful, this method returns a `200 OK` response code and [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object in the value of response body.</span></span>
## <a name="example"></a><span data-ttu-id="fcdad-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fcdad-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fcdad-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcdad-134">Request</span></span>
<span data-ttu-id="fcdad-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcdad-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents/2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71
```
##### <a name="response"></a><span data-ttu-id="fcdad-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcdad-136">Response</span></span>
<span data-ttu-id="fcdad-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fcdad-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
