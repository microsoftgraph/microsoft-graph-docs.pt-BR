---
title: tipo de recurso mobileAppTroubleshootingHistoryItem
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fbc37488f478c47b0b097c4fd8a54b09273bc5c3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160855"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="40a4d-103">tipo de recurso mobileAppTroubleshootingHistoryItem</span><span class="sxs-lookup"><span data-stu-id="40a4d-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="40a4d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40a4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40a4d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40a4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40a4d-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="40a4d-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="40a4d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40a4d-107">Properties</span></span>
|<span data-ttu-id="40a4d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40a4d-108">Property</span></span>|<span data-ttu-id="40a4d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="40a4d-109">Type</span></span>|<span data-ttu-id="40a4d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="40a4d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40a4d-111">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="40a4d-111">occurrenceDateTime</span></span>|<span data-ttu-id="40a4d-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40a4d-112">DateTimeOffset</span></span>|<span data-ttu-id="40a4d-113">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="40a4d-113">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40a4d-114">Relações</span><span class="sxs-lookup"><span data-stu-id="40a4d-114">Relationships</span></span>
<span data-ttu-id="40a4d-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40a4d-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40a4d-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40a4d-116">JSON Representation</span></span>
<span data-ttu-id="40a4d-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="40a4d-117">Here is a JSON representation of the resource.</span></span>
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




