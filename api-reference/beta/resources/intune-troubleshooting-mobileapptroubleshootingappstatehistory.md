---
title: tipo de recurso mobileAppTroubleshootingAppStateHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 71a5786bb5c2a89d6a4397e999155a31cc0f9369
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42729098"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="d7612-103">tipo de recurso mobileAppTroubleshootingAppStateHistory</span><span class="sxs-lookup"><span data-stu-id="d7612-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="d7612-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d7612-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7612-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d7612-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7612-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="d7612-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="d7612-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d7612-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d7612-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7612-108">Properties</span></span>
|<span data-ttu-id="d7612-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7612-109">Property</span></span>|<span data-ttu-id="d7612-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7612-110">Type</span></span>|<span data-ttu-id="d7612-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7612-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7612-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="d7612-112">occurrenceDateTime</span></span>|<span data-ttu-id="d7612-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7612-113">DateTimeOffset</span></span>|<span data-ttu-id="d7612-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="d7612-114">Time when the history item occurred.</span></span> <span data-ttu-id="d7612-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d7612-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="d7612-116">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="d7612-116">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="d7612-117">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="d7612-117">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="d7612-118">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="d7612-118">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="d7612-119">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d7612-119">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="d7612-120">actionType</span><span class="sxs-lookup"><span data-stu-id="d7612-120">actionType</span></span>|[<span data-ttu-id="d7612-121">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="d7612-121">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="d7612-122">Tipo de ação para o aplicativo do Intune.</span><span class="sxs-lookup"><span data-stu-id="d7612-122">Action type for Intune Application.</span></span> <span data-ttu-id="d7612-123">Os valores possíveis são: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="d7612-123">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="d7612-124">runState</span><span class="sxs-lookup"><span data-stu-id="d7612-124">runState</span></span>|[<span data-ttu-id="d7612-125">runState</span><span class="sxs-lookup"><span data-stu-id="d7612-125">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="d7612-126">Status do item.</span><span class="sxs-lookup"><span data-stu-id="d7612-126">Status of the item.</span></span> <span data-ttu-id="d7612-127">Os valores possíveis são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="d7612-127">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="d7612-128">errorCode</span><span class="sxs-lookup"><span data-stu-id="d7612-128">errorCode</span></span>|<span data-ttu-id="d7612-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7612-129">String</span></span>|<span data-ttu-id="d7612-130">Código de erro para a falha, vazio se não houver falha.</span><span class="sxs-lookup"><span data-stu-id="d7612-130">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7612-131">Relações</span><span class="sxs-lookup"><span data-stu-id="d7612-131">Relationships</span></span>
<span data-ttu-id="d7612-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d7612-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7612-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7612-133">JSON Representation</span></span>
<span data-ttu-id="d7612-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d7612-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppStateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppStateHistory",
  "occurrenceDateTime": "String (timestamp)",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  },
  "actionType": "String",
  "runState": "String",
  "errorCode": "String"
}
```



