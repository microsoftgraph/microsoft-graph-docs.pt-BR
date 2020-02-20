---
title: tipo de recurso mobileAppTroubleshootingAppUpdateHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0ba8969dbd74da45f9d5f89fd07524cd1f025a46
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163728"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="1f3be-103">tipo de recurso mobileAppTroubleshootingAppUpdateHistory</span><span class="sxs-lookup"><span data-stu-id="1f3be-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="1f3be-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1f3be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f3be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f3be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f3be-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="1f3be-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="1f3be-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="1f3be-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1f3be-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f3be-108">Properties</span></span>
|<span data-ttu-id="1f3be-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f3be-109">Property</span></span>|<span data-ttu-id="1f3be-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f3be-110">Type</span></span>|<span data-ttu-id="1f3be-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f3be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f3be-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="1f3be-112">occurrenceDateTime</span></span>|<span data-ttu-id="1f3be-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f3be-113">DateTimeOffset</span></span>|<span data-ttu-id="1f3be-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="1f3be-114">Time when the history item occurred.</span></span> <span data-ttu-id="1f3be-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="1f3be-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="1f3be-116">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="1f3be-116">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="1f3be-117">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="1f3be-117">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="1f3be-118">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="1f3be-118">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="1f3be-119">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="1f3be-119">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f3be-120">Relações</span><span class="sxs-lookup"><span data-stu-id="1f3be-120">Relationships</span></span>
<span data-ttu-id="1f3be-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f3be-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f3be-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f3be-122">JSON Representation</span></span>
<span data-ttu-id="1f3be-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f3be-123">Here is a JSON representation of the resource.</span></span>
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



