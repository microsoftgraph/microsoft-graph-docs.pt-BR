---
title: tipo de recurso configurationManageraction
description: Parâmetro para a ação triggerConfigurationManagerAction
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff71bc6b4094543e3da6d22639014f595a86ce7d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199677"
---
# <a name="configurationmanageraction-resource-type"></a><span data-ttu-id="b1c2b-103">tipo de recurso configurationManageraction</span><span class="sxs-lookup"><span data-stu-id="b1c2b-103">configurationManagerAction resource type</span></span>

> <span data-ttu-id="b1c2b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1c2b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1c2b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1c2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1c2b-106">Parâmetro para a ação triggerConfigurationManagerAction</span><span class="sxs-lookup"><span data-stu-id="b1c2b-106">Parameter for action triggerConfigurationManagerAction</span></span>

## <a name="properties"></a><span data-ttu-id="b1c2b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1c2b-107">Properties</span></span>
|<span data-ttu-id="b1c2b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1c2b-108">Property</span></span>|<span data-ttu-id="b1c2b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1c2b-109">Type</span></span>|<span data-ttu-id="b1c2b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1c2b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1c2b-111">ação</span><span class="sxs-lookup"><span data-stu-id="b1c2b-111">action</span></span>|[<span data-ttu-id="b1c2b-112">configurationManagerActionType</span><span class="sxs-lookup"><span data-stu-id="b1c2b-112">configurationManagerActionType</span></span>](../resources/intune-devices-configurationmanageractiontype.md)|<span data-ttu-id="b1c2b-113">O tipo de ação a ser disparado no cliente do Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="b1c2b-113">The action type to trigger on Configuration Manager client.</span></span> <span data-ttu-id="b1c2b-114">Os valores possíveis são: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.</span><span class="sxs-lookup"><span data-stu-id="b1c2b-114">Possible values are: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1c2b-115">Relações</span><span class="sxs-lookup"><span data-stu-id="b1c2b-115">Relationships</span></span>
<span data-ttu-id="b1c2b-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1c2b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1c2b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1c2b-117">JSON Representation</span></span>
<span data-ttu-id="b1c2b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1c2b-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerAction",
  "action": "String"
}
```



