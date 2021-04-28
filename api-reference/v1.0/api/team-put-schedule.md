---
title: Criar ou substituir agendamento
description: Crie ou substitua um **objeto schedule.**
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5d40cf859826d66b679e0f0ef7bc2e73c79ffac9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051232"
---
# <a name="create-or-replace-schedule"></a><span data-ttu-id="5ea9e-103">Criar ou substituir agendamento</span><span class="sxs-lookup"><span data-stu-id="5ea9e-103">Create or replace schedule</span></span>

<span data-ttu-id="5ea9e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ea9e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ea9e-105">Crie ou substitua um [objeto schedule.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="5ea9e-105">Create or replace a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="5ea9e-106">O processo de criação de agendamento está em conformidade com a diretriz da API One para operações de longa execução [(RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo)baseadas em recursos.</span><span class="sxs-lookup"><span data-stu-id="5ea9e-106">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="5ea9e-107">Quando os clientes usam o método PUT, se o agendamento for provisionado, a operação substituirá o agendamento; caso contrário, a operação inicia o processo de provisionamento de agendamento em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="5ea9e-107">When clients use the PUT method, if the schedule is provisioned, the operation replaces the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="5ea9e-108">Durante o provisionamento de agendamento, os clientes podem usar o [método GET](schedule-get.md) para obter o agendamento e olhar para a propriedade para o estado atual `provisionStatus` do provisionamento.</span><span class="sxs-lookup"><span data-stu-id="5ea9e-108">During schedule provisioning, clients can use the [GET method](schedule-get.md) to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="5ea9e-109">Se o provisionamento falhar, os clientes poderão obter informações adicionais da `provisionStatusCode` propriedade.</span><span class="sxs-lookup"><span data-stu-id="5ea9e-109">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="5ea9e-110">Os clientes também podem inspecionar a configuração da agenda.</span><span class="sxs-lookup"><span data-stu-id="5ea9e-110">Clients can also inspect the configuration of the schedule.</span></span>


## <a name="permissions"></a><span data-ttu-id="5ea9e-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ea9e-111">Permissions</span></span>

<span data-ttu-id="5ea9e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ea9e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ea9e-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ea9e-114">Permission type</span></span>      | <span data-ttu-id="5ea9e-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ea9e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ea9e-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ea9e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="5ea9e-117">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ea9e-117">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5ea9e-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ea9e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ea9e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ea9e-119">Not supported.</span></span>    |
|<span data-ttu-id="5ea9e-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ea9e-120">Application</span></span> | <span data-ttu-id="5ea9e-121">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ea9e-121">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ea9e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ea9e-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="5ea9e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ea9e-123">Request headers</span></span>

| <span data-ttu-id="5ea9e-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ea9e-124">Header</span></span>       | <span data-ttu-id="5ea9e-125">Valor</span><span class="sxs-lookup"><span data-stu-id="5ea9e-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5ea9e-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ea9e-126">Authorization</span></span>  | <span data-ttu-id="5ea9e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ea9e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5ea9e-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ea9e-129">Content-Type</span></span>  | <span data-ttu-id="5ea9e-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ea9e-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5ea9e-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ea9e-132">Request body</span></span>

<span data-ttu-id="5ea9e-133">No corpo da solicitação, fornece uma representação JSON de um [objeto schedule.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="5ea9e-133">In the request body, supply a JSON representation of a [schedule](../resources/schedule.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5ea9e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ea9e-134">Response</span></span>

<span data-ttu-id="5ea9e-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [schedule](../resources/schedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ea9e-135">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ea9e-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ea9e-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ea9e-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ea9e-137">Request</span></span>

<span data-ttu-id="5ea9e-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ea9e-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "team-put-schedule"
}-->
```http
PUT https://graph.microsoft.com/v1/teams/{teamId}/schedule
Content-type: application/json

{
  "enabled": true,
  "timeZone": "America/Chicago"
}
```
---


### <a name="response"></a><span data-ttu-id="5ea9e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ea9e-139">Response</span></span>

<span data-ttu-id="5ea9e-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ea9e-140">The following is an example of the response.</span></span> 

><span data-ttu-id="5ea9e-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5ea9e-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Creates or replaces the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

