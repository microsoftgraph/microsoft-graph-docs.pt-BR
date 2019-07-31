---
title: Listar suspiciousIpRiskEvents
description: Recupere uma lista de objetos suspiciousipriskevent.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 1758b62dc46223c902e210e06183ab4f3d61f00c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977759"
---
# <a name="list-suspiciousipriskevents"></a><span data-ttu-id="335a8-103">Listar suspiciousIpRiskEvents</span><span class="sxs-lookup"><span data-stu-id="335a8-103">List suspiciousIpRiskEvents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="335a8-104">Recupere uma lista de objetos suspiciousipriskevent.</span><span class="sxs-lookup"><span data-stu-id="335a8-104">Retrieve a list of suspiciousipriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="335a8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="335a8-105">Permissions</span></span>
<span data-ttu-id="335a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="335a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="335a8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="335a8-108">Permission type</span></span>      | <span data-ttu-id="335a8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="335a8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="335a8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="335a8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="335a8-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="335a8-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="335a8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="335a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="335a8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="335a8-113">Not supported.</span></span>    |
|<span data-ttu-id="335a8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="335a8-114">Application</span></span> | <span data-ttu-id="335a8-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="335a8-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="335a8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="335a8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="335a8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="335a8-117">Request headers</span></span>
| <span data-ttu-id="335a8-118">Nome</span><span class="sxs-lookup"><span data-stu-id="335a8-118">Name</span></span>      |<span data-ttu-id="335a8-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="335a8-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="335a8-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="335a8-120">Authorization</span></span>  | <span data-ttu-id="335a8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="335a8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="335a8-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="335a8-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="335a8-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="335a8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="335a8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="335a8-126">Request body</span></span>
<span data-ttu-id="335a8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="335a8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="335a8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="335a8-128">Response</span></span>

<span data-ttu-id="335a8-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="335a8-129">If successful, this method returns a `200 OK` response code and collection of [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="335a8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="335a8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="335a8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="335a8-131">Request</span></span>
<span data-ttu-id="335a8-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="335a8-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents
```
##### <a name="response"></a><span data-ttu-id="335a8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="335a8-133">Response</span></span>
<span data-ttu-id="335a8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="335a8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
