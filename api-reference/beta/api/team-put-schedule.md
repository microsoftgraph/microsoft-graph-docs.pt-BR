---
title: Criar ou substituir agendamento
description: Criar ou substituir um objeto **Schedule** .
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ddae7a348d4150e8ef36974fecfe6b2c276b7f1d
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657480"
---
# <a name="create-or-replace-schedule"></a><span data-ttu-id="dabd8-103">Criar ou substituir agendamento</span><span class="sxs-lookup"><span data-stu-id="dabd8-103">Create or replace schedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dabd8-104">Criar ou substituir um objeto [Schedule](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="dabd8-104">Create or replace a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="dabd8-105">O processo de criação de agendamento está em conformidade com a [diretriz de uma API para operações de longa duração com base em recursos (relo)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span><span class="sxs-lookup"><span data-stu-id="dabd8-105">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="dabd8-106">Quando os clientes usam o método PUT, se a agenda for provisionada, a operação substituirá a agenda; caso contrário, a operação iniciará o processo de provisionamento de agendamento em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="dabd8-106">When clients use the PUT method, if the schedule is provisioned, the operation replaces the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="dabd8-107">Durante o provisionamento de agendamento, os clientes podem usar o [método Get](schedule-get.md) para obter o agendamento e observar a `provisionStatus` propriedade para o estado atual do provisionamento.</span><span class="sxs-lookup"><span data-stu-id="dabd8-107">During schedule provisioning, clients can use the [GET method](schedule-get.md) to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="dabd8-108">Se o provisionamento falhar, os clientes poderão obter informações adicionais da `provisionStatusCode` propriedade.</span><span class="sxs-lookup"><span data-stu-id="dabd8-108">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="dabd8-109">Os clientes também podem inspecionar a configuração do cronograma.</span><span class="sxs-lookup"><span data-stu-id="dabd8-109">Clients can also inspect the configuration of the schedule.</span></span>


## <a name="permissions"></a><span data-ttu-id="dabd8-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="dabd8-110">Permissions</span></span>

<span data-ttu-id="dabd8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dabd8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dabd8-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dabd8-113">Permission type</span></span>      | <span data-ttu-id="dabd8-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dabd8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dabd8-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dabd8-115">Delegated (work or school account)</span></span> | <span data-ttu-id="dabd8-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dabd8-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dabd8-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dabd8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dabd8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dabd8-118">Not supported.</span></span>    |
|<span data-ttu-id="dabd8-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dabd8-119">Application</span></span> | <span data-ttu-id="dabd8-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dabd8-120">Not supported.</span></span> |

> <span data-ttu-id="dabd8-121">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="dabd8-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="dabd8-122">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="dabd8-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="dabd8-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dabd8-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="dabd8-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dabd8-124">Request headers</span></span>

| <span data-ttu-id="dabd8-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dabd8-125">Header</span></span>       | <span data-ttu-id="dabd8-126">Valor</span><span class="sxs-lookup"><span data-stu-id="dabd8-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dabd8-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="dabd8-127">Authorization</span></span>  | <span data-ttu-id="dabd8-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dabd8-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dabd8-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dabd8-130">Content-Type</span></span>  | <span data-ttu-id="dabd8-131">application/json</span><span class="sxs-lookup"><span data-stu-id="dabd8-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dabd8-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dabd8-132">Request body</span></span>

<span data-ttu-id="dabd8-133">No corpo da solicitação, forneça uma representação JSON de um objeto [Schedule](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="dabd8-133">In the request body, supply a JSON representation of a [schedule](../resources/schedule.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dabd8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dabd8-134">Response</span></span>

<span data-ttu-id="dabd8-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Schedule](../resources/schedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dabd8-135">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dabd8-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dabd8-136">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dabd8-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dabd8-137">Request</span></span>

<span data-ttu-id="dabd8-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dabd8-138">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="dabd8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="dabd8-139">Response</span></span>

<span data-ttu-id="dabd8-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dabd8-140">The following is an example of the response.</span></span> 

><span data-ttu-id="dabd8-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dabd8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/team-put-schedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
