---
title: tipo de recurso mobileAppTroubleshootingDeviceCheckinHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: af7daab0b92e1753438cf8b77d129127ee7572ec
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42764436"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="14e8d-103">tipo de recurso mobileAppTroubleshootingDeviceCheckinHistory</span><span class="sxs-lookup"><span data-stu-id="14e8d-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="14e8d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14e8d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14e8d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14e8d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14e8d-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="14e8d-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="14e8d-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="14e8d-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="14e8d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14e8d-108">Properties</span></span>
|<span data-ttu-id="14e8d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14e8d-109">Property</span></span>|<span data-ttu-id="14e8d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="14e8d-110">Type</span></span>|<span data-ttu-id="14e8d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="14e8d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14e8d-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="14e8d-112">occurrenceDateTime</span></span>|<span data-ttu-id="14e8d-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14e8d-113">DateTimeOffset</span></span>|<span data-ttu-id="14e8d-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="14e8d-114">Time when the history item occurred.</span></span> <span data-ttu-id="14e8d-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="14e8d-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="14e8d-116">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="14e8d-116">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="14e8d-117">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="14e8d-117">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="14e8d-118">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="14e8d-118">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="14e8d-119">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="14e8d-119">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="14e8d-120">Relações</span><span class="sxs-lookup"><span data-stu-id="14e8d-120">Relationships</span></span>
<span data-ttu-id="14e8d-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="14e8d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14e8d-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14e8d-122">JSON Representation</span></span>
<span data-ttu-id="14e8d-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="14e8d-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory",
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



