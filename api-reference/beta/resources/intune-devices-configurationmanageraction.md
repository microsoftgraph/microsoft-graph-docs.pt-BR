---
title: tipo de recurso configurationManageraction
description: Parâmetro para a ação triggerConfigurationManagerAction
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b16f09234c1c0c90930b99044648aa8d4236a023
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060710"
---
# <a name="configurationmanageraction-resource-type"></a><span data-ttu-id="2d056-103">tipo de recurso configurationManageraction</span><span class="sxs-lookup"><span data-stu-id="2d056-103">configurationManagerAction resource type</span></span>

<span data-ttu-id="2d056-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d056-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d056-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2d056-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d056-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d056-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d056-107">Parâmetro para a ação triggerConfigurationManagerAction</span><span class="sxs-lookup"><span data-stu-id="2d056-107">Parameter for action triggerConfigurationManagerAction</span></span>

## <a name="properties"></a><span data-ttu-id="2d056-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d056-108">Properties</span></span>
|<span data-ttu-id="2d056-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d056-109">Property</span></span>|<span data-ttu-id="2d056-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d056-110">Type</span></span>|<span data-ttu-id="2d056-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d056-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d056-112">ação</span><span class="sxs-lookup"><span data-stu-id="2d056-112">action</span></span>|[<span data-ttu-id="2d056-113">configurationManagerActionType</span><span class="sxs-lookup"><span data-stu-id="2d056-113">configurationManagerActionType</span></span>](../resources/intune-devices-configurationmanageractiontype.md)|<span data-ttu-id="2d056-114">O tipo de ação a ser disparado no cliente do Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="2d056-114">The action type to trigger on Configuration Manager client.</span></span> <span data-ttu-id="2d056-115">Os valores possíveis são: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.</span><span class="sxs-lookup"><span data-stu-id="2d056-115">Possible values are: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d056-116">Relações</span><span class="sxs-lookup"><span data-stu-id="2d056-116">Relationships</span></span>
<span data-ttu-id="2d056-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2d056-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d056-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d056-118">JSON Representation</span></span>
<span data-ttu-id="2d056-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d056-119">Here is a JSON representation of the resource.</span></span>
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






