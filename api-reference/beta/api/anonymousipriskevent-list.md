---
title: Listar anonymousIpRiskEvents
description: Recupere uma lista de objetos anonymousipriskevent.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7faa48557cb9a275df710dec699c964df9a8b9a7
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868468"
---
# <a name="list-anonymousipriskevents"></a><span data-ttu-id="136f6-103">Listar anonymousIpRiskEvents</span><span class="sxs-lookup"><span data-stu-id="136f6-103">List anonymousIpRiskEvents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="136f6-104">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="136f6-104">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="136f6-105">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="136f6-105">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="136f6-106">Recupere uma lista de objetos anonymousipriskevent.</span><span class="sxs-lookup"><span data-stu-id="136f6-106">Retrieve a list of anonymousipriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="136f6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="136f6-107">Permissions</span></span>
<span data-ttu-id="136f6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="136f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="136f6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="136f6-110">Permission type</span></span>      | <span data-ttu-id="136f6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="136f6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="136f6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="136f6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="136f6-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="136f6-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="136f6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="136f6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="136f6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="136f6-115">Not supported.</span></span>    |
|<span data-ttu-id="136f6-116">Application</span><span class="sxs-lookup"><span data-stu-id="136f6-116">Application</span></span> | <span data-ttu-id="136f6-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="136f6-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="136f6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="136f6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents
```

## <a name="request-headers"></a><span data-ttu-id="136f6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="136f6-119">Request headers</span></span>
| <span data-ttu-id="136f6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="136f6-120">Name</span></span>      |<span data-ttu-id="136f6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="136f6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="136f6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="136f6-122">Authorization</span></span>  | <span data-ttu-id="136f6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="136f6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="136f6-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="136f6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="136f6-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="136f6-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="136f6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="136f6-128">Request body</span></span>
<span data-ttu-id="136f6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="136f6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="136f6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="136f6-130">Response</span></span>

<span data-ttu-id="136f6-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="136f6-131">If successful, this method returns a `200 OK` response code and collection of [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="136f6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="136f6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="136f6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="136f6-133">Request</span></span>
<span data-ttu-id="136f6-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="136f6-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents
```
##### <a name="response"></a><span data-ttu-id="136f6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="136f6-135">Response</span></span>
<span data-ttu-id="136f6-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="136f6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 290

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List anonymousIpRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
