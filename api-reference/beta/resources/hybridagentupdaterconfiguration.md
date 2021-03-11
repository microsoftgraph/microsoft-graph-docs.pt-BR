---
title: Tipo de recurso hybridAgentUpdaterConfiguration
description: Tipo de recurso hybridAgentUpdaterConfiguration.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: c81d48053e7fb26eaee678da4e4b33708717e3c1
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722395"
---
# <a name="hybridagentupdaterconfiguration-resource-type"></a><span data-ttu-id="bbe1b-103">Tipo de recurso hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="bbe1b-103">hybridAgentUpdaterConfiguration resource type</span></span>

<span data-ttu-id="bbe1b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbe1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbe1b-105">Um administrador de locatário pode configurar para cada onPremisesPublishingProfile a janela de tempo durante a qual os agentes podem receber atualizações ou adiar atualizações para os agentes.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-105">A tenant admin can configure for each onPremisesPublishingProfile the time window during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="bbe1b-106">O hybridAgentUpdaterConfiguration especificado para um onPremisesPublishingProfile é aplicável a todos os agentes dentro desse onPremisesPublishingProfile.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-106">The hybridAgentUpdaterConfiguration specified for an onPremisesPublishingProfile is applicable to all the agents within that onPremisesPublishingProfile.</span></span>

<span data-ttu-id="bbe1b-107">Por exemplo, para os agentes em onPremisesPublishingProfile do tipo "provisionamento" as etapas podem ser as seguintes.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-107">For example, for the agents in onPremisesPublishingProfile of type "provisioning" the steps could be as below.</span></span>

1) <span data-ttu-id="bbe1b-108">O administrador de locatários pode configurar para não receber atualizações para os agentes de Provisionamento para os próximos n dias.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-108">Tenant administrator can configure to not receive any updates to the Provisioning agents for the next n days.</span></span>
2) <span data-ttu-id="bbe1b-109">O administrador de locatários pode configurar uma janela de atualização(início e hora de término) durante a qual os agentes podem realinhe as atualizações.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-109">Tenant administrator can configure an update window(start and end time) during which the agents can recive updates.</span></span>
3) <span data-ttu-id="bbe1b-110">O administrador de locatários pode habilitar allowUpdateConfigurationOverride que substitui a configutração do atualizador para agentes de Provisionamento e permite que eles recebam a próxima atualização disponível.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-110">Tenant administrator can enable allowUpdateConfigurationOverride which overrides the updater configutration for Provisioning agents and alows them to receive the next available update.</span></span>

<span data-ttu-id="bbe1b-111">As informações DateTime/Time especificadas na configuração do atualizador serão convertidas no zona de tempo local relatada pelo agente durante a evaluvação.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-111">The DateTime/Time information specified in the updater configuration will be converted to the local timezone reported by the agent during evaluvation.</span></span>

<span data-ttu-id="bbe1b-112">A atualização do agente seguirá a lista de prioridade abaixo</span><span class="sxs-lookup"><span data-stu-id="bbe1b-112">The update of the agent will follow the below priority list</span></span>

1) <span data-ttu-id="bbe1b-113">Se allowUpdateConfigurationOverride for definido como true, a configuração do updater definida pelo locatário será ignorada e o agente receberá uma atualização quando a próxima versão do agente estiver disponível (prioridade 1).</span><span class="sxs-lookup"><span data-stu-id="bbe1b-113">If allowUpdateConfigurationOverride is set to true the updater configuration set by the tenant will be skipped and the agent will receive an update when the next version of the agent is available (priority 1).</span></span>
2) <span data-ttu-id="bbe1b-114">Se a atualização de adiamento estiver definida, o agente não será atualizado até a hora da atualização de adiamento (prioridade 2).</span><span class="sxs-lookup"><span data-stu-id="bbe1b-114">If the defer update is set, the agent will not be updated until the defer update date time (priority 2).</span></span>
3) <span data-ttu-id="bbe1b-115">Se a janela de atualização estiver definida, o agente será atualizado somente durante essa janela de tempo em um dia de 24 horas (prioridade 3).</span><span class="sxs-lookup"><span data-stu-id="bbe1b-115">If the update window is set, the agent will be updated only during that time window in a 24 hour day (priority 3).</span></span>
4) <span data-ttu-id="bbe1b-116">Se nenhuma configuração do atualizador válida for definida pelo locatário, o agente receberá uma atualização quando a próxima versão do agente estiver disponível</span><span class="sxs-lookup"><span data-stu-id="bbe1b-116">If no valid updater configuration is set by the tenant, the agent will receive an update when the next version of the agent is available</span></span>

## <a name="properties"></a><span data-ttu-id="bbe1b-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bbe1b-117">Properties</span></span>

| <span data-ttu-id="bbe1b-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbe1b-118">Property</span></span>     | <span data-ttu-id="bbe1b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbe1b-119">Type</span></span>        | <span data-ttu-id="bbe1b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbe1b-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bbe1b-121">allowUpdateConfigurationOverride</span><span class="sxs-lookup"><span data-stu-id="bbe1b-121">allowUpdateConfigurationOverride</span></span>|<span data-ttu-id="bbe1b-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="bbe1b-122">Boolean</span></span>|<span data-ttu-id="bbe1b-123">Indica se a configuração do atualizador será ignorada e o agente receberá uma atualização quando a próxima versão do agente estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-123">Indicates if updater configuration will be skipped and the agent will receive an update when the next version of the agent is available.</span></span>|
|<span data-ttu-id="bbe1b-124">deferUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="bbe1b-124">deferUpdateDateTime</span></span>|<span data-ttu-id="bbe1b-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbe1b-125">DateTimeOffset</span></span>|<span data-ttu-id="bbe1b-126">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bbe1b-127">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="bbe1b-127">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="bbe1b-128">updateWindow</span><span class="sxs-lookup"><span data-stu-id="bbe1b-128">updateWindow</span></span>|[<span data-ttu-id="bbe1b-129">updateWindow</span><span class="sxs-lookup"><span data-stu-id="bbe1b-129">updateWindow</span></span>](updatewindow.md)||

## <a name="json-representation"></a><span data-ttu-id="bbe1b-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bbe1b-130">JSON representation</span></span>

<span data-ttu-id="bbe1b-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bbe1b-131">The following is a JSON representation of the resource.</span></span>

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


