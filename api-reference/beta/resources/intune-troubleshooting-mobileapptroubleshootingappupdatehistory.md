---
title: tipo de recurso mobileAppTroubleshootingAppUpdateHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3eadbec77e95dd90fd9ef819e468241bf8ef5c9e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153638"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="0c3cc-103">tipo de recurso mobileAppTroubleshootingAppUpdateHistory</span><span class="sxs-lookup"><span data-stu-id="0c3cc-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="0c3cc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0c3cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c3cc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c3cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c3cc-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="0c3cc-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="0c3cc-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="0c3cc-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0c3cc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c3cc-108">Properties</span></span>
|<span data-ttu-id="0c3cc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c3cc-109">Property</span></span>|<span data-ttu-id="0c3cc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c3cc-110">Type</span></span>|<span data-ttu-id="0c3cc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c3cc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c3cc-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="0c3cc-112">occurrenceDateTime</span></span>|<span data-ttu-id="0c3cc-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c3cc-113">DateTimeOffset</span></span>|<span data-ttu-id="0c3cc-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="0c3cc-114">Time when the history item occurred.</span></span> <span data-ttu-id="0c3cc-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="0c3cc-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c3cc-116">Relações</span><span class="sxs-lookup"><span data-stu-id="0c3cc-116">Relationships</span></span>
<span data-ttu-id="0c3cc-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c3cc-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c3cc-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c3cc-118">JSON Representation</span></span>
<span data-ttu-id="0c3cc-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c3cc-119">Here is a JSON representation of the resource.</span></span>
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




