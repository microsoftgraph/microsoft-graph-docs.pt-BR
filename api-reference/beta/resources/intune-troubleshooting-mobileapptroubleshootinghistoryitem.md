---
title: tipo de recurso mobileAppTroubleshootingHistoryItem
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e63de7a150f36529237aac6f5f0794c8407e13e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938671"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="ea51b-103">tipo de recurso mobileAppTroubleshootingHistoryItem</span><span class="sxs-lookup"><span data-stu-id="ea51b-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="ea51b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ea51b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea51b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea51b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea51b-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="ea51b-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="ea51b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea51b-107">Properties</span></span>
|<span data-ttu-id="ea51b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea51b-108">Property</span></span>|<span data-ttu-id="ea51b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea51b-109">Type</span></span>|<span data-ttu-id="ea51b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea51b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea51b-111">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="ea51b-111">occurrenceDateTime</span></span>|<span data-ttu-id="ea51b-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea51b-112">DateTimeOffset</span></span>|<span data-ttu-id="ea51b-113">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="ea51b-113">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea51b-114">Relações</span><span class="sxs-lookup"><span data-stu-id="ea51b-114">Relationships</span></span>
<span data-ttu-id="ea51b-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea51b-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea51b-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea51b-116">JSON Representation</span></span>
<span data-ttu-id="ea51b-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea51b-117">Here is a JSON representation of the resource.</span></span>
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




