---
title: tipo de recurso mobileAppTroubleshootingDeviceCheckinHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f8bbcbd3b8291b16fa1cae1eb7c4b3fba30baf6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784856"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="e9808-103">tipo de recurso mobileAppTroubleshootingDeviceCheckinHistory</span><span class="sxs-lookup"><span data-stu-id="e9808-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="e9808-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e9808-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9808-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9808-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9808-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e9808-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="e9808-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e9808-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e9808-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e9808-108">Properties</span></span>
|<span data-ttu-id="e9808-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9808-109">Property</span></span>|<span data-ttu-id="e9808-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9808-110">Type</span></span>|<span data-ttu-id="e9808-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9808-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9808-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="e9808-112">occurrenceDateTime</span></span>|<span data-ttu-id="e9808-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9808-113">DateTimeOffset</span></span>|<span data-ttu-id="e9808-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="e9808-114">Time when the history item occurred.</span></span> <span data-ttu-id="e9808-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e9808-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9808-116">Relações</span><span class="sxs-lookup"><span data-stu-id="e9808-116">Relationships</span></span>
<span data-ttu-id="e9808-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e9808-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9808-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e9808-118">JSON Representation</span></span>
<span data-ttu-id="e9808-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e9808-119">Here is a JSON representation of the resource.</span></span>
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



