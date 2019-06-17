---
title: tipo de recurso mobileAppTroubleshootingHistoryItem
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7158855510df58b56fc63b467ec721250ca502d3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983579"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="31dc4-103">tipo de recurso mobileAppTroubleshootingHistoryItem</span><span class="sxs-lookup"><span data-stu-id="31dc4-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="31dc4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="31dc4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31dc4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="31dc4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31dc4-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="31dc4-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="31dc4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31dc4-107">Properties</span></span>
|<span data-ttu-id="31dc4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31dc4-108">Property</span></span>|<span data-ttu-id="31dc4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="31dc4-109">Type</span></span>|<span data-ttu-id="31dc4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="31dc4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31dc4-111">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="31dc4-111">occurrenceDateTime</span></span>|<span data-ttu-id="31dc4-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31dc4-112">DateTimeOffset</span></span>|<span data-ttu-id="31dc4-113">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="31dc4-113">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31dc4-114">Relações</span><span class="sxs-lookup"><span data-stu-id="31dc4-114">Relationships</span></span>
<span data-ttu-id="31dc4-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="31dc4-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="31dc4-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31dc4-116">JSON Representation</span></span>
<span data-ttu-id="31dc4-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="31dc4-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingHistoryItem",
  "occurrenceDateTime": "String (timestamp)"
}
```





