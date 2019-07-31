---
title: tipo de recurso mobileAppTroubleshootingAppStateHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2d145212645283738d1248bd05c50b1f6658460f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967214"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="150a6-103">tipo de recurso mobileAppTroubleshootingAppStateHistory</span><span class="sxs-lookup"><span data-stu-id="150a6-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="150a6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="150a6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="150a6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="150a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="150a6-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="150a6-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="150a6-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="150a6-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="150a6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="150a6-108">Properties</span></span>
|<span data-ttu-id="150a6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="150a6-109">Property</span></span>|<span data-ttu-id="150a6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="150a6-110">Type</span></span>|<span data-ttu-id="150a6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="150a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="150a6-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="150a6-112">occurrenceDateTime</span></span>|<span data-ttu-id="150a6-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="150a6-113">DateTimeOffset</span></span>|<span data-ttu-id="150a6-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="150a6-114">Time when the history item occurred.</span></span> <span data-ttu-id="150a6-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="150a6-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="150a6-116">actionType</span><span class="sxs-lookup"><span data-stu-id="150a6-116">actionType</span></span>|[<span data-ttu-id="150a6-117">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="150a6-117">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="150a6-118">Tipo de ação para o aplicativo do Intune.</span><span class="sxs-lookup"><span data-stu-id="150a6-118">Action type for Intune Application.</span></span> <span data-ttu-id="150a6-119">Os valores possíveis são: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="150a6-119">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="150a6-120">runState</span><span class="sxs-lookup"><span data-stu-id="150a6-120">runState</span></span>|[<span data-ttu-id="150a6-121">runState</span><span class="sxs-lookup"><span data-stu-id="150a6-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="150a6-122">Status do item.</span><span class="sxs-lookup"><span data-stu-id="150a6-122">Status of the item.</span></span> <span data-ttu-id="150a6-123">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="150a6-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="150a6-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="150a6-124">errorCode</span></span>|<span data-ttu-id="150a6-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="150a6-125">String</span></span>|<span data-ttu-id="150a6-126">Código de erro para a falha, vazio se não houver falha.</span><span class="sxs-lookup"><span data-stu-id="150a6-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="150a6-127">Relações</span><span class="sxs-lookup"><span data-stu-id="150a6-127">Relationships</span></span>
<span data-ttu-id="150a6-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="150a6-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="150a6-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="150a6-129">JSON Representation</span></span>
<span data-ttu-id="150a6-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="150a6-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppStateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppStateHistory",
  "occurrenceDateTime": "String (timestamp)",
  "actionType": "String",
  "runState": "String",
  "errorCode": "String"
}
```





