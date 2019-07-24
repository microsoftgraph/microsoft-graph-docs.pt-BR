---
title: tipo de recurso hybridAgentUpdaterConfiguration
description: tipo de recurso hybridAgentUpdaterConfiguration.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5c3efdd55f432add28f6d13797a0f73b4458b966
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841245"
---
# <a name="hybridagentupdaterconfiguration-resource-type"></a><span data-ttu-id="e9fc5-103">tipo de recurso hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9fc5-103">hybridAgentUpdaterConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9fc5-104">Um administrador de locatários pode configurar para cada onPremisesPublishingProfile a janela de tempo durante a qual os agentes podem receber atualizações ou adiar atualizações para os agentes.</span><span class="sxs-lookup"><span data-stu-id="e9fc5-104">A tenant admin can configure for each onPremisesPublishingProfile the time window during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="e9fc5-105">O hybridAgentUpdaterConfiguration especificado para um onPremisesPublishingProfile é aplicável a todos os agentes dentro desse onPremisesPublishingProfile.</span><span class="sxs-lookup"><span data-stu-id="e9fc5-105">The hybridAgentUpdaterConfiguration specified for an onPremisesPublishingProfile is applicable to all the agents within that onPremisesPublishingProfile.</span></span>

<span data-ttu-id="e9fc5-106">Por exemplo, para os agentes no onPremisesPublishingProfile do tipo "Provisioning", as etapas podem ser as seguintes:</span><span class="sxs-lookup"><span data-stu-id="e9fc5-106">For example, for the agents in onPremisesPublishingProfile of type "provisioning" the steps could be as below.</span></span>

1) <span data-ttu-id="e9fc5-107">O administrador de locatários pode configurar o para não receber nenhuma atualização para os agentes de provisionamento nos próximos n dias.</span><span class="sxs-lookup"><span data-stu-id="e9fc5-107">Tenant administrator can configure to not receive any updates to the Provisioning agents for the next n days.</span></span>
2) <span data-ttu-id="e9fc5-108">O administrador de locatários pode configurar uma janela de atualização (hora de início e de término) durante a qual os agentes podem recive atualizações.</span><span class="sxs-lookup"><span data-stu-id="e9fc5-108">Tenant administrator can configure an update window(start and end time) during which the agents can recive updates.</span></span>
3) <span data-ttu-id="e9fc5-109">O administrador de locatários pode habilitar o allowUpdateConfigurationOverride que substitui o configutration atualizador de agentes de provisionamento e alows que eles recebam a próxima atualização disponível.</span><span class="sxs-lookup"><span data-stu-id="e9fc5-109">Tenant administrator can enable allowUpdateConfigurationOverride which overrides the updater configutration for Provisioning agents and alows them to receive the next available update.</span></span>

<span data-ttu-id="e9fc5-110">As informações de data/hora especificadas na configuração do atualizador serão convertidas no fuso horário local relatado pelo agente durante a evaluvation.</span><span class="sxs-lookup"><span data-stu-id="e9fc5-110">The DateTime/Time information specified in the updater configuration will be converted to the local timezone reported by the agent during evaluvation.</span></span>

<span data-ttu-id="e9fc5-111">A atualização do agente seguirá a lista de prioridades abaixo</span><span class="sxs-lookup"><span data-stu-id="e9fc5-111">The update of the agent will follow the below priority list</span></span>

1) <span data-ttu-id="e9fc5-112">Se allowUpdateConfigurationOverride for definido como true, a configuração do atualizador definida pelo locatário será ignorada e o agente receberá uma atualização quando a próxima versão do agente estiver disponível (prioridade 1).</span><span class="sxs-lookup"><span data-stu-id="e9fc5-112">If allowUpdateConfigurationOverride is set to true the updater configuration set by the tenant will be skipped and the agent will receive an update when the next version of the agent is available (priority 1).</span></span>
2) <span data-ttu-id="e9fc5-113">Se a atualização de adiamento estiver definida, o agente não será atualizado até a data de término da atualização (prioridade 2).</span><span class="sxs-lookup"><span data-stu-id="e9fc5-113">If the defer update is set, the agent will not be updated until the defer update date time (priority 2).</span></span>
3) <span data-ttu-id="e9fc5-114">Se a janela de atualização for definida, o agente só será atualizado durante essa janela de tempo em um dia de 24 horas (prioridade 3).</span><span class="sxs-lookup"><span data-stu-id="e9fc5-114">If the update window is set, the agent will be updated only during that time window in a 24 hour day (priority 3).</span></span>
4) <span data-ttu-id="e9fc5-115">Se nenhuma configuração válida do Updater for definida pelo locatário, o agente receberá uma atualização quando a próxima versão do agente estiver disponível</span><span class="sxs-lookup"><span data-stu-id="e9fc5-115">If no valid updater configuration is set by the tenant, the agent will receive an update when the next version of the agent is available</span></span>

## <a name="properties"></a><span data-ttu-id="e9fc5-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e9fc5-116">Properties</span></span>

| <span data-ttu-id="e9fc5-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9fc5-117">Property</span></span>     | <span data-ttu-id="e9fc5-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9fc5-118">Type</span></span>        | <span data-ttu-id="e9fc5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9fc5-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e9fc5-120">allowUpdateConfigurationOverride</span><span class="sxs-lookup"><span data-stu-id="e9fc5-120">allowUpdateConfigurationOverride</span></span>|<span data-ttu-id="e9fc5-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="e9fc5-121">Boolean</span></span>|<span data-ttu-id="e9fc5-122">Indica se a configuração do atualizador será ignorada e o agente receberá uma atualização quando a próxima versão do agente estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="e9fc5-122">Indicates if updater configuration will be skipped and the agent will receive an update when the next version of the agent is available.</span></span>|
|<span data-ttu-id="e9fc5-123">deferUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="e9fc5-123">deferUpdateDateTime</span></span>|<span data-ttu-id="e9fc5-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9fc5-124">DateTimeOffset</span></span>|<span data-ttu-id="e9fc5-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e9fc5-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e9fc5-127">updateWindow</span><span class="sxs-lookup"><span data-stu-id="e9fc5-127">updateWindow</span></span>|[<span data-ttu-id="e9fc5-128">updateWindow</span><span class="sxs-lookup"><span data-stu-id="e9fc5-128">updateWindow</span></span>](updatewindow.md)||

## <a name="json-representation"></a><span data-ttu-id="e9fc5-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e9fc5-129">JSON representation</span></span>

<span data-ttu-id="e9fc5-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e9fc5-130">The following is a JSON representation of the resource.</span></span>

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
