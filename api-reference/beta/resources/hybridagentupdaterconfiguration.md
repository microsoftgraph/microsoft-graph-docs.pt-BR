---
title: tipo de recurso hybridAgentUpdaterConfiguration
description: tipo de recurso hybridAgentUpdaterConfiguration.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5054ab7c22cb35a846df29ea058e0d3c02c5e7e4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440509"
---
# <a name="hybridagentupdaterconfiguration-resource-type"></a><span data-ttu-id="4b1ab-103">tipo de recurso hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b1ab-103">hybridAgentUpdaterConfiguration resource type</span></span>

<span data-ttu-id="4b1ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b1ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b1ab-105">Um administrador de locatários pode configurar para cada onPremisesPublishingProfile a janela de tempo durante a qual os agentes podem receber atualizações ou adiar atualizações para os agentes.</span><span class="sxs-lookup"><span data-stu-id="4b1ab-105">A tenant admin can configure for each onPremisesPublishingProfile the time window during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="4b1ab-106">O hybridAgentUpdaterConfiguration especificado para um onPremisesPublishingProfile é aplicável a todos os agentes dentro desse onPremisesPublishingProfile.</span><span class="sxs-lookup"><span data-stu-id="4b1ab-106">The hybridAgentUpdaterConfiguration specified for an onPremisesPublishingProfile is applicable to all the agents within that onPremisesPublishingProfile.</span></span>

<span data-ttu-id="4b1ab-107">Por exemplo, para os agentes no onPremisesPublishingProfile do tipo "Provisioning", as etapas podem ser as seguintes:</span><span class="sxs-lookup"><span data-stu-id="4b1ab-107">For example, for the agents in onPremisesPublishingProfile of type "provisioning" the steps could be as below.</span></span>

1) <span data-ttu-id="4b1ab-108">O administrador de locatários pode configurar o para não receber nenhuma atualização para os agentes de provisionamento nos próximos n dias.</span><span class="sxs-lookup"><span data-stu-id="4b1ab-108">Tenant administrator can configure to not receive any updates to the Provisioning agents for the next n days.</span></span>
2) <span data-ttu-id="4b1ab-109">O administrador de locatários pode configurar uma janela de atualização (hora de início e de término) durante a qual os agentes podem recive atualizações.</span><span class="sxs-lookup"><span data-stu-id="4b1ab-109">Tenant administrator can configure an update window(start and end time) during which the agents can recive updates.</span></span>
3) <span data-ttu-id="4b1ab-110">O administrador de locatários pode habilitar o allowUpdateConfigurationOverride que substitui o configutration atualizador de agentes de provisionamento e alows que eles recebam a próxima atualização disponível.</span><span class="sxs-lookup"><span data-stu-id="4b1ab-110">Tenant administrator can enable allowUpdateConfigurationOverride which overrides the updater configutration for Provisioning agents and alows them to receive the next available update.</span></span>

<span data-ttu-id="4b1ab-111">As informações de data/hora especificadas na configuração do atualizador serão convertidas no fuso horário local relatado pelo agente durante a evaluvation.</span><span class="sxs-lookup"><span data-stu-id="4b1ab-111">The DateTime/Time information specified in the updater configuration will be converted to the local timezone reported by the agent during evaluvation.</span></span>

<span data-ttu-id="4b1ab-112">A atualização do agente seguirá a lista de prioridades abaixo</span><span class="sxs-lookup"><span data-stu-id="4b1ab-112">The update of the agent will follow the below priority list</span></span>

1) <span data-ttu-id="4b1ab-113">Se allowUpdateConfigurationOverride for definido como true, a configuração do atualizador definida pelo locatário será ignorada e o agente receberá uma atualização quando a próxima versão do agente estiver disponível (prioridade 1).</span><span class="sxs-lookup"><span data-stu-id="4b1ab-113">If allowUpdateConfigurationOverride is set to true the updater configuration set by the tenant will be skipped and the agent will receive an update when the next version of the agent is available (priority 1).</span></span>
2) <span data-ttu-id="4b1ab-114">Se a atualização de adiamento estiver definida, o agente não será atualizado até a data de término da atualização (prioridade 2).</span><span class="sxs-lookup"><span data-stu-id="4b1ab-114">If the defer update is set, the agent will not be updated until the defer update date time (priority 2).</span></span>
3) <span data-ttu-id="4b1ab-115">Se a janela de atualização for definida, o agente só será atualizado durante essa janela de tempo em um dia de 24 horas (prioridade 3).</span><span class="sxs-lookup"><span data-stu-id="4b1ab-115">If the update window is set, the agent will be updated only during that time window in a 24 hour day (priority 3).</span></span>
4) <span data-ttu-id="4b1ab-116">Se nenhuma configuração válida do Updater for definida pelo locatário, o agente receberá uma atualização quando a próxima versão do agente estiver disponível</span><span class="sxs-lookup"><span data-stu-id="4b1ab-116">If no valid updater configuration is set by the tenant, the agent will receive an update when the next version of the agent is available</span></span>

## <a name="properties"></a><span data-ttu-id="4b1ab-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b1ab-117">Properties</span></span>

| <span data-ttu-id="4b1ab-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b1ab-118">Property</span></span>     | <span data-ttu-id="4b1ab-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b1ab-119">Type</span></span>        | <span data-ttu-id="4b1ab-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b1ab-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4b1ab-121">allowUpdateConfigurationOverride</span><span class="sxs-lookup"><span data-stu-id="4b1ab-121">allowUpdateConfigurationOverride</span></span>|<span data-ttu-id="4b1ab-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b1ab-122">Boolean</span></span>|<span data-ttu-id="4b1ab-123">Indica se a configuração do atualizador será ignorada e o agente receberá uma atualização quando a próxima versão do agente estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="4b1ab-123">Indicates if updater configuration will be skipped and the agent will receive an update when the next version of the agent is available.</span></span>|
|<span data-ttu-id="4b1ab-124">deferUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="4b1ab-124">deferUpdateDateTime</span></span>|<span data-ttu-id="4b1ab-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b1ab-125">DateTimeOffset</span></span>|<span data-ttu-id="4b1ab-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4b1ab-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4b1ab-128">updateWindow</span><span class="sxs-lookup"><span data-stu-id="4b1ab-128">updateWindow</span></span>|[<span data-ttu-id="4b1ab-129">updateWindow</span><span class="sxs-lookup"><span data-stu-id="4b1ab-129">updateWindow</span></span>](updatewindow.md)||

## <a name="json-representation"></a><span data-ttu-id="4b1ab-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b1ab-130">JSON representation</span></span>

<span data-ttu-id="4b1ab-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b1ab-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
  "baseType": null
}-->

```json
{
  "allowUpdateConfigurationOverride": true,
  "deferUpdateDateTime": "String (timestamp)",
  "updateWindow": {"@odata.type": "microsoft.graph.updateWindow"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hybridAgentUpdaterConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
