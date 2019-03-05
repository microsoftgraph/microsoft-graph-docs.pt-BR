---
title: tipo de recurso mobileAppTroubleshootingDeviceCheckinHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 646fb576e8590d9f5c58b2b67c6fd3612cf689f0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171215"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="ee350-103">tipo de recurso mobileAppTroubleshootingDeviceCheckinHistory</span><span class="sxs-lookup"><span data-stu-id="ee350-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="ee350-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ee350-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee350-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ee350-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee350-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="ee350-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="ee350-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="ee350-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ee350-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee350-108">Properties</span></span>
|<span data-ttu-id="ee350-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee350-109">Property</span></span>|<span data-ttu-id="ee350-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee350-110">Type</span></span>|<span data-ttu-id="ee350-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee350-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee350-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="ee350-112">occurrenceDateTime</span></span>|<span data-ttu-id="ee350-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee350-113">DateTimeOffset</span></span>|<span data-ttu-id="ee350-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="ee350-114">Time when the history item occurred.</span></span> <span data-ttu-id="ee350-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="ee350-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee350-116">Relações</span><span class="sxs-lookup"><span data-stu-id="ee350-116">Relationships</span></span>
<span data-ttu-id="ee350-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee350-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee350-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee350-118">JSON Representation</span></span>
<span data-ttu-id="ee350-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee350-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory",
  "occurrenceDateTime": "String (timestamp)"
}
```




