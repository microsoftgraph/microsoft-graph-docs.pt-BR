---
title: tipo de recurso mobileAppTroubleshootingAppUpdateHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 536dcd025d76126f813afec5ee2e05a20b1866e6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222153"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="7e5f9-103">tipo de recurso mobileAppTroubleshootingAppUpdateHistory</span><span class="sxs-lookup"><span data-stu-id="7e5f9-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

<span data-ttu-id="7e5f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e5f9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e5f9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7e5f9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e5f9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7e5f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e5f9-107">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="7e5f9-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="7e5f9-108">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="7e5f9-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7e5f9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7e5f9-109">Properties</span></span>
|<span data-ttu-id="7e5f9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e5f9-110">Property</span></span>|<span data-ttu-id="7e5f9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e5f9-111">Type</span></span>|<span data-ttu-id="7e5f9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e5f9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e5f9-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="7e5f9-113">occurrenceDateTime</span></span>|<span data-ttu-id="7e5f9-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e5f9-114">DateTimeOffset</span></span>|<span data-ttu-id="7e5f9-115">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="7e5f9-115">Time when the history item occurred.</span></span> <span data-ttu-id="7e5f9-116">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="7e5f9-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="7e5f9-117">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="7e5f9-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="7e5f9-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="7e5f9-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="7e5f9-119">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="7e5f9-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="7e5f9-120">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="7e5f9-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e5f9-121">Relações</span><span class="sxs-lookup"><span data-stu-id="7e5f9-121">Relationships</span></span>
<span data-ttu-id="7e5f9-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7e5f9-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e5f9-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7e5f9-123">JSON Representation</span></span>
<span data-ttu-id="7e5f9-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7e5f9-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppUpdateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppUpdateHistory",
  "occurrenceDateTime": "String (timestamp)",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  }
}
```




