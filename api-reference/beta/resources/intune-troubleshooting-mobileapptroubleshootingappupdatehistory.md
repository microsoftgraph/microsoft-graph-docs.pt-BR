---
title: tipo de recurso mobileAppTroubleshootingAppUpdateHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c957f870f7a63506299a22b0b3496b6fa2096bd0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570628"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="25a13-103">tipo de recurso mobileAppTroubleshootingAppUpdateHistory</span><span class="sxs-lookup"><span data-stu-id="25a13-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="25a13-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="25a13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25a13-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="25a13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25a13-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="25a13-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="25a13-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="25a13-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="25a13-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25a13-108">Properties</span></span>
|<span data-ttu-id="25a13-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25a13-109">Property</span></span>|<span data-ttu-id="25a13-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="25a13-110">Type</span></span>|<span data-ttu-id="25a13-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="25a13-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25a13-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="25a13-112">occurrenceDateTime</span></span>|<span data-ttu-id="25a13-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25a13-113">DateTimeOffset</span></span>|<span data-ttu-id="25a13-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="25a13-114">Time when the history item occurred.</span></span> <span data-ttu-id="25a13-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="25a13-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="25a13-116">Relações</span><span class="sxs-lookup"><span data-stu-id="25a13-116">Relationships</span></span>
<span data-ttu-id="25a13-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25a13-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="25a13-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25a13-118">JSON Representation</span></span>
<span data-ttu-id="25a13-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25a13-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppUpdateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppUpdateHistory",
  "occurrenceDateTime": "String (timestamp)"
}
```



