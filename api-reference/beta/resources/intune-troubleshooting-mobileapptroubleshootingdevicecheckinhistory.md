---
title: tipo de recurso mobileAppTroubleshootingDeviceCheckinHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f8bbcbd3b8291b16fa1cae1eb7c4b3fba30baf6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570023"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="874bc-103">tipo de recurso mobileAppTroubleshootingDeviceCheckinHistory</span><span class="sxs-lookup"><span data-stu-id="874bc-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="874bc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="874bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="874bc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="874bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="874bc-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="874bc-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="874bc-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="874bc-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="874bc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="874bc-108">Properties</span></span>
|<span data-ttu-id="874bc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="874bc-109">Property</span></span>|<span data-ttu-id="874bc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="874bc-110">Type</span></span>|<span data-ttu-id="874bc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="874bc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="874bc-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="874bc-112">occurrenceDateTime</span></span>|<span data-ttu-id="874bc-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="874bc-113">DateTimeOffset</span></span>|<span data-ttu-id="874bc-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="874bc-114">Time when the history item occurred.</span></span> <span data-ttu-id="874bc-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="874bc-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="874bc-116">Relações</span><span class="sxs-lookup"><span data-stu-id="874bc-116">Relationships</span></span>
<span data-ttu-id="874bc-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="874bc-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="874bc-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="874bc-118">JSON Representation</span></span>
<span data-ttu-id="874bc-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="874bc-119">Here is a JSON representation of the resource.</span></span>
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



