---
title: tipo de recurso mobileAppTroubleshootingHistoryItem
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 14298388574375a0beb7e638cb64d19e093452bb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993221"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="fde5d-103">tipo de recurso mobileAppTroubleshootingHistoryItem</span><span class="sxs-lookup"><span data-stu-id="fde5d-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

<span data-ttu-id="fde5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fde5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fde5d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fde5d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fde5d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fde5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fde5d-107">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="fde5d-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="fde5d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fde5d-108">Properties</span></span>
|<span data-ttu-id="fde5d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fde5d-109">Property</span></span>|<span data-ttu-id="fde5d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fde5d-110">Type</span></span>|<span data-ttu-id="fde5d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fde5d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fde5d-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="fde5d-112">occurrenceDateTime</span></span>|<span data-ttu-id="fde5d-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fde5d-113">DateTimeOffset</span></span>|<span data-ttu-id="fde5d-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="fde5d-114">Time when the history item occurred.</span></span>|
|<span data-ttu-id="fde5d-115">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="fde5d-115">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="fde5d-116">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="fde5d-116">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="fde5d-117">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="fde5d-117">Object containing detailed information about the error and its remediation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fde5d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="fde5d-118">Relationships</span></span>
<span data-ttu-id="fde5d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fde5d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fde5d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fde5d-120">JSON Representation</span></span>
<span data-ttu-id="fde5d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fde5d-121">Here is a JSON representation of the resource.</span></span>
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






