---
title: tipo de recurso configurationManageraction
description: Parâmetro para a ação triggerConfigurationManagerAction
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 04d78d751f6cdd2978aa9cc65942acf312482202
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785095"
---
# <a name="configurationmanageraction-resource-type"></a><span data-ttu-id="337c2-103">tipo de recurso configurationManageraction</span><span class="sxs-lookup"><span data-stu-id="337c2-103">configurationManagerAction resource type</span></span>

> <span data-ttu-id="337c2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="337c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="337c2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="337c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="337c2-106">Parâmetro para a ação triggerConfigurationManagerAction</span><span class="sxs-lookup"><span data-stu-id="337c2-106">Parameter for action triggerConfigurationManagerAction</span></span>

## <a name="properties"></a><span data-ttu-id="337c2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="337c2-107">Properties</span></span>
|<span data-ttu-id="337c2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="337c2-108">Property</span></span>|<span data-ttu-id="337c2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="337c2-109">Type</span></span>|<span data-ttu-id="337c2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="337c2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="337c2-111">ação</span><span class="sxs-lookup"><span data-stu-id="337c2-111">action</span></span>|[<span data-ttu-id="337c2-112">configurationManagerActionType</span><span class="sxs-lookup"><span data-stu-id="337c2-112">configurationManagerActionType</span></span>](../resources/intune-devices-configurationmanageractiontype.md)|<span data-ttu-id="337c2-113">O tipo de ação a ser disparado no cliente do Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="337c2-113">The action type to trigger on Configuration Manager client.</span></span> <span data-ttu-id="337c2-114">Os valores possíveis são: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.</span><span class="sxs-lookup"><span data-stu-id="337c2-114">Possible values are: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="337c2-115">Relações</span><span class="sxs-lookup"><span data-stu-id="337c2-115">Relationships</span></span>
<span data-ttu-id="337c2-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="337c2-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="337c2-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="337c2-117">JSON Representation</span></span>
<span data-ttu-id="337c2-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="337c2-118">Here is a JSON representation of the resource.</span></span>
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



