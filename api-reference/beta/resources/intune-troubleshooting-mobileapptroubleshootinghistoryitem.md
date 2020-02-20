---
title: tipo de recurso mobileAppTroubleshootingHistoryItem
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c04239119d475f1dc3763ddbcd811afe7783efc2
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163714"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="14bbc-103">tipo de recurso mobileAppTroubleshootingHistoryItem</span><span class="sxs-lookup"><span data-stu-id="14bbc-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="14bbc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14bbc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14bbc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14bbc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14bbc-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="14bbc-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="14bbc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14bbc-107">Properties</span></span>
|<span data-ttu-id="14bbc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14bbc-108">Property</span></span>|<span data-ttu-id="14bbc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="14bbc-109">Type</span></span>|<span data-ttu-id="14bbc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="14bbc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14bbc-111">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="14bbc-111">occurrenceDateTime</span></span>|<span data-ttu-id="14bbc-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14bbc-112">DateTimeOffset</span></span>|<span data-ttu-id="14bbc-113">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="14bbc-113">Time when the history item occurred.</span></span>|
|<span data-ttu-id="14bbc-114">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="14bbc-114">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="14bbc-115">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="14bbc-115">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="14bbc-116">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="14bbc-116">Object containing detailed information about the error and its remediation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14bbc-117">Relações</span><span class="sxs-lookup"><span data-stu-id="14bbc-117">Relationships</span></span>
<span data-ttu-id="14bbc-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="14bbc-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14bbc-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14bbc-119">JSON Representation</span></span>
<span data-ttu-id="14bbc-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="14bbc-120">Here is a JSON representation of the resource.</span></span>
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



