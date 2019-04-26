---
title: Criar ou substituir agendamento
description: Criar ou substituir um objeto **Schedule** .
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 84d34de6a0410e1372950688c610e6ed7c2e3554
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330520"
---
# <a name="create-or-replace-schedule"></a><span data-ttu-id="26f1f-103">Criar ou substituir agendamento</span><span class="sxs-lookup"><span data-stu-id="26f1f-103">Create or replace schedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26f1f-104">Criar ou substituir um objeto [Schedule](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="26f1f-104">Create or replace a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="26f1f-105">O processo de criação de agendamento está em conformidade com a [diretriz de uma API para operações de longa duração com base em recursos (relo)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span><span class="sxs-lookup"><span data-stu-id="26f1f-105">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="26f1f-106">Quando os clientes usam o método PUT, se a agenda for provisionada, a operação substituirá a agenda; caso contrário, a operação iniciará o processo de provisionamento de agendamento em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="26f1f-106">When clients use the PUT method, if the schedule is provisioned, the operation replaces the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="26f1f-107">Durante o provisionamento de agendamento, os clientes podem usar o [método Get](schedule-get.md) para obter o agendamento e observar a `provisionStatus` propriedade para o estado atual do provisionamento.</span><span class="sxs-lookup"><span data-stu-id="26f1f-107">During schedule provisioning, clients can use the [GET method](schedule-get.md) to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="26f1f-108">Se o provisionamento falhar, os clientes poderão obter informações adicionais da `provisionStatusCode` propriedade.</span><span class="sxs-lookup"><span data-stu-id="26f1f-108">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="26f1f-109">Os clientes também podem inspecionar a configuração do cronograma.</span><span class="sxs-lookup"><span data-stu-id="26f1f-109">Clients can also inspect the configuration of the schedule.</span></span>


## <a name="permissions"></a><span data-ttu-id="26f1f-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="26f1f-110">Permissions</span></span>

<span data-ttu-id="26f1f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26f1f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26f1f-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26f1f-113">Permission type</span></span>      | <span data-ttu-id="26f1f-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26f1f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26f1f-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26f1f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="26f1f-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26f1f-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="26f1f-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26f1f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26f1f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26f1f-118">Not supported.</span></span>    |
|<span data-ttu-id="26f1f-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26f1f-119">Application</span></span> | <span data-ttu-id="26f1f-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26f1f-120">Not supported.</span></span> |

> <span data-ttu-id="26f1f-121">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="26f1f-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="26f1f-122">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="26f1f-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="26f1f-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26f1f-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="26f1f-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26f1f-124">Request headers</span></span>

| <span data-ttu-id="26f1f-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26f1f-125">Header</span></span>       | <span data-ttu-id="26f1f-126">Valor</span><span class="sxs-lookup"><span data-stu-id="26f1f-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="26f1f-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="26f1f-127">Authorization</span></span>  | <span data-ttu-id="26f1f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26f1f-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="26f1f-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26f1f-130">Content-Type</span></span>  | <span data-ttu-id="26f1f-131">application/json</span><span class="sxs-lookup"><span data-stu-id="26f1f-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="26f1f-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26f1f-132">Request body</span></span>

<span data-ttu-id="26f1f-133">No corpo da solicitação, forneça uma representação JSON de um objeto [Schedule](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="26f1f-133">In the request body, supply a JSON representation of a [schedule](../resources/schedule.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="26f1f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="26f1f-134">Response</span></span>

<span data-ttu-id="26f1f-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Schedule](../resources/schedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26f1f-135">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26f1f-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26f1f-136">Example</span></span>

#### <a name="request"></a><span data-ttu-id="26f1f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26f1f-137">Request</span></span>

<span data-ttu-id="26f1f-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="26f1f-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "team-put-schedule"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule
Content-type: application/json

{
  "enabled": true,
  "timeZone": "America/Chicago"
}
```

#### <a name="response"></a><span data-ttu-id="26f1f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="26f1f-139">Response</span></span>

<span data-ttu-id="26f1f-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="26f1f-140">The following is an example of the response.</span></span> 

><span data-ttu-id="26f1f-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26f1f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "provisionStatusCode": null
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
  "suppressions": []
}
-->
