---
title: Obter cronograma
description: Recupere as propriedades e os relacionamentos de um objeto **Schedule** .
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fe5f2d72d43398893b366e4aa2632700df6649c6
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155170"
---
# <a name="get-schedule"></a><span data-ttu-id="9be41-103">Obter cronograma</span><span class="sxs-lookup"><span data-stu-id="9be41-103">Get schedule</span></span>

<span data-ttu-id="9be41-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9be41-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9be41-105">Recupere as propriedades e os relacionamentos de um objeto [Schedule](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="9be41-105">Retrieve the properties and relationships of a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="9be41-106">O processo de criação de agendamento está em conformidade com a [diretriz de uma API para operações de longa duração com base em recursos (relo)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span><span class="sxs-lookup"><span data-stu-id="9be41-106">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="9be41-107">Quando os clientes usam o [método Put](team-put-schedule.md), se a agenda for provisionada, a operação atualizará a agenda; caso contrário, a operação iniciará o processo de provisionamento de agendamento em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="9be41-107">When clients use the [PUT method](team-put-schedule.md), if the schedule is provisioned, the operation updates the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="9be41-108">Durante o provisionamento de agendamento, os clientes podem usar o método GET para obter o agendamento e observar a `provisionStatus` propriedade para o estado atual do provisionamento.</span><span class="sxs-lookup"><span data-stu-id="9be41-108">During schedule provisioning, clients can use the GET method to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="9be41-109">Se o provisionamento falhar, os clientes poderão obter informações adicionais da `provisionStatusCode` propriedade.</span><span class="sxs-lookup"><span data-stu-id="9be41-109">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="9be41-110">Os clientes também podem inspecionar a configuração do cronograma.</span><span class="sxs-lookup"><span data-stu-id="9be41-110">Clients can also inspect the configuration of the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="9be41-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="9be41-111">Permissions</span></span>

<span data-ttu-id="9be41-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9be41-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9be41-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9be41-114">Permission type</span></span>      | <span data-ttu-id="9be41-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9be41-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9be41-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9be41-116">Delegated (work or school account)</span></span> | <span data-ttu-id="9be41-117">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9be41-117">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9be41-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9be41-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9be41-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9be41-119">Not supported.</span></span>    |<span data-ttu-id="9be41-120">s</span><span class="sxs-lookup"><span data-stu-id="9be41-120">s</span></span>
|<span data-ttu-id="9be41-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9be41-121">Application</span></span> | <span data-ttu-id="9be41-122">Schedule. Read. All, Schedule. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9be41-122">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="9be41-123">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="9be41-123">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9be41-124">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="9be41-124">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9be41-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9be41-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9be41-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9be41-126">Optional query parameters</span></span>

<span data-ttu-id="9be41-127">Este método não oferece suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9be41-127">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9be41-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9be41-128">Request headers</span></span>

| <span data-ttu-id="9be41-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9be41-129">Header</span></span>       | <span data-ttu-id="9be41-130">Valor</span><span class="sxs-lookup"><span data-stu-id="9be41-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9be41-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="9be41-131">Authorization</span></span>  | <span data-ttu-id="9be41-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9be41-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9be41-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9be41-134">Content-Type</span></span>  | <span data-ttu-id="9be41-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9be41-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9be41-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9be41-137">Request body</span></span>
<span data-ttu-id="9be41-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9be41-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9be41-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9be41-139">Response</span></span>

<span data-ttu-id="9be41-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Schedule](../resources/schedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9be41-140">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9be41-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9be41-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="9be41-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9be41-142">Request</span></span>

<span data-ttu-id="9be41-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9be41-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule
```
---


### <a name="response"></a><span data-ttu-id="9be41-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="9be41-144">Response</span></span>

<span data-ttu-id="9be41-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9be41-145">The following is an example of the response.</span></span> 

><span data-ttu-id="9be41-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9be41-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedule"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null,
  "timeClockEnabled": true,
  "openShiftsEnabled": true,
  "swapShiftsRequestsEnabled": true,
  "offerShiftRequestsEnabled": true,
  "timeOffRequestsEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
