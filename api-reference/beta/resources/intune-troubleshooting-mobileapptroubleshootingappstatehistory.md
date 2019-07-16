---
title: tipo de recurso mobileAppTroubleshootingAppStateHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: efef2bb43c34c004df48453ca6a2713d445ec970
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737360"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="a8596-103">tipo de recurso mobileAppTroubleshootingAppStateHistory</span><span class="sxs-lookup"><span data-stu-id="a8596-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="a8596-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a8596-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8596-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8596-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8596-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="a8596-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="a8596-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="a8596-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a8596-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8596-108">Properties</span></span>
|<span data-ttu-id="a8596-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8596-109">Property</span></span>|<span data-ttu-id="a8596-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8596-110">Type</span></span>|<span data-ttu-id="a8596-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8596-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8596-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="a8596-112">occurrenceDateTime</span></span>|<span data-ttu-id="a8596-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8596-113">DateTimeOffset</span></span>|<span data-ttu-id="a8596-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="a8596-114">Time when the history item occurred.</span></span> <span data-ttu-id="a8596-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="a8596-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="a8596-116">actionType</span><span class="sxs-lookup"><span data-stu-id="a8596-116">actionType</span></span>|[<span data-ttu-id="a8596-117">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="a8596-117">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="a8596-118">Tipo de ação para o aplicativo do Intune.</span><span class="sxs-lookup"><span data-stu-id="a8596-118">Action type for Intune Application.</span></span> <span data-ttu-id="a8596-119">Os valores possíveis são: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="a8596-119">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="a8596-120">runState</span><span class="sxs-lookup"><span data-stu-id="a8596-120">runState</span></span>|[<span data-ttu-id="a8596-121">runState</span><span class="sxs-lookup"><span data-stu-id="a8596-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="a8596-122">Status do item.</span><span class="sxs-lookup"><span data-stu-id="a8596-122">Status of the item.</span></span> <span data-ttu-id="a8596-123">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="a8596-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="a8596-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="a8596-124">errorCode</span></span>|<span data-ttu-id="a8596-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8596-125">String</span></span>|<span data-ttu-id="a8596-126">Código de erro para a falha, vazio se não houver falha.</span><span class="sxs-lookup"><span data-stu-id="a8596-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8596-127">Relações</span><span class="sxs-lookup"><span data-stu-id="a8596-127">Relationships</span></span>
<span data-ttu-id="a8596-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8596-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8596-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8596-129">JSON Representation</span></span>
<span data-ttu-id="a8596-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8596-130">Here is a JSON representation of the resource.</span></span>
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





