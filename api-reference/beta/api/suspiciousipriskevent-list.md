---
title: Listar suspiciousIpRiskEvents
description: Recupere uma lista de objetos suspiciousipriskevent.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 99eb2849a8a25aa20a5223701410093dde314a96
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865038"
---
# <a name="list-suspiciousipriskevents"></a><span data-ttu-id="2b086-103">Listar suspiciousIpRiskEvents</span><span class="sxs-lookup"><span data-stu-id="2b086-103">List suspiciousIpRiskEvents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="2b086-104">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="2b086-104">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="2b086-105">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="2b086-105">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="2b086-106">Recupere uma lista de objetos suspiciousipriskevent.</span><span class="sxs-lookup"><span data-stu-id="2b086-106">Retrieve a list of suspiciousipriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b086-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2b086-107">Permissions</span></span>
<span data-ttu-id="2b086-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b086-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b086-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b086-110">Permission type</span></span>      | <span data-ttu-id="2b086-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b086-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b086-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b086-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2b086-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b086-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="2b086-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b086-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b086-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b086-115">Not supported.</span></span>    |
|<span data-ttu-id="2b086-116">Application</span><span class="sxs-lookup"><span data-stu-id="2b086-116">Application</span></span> | <span data-ttu-id="2b086-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b086-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b086-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b086-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="2b086-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b086-119">Request headers</span></span>
| <span data-ttu-id="2b086-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2b086-120">Name</span></span>      |<span data-ttu-id="2b086-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b086-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2b086-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b086-122">Authorization</span></span>  | <span data-ttu-id="2b086-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b086-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b086-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2b086-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="2b086-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2b086-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b086-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b086-128">Request body</span></span>
<span data-ttu-id="2b086-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2b086-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b086-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b086-130">Response</span></span>

<span data-ttu-id="2b086-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b086-131">If successful, this method returns a `200 OK` response code and collection of [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b086-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b086-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b086-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b086-133">Request</span></span>
<span data-ttu-id="2b086-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b086-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents
```
##### <a name="response"></a><span data-ttu-id="2b086-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b086-135">Response</span></span>
<span data-ttu-id="2b086-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b086-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 290

{
  "value": [
    {
      "closedDateTime": null,
      "createdDateTime": "2016-02-03T06:08:35.123512Z",
      "id": "02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475",
      "ipAddress": "95.31.18.119",
      "location": "Moskva, Russia, RU",
      "riskEventDateTime": "2016-02-03T05:33:49.9516789Z",
      "riskEventStatus": "active",
      "riskLevel": "low",
      "riskType": "SuspiciousIpRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "97b7301f-bc05-8e2c-fdfa-2004eb66ff70",
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
  "description": "List suspiciousIpRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
