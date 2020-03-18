---
title: tipo de recurso mobileAppTroubleshootingHistoryItem
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c1c30f3cb1f6eb4375da4112ca51c0b8298245a6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42764415"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="3045d-103">tipo de recurso mobileAppTroubleshootingHistoryItem</span><span class="sxs-lookup"><span data-stu-id="3045d-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="3045d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3045d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3045d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3045d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3045d-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="3045d-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="3045d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3045d-107">Properties</span></span>
|<span data-ttu-id="3045d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3045d-108">Property</span></span>|<span data-ttu-id="3045d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3045d-109">Type</span></span>|<span data-ttu-id="3045d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3045d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3045d-111">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="3045d-111">occurrenceDateTime</span></span>|<span data-ttu-id="3045d-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3045d-112">DateTimeOffset</span></span>|<span data-ttu-id="3045d-113">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="3045d-113">Time when the history item occurred.</span></span>|
|<span data-ttu-id="3045d-114">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3045d-114">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="3045d-115">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3045d-115">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="3045d-116">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="3045d-116">Object containing detailed information about the error and its remediation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3045d-117">Relações</span><span class="sxs-lookup"><span data-stu-id="3045d-117">Relationships</span></span>
<span data-ttu-id="3045d-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3045d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3045d-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3045d-119">JSON Representation</span></span>
<span data-ttu-id="3045d-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3045d-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingHistoryItem",
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



