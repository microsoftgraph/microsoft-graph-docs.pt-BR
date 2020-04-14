---
title: tipo de recurso mobileAppTroubleshootingAppUpdateHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 72eedcfc1c3031a8c571d4f490a74def6a0fd9de
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388234"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="567fa-103">tipo de recurso mobileAppTroubleshootingAppUpdateHistory</span><span class="sxs-lookup"><span data-stu-id="567fa-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

<span data-ttu-id="567fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="567fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="567fa-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="567fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="567fa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="567fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="567fa-107">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="567fa-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="567fa-108">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="567fa-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="567fa-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="567fa-109">Properties</span></span>
|<span data-ttu-id="567fa-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="567fa-110">Property</span></span>|<span data-ttu-id="567fa-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="567fa-111">Type</span></span>|<span data-ttu-id="567fa-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="567fa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="567fa-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="567fa-113">occurrenceDateTime</span></span>|<span data-ttu-id="567fa-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="567fa-114">DateTimeOffset</span></span>|<span data-ttu-id="567fa-115">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="567fa-115">Time when the history item occurred.</span></span> <span data-ttu-id="567fa-116">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="567fa-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="567fa-117">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="567fa-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="567fa-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="567fa-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="567fa-119">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="567fa-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="567fa-120">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="567fa-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="567fa-121">Relações</span><span class="sxs-lookup"><span data-stu-id="567fa-121">Relationships</span></span>
<span data-ttu-id="567fa-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="567fa-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="567fa-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="567fa-123">JSON Representation</span></span>
<span data-ttu-id="567fa-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="567fa-124">Here is a JSON representation of the resource.</span></span>
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



