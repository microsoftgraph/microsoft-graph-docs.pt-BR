---
title: Listar unfamiliarLocationRiskEvents
description: Recupere uma lista de objetos unfamiliarlocationriskevent.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: b12bc0520bfa285b654b615cfb74582683b04c49
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987898"
---
# <a name="list-unfamiliarlocationriskevents"></a><span data-ttu-id="1aa33-103">Listar unfamiliarLocationRiskEvents</span><span class="sxs-lookup"><span data-stu-id="1aa33-103">List unfamiliarLocationRiskEvents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1aa33-104">Recupere uma lista de objetos unfamiliarlocationriskevent.</span><span class="sxs-lookup"><span data-stu-id="1aa33-104">Retrieve a list of unfamiliarlocationriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="1aa33-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1aa33-105">Permissions</span></span>
<span data-ttu-id="1aa33-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1aa33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1aa33-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1aa33-108">Permission type</span></span>      | <span data-ttu-id="1aa33-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1aa33-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1aa33-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1aa33-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1aa33-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="1aa33-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="1aa33-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1aa33-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1aa33-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1aa33-113">Not supported.</span></span>    |
|<span data-ttu-id="1aa33-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1aa33-114">Application</span></span> | <span data-ttu-id="1aa33-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="1aa33-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1aa33-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1aa33-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /unfamiliarLocationRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="1aa33-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1aa33-117">Request headers</span></span>
| <span data-ttu-id="1aa33-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1aa33-118">Name</span></span>      |<span data-ttu-id="1aa33-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1aa33-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1aa33-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="1aa33-120">Authorization</span></span>  | <span data-ttu-id="1aa33-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1aa33-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1aa33-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1aa33-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="1aa33-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1aa33-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1aa33-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1aa33-126">Request body</span></span>
<span data-ttu-id="1aa33-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1aa33-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1aa33-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1aa33-128">Response</span></span>

<span data-ttu-id="1aa33-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1aa33-129">If successful, this method returns a `200 OK` response code and collection of [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1aa33-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1aa33-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1aa33-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1aa33-131">Request</span></span>
<span data-ttu-id="1aa33-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1aa33-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unfamiliarlocationriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/unfamiliarLocationRiskEvents
```
##### <a name="response"></a><span data-ttu-id="1aa33-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1aa33-133">Response</span></span>
<span data-ttu-id="1aa33-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1aa33-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent",
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
      "id": "700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604",
      "ipAddress": "176.10.104.240",
      "location": "Bern, CH",
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "remediated",
      "riskLevel": "medium",
      "riskType": "UnfamiliarLocationRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad",
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
  "description": "List unfamiliarLocationRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
