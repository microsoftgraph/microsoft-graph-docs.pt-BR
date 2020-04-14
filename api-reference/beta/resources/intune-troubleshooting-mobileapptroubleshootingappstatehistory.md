---
title: tipo de recurso mobileAppTroubleshootingAppStateHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 198e22884adf355dfaf05a1ab516e2d6d22f0510
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43385271"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="3f031-103">tipo de recurso mobileAppTroubleshootingAppStateHistory</span><span class="sxs-lookup"><span data-stu-id="3f031-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

<span data-ttu-id="3f031-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f031-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f031-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3f031-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f031-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3f031-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f031-107">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="3f031-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="3f031-108">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="3f031-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3f031-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f031-109">Properties</span></span>
|<span data-ttu-id="3f031-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f031-110">Property</span></span>|<span data-ttu-id="3f031-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f031-111">Type</span></span>|<span data-ttu-id="3f031-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f031-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f031-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="3f031-113">occurrenceDateTime</span></span>|<span data-ttu-id="3f031-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f031-114">DateTimeOffset</span></span>|<span data-ttu-id="3f031-115">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="3f031-115">Time when the history item occurred.</span></span> <span data-ttu-id="3f031-116">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="3f031-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="3f031-117">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3f031-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="3f031-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3f031-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="3f031-119">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="3f031-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="3f031-120">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="3f031-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="3f031-121">actionType</span><span class="sxs-lookup"><span data-stu-id="3f031-121">actionType</span></span>|[<span data-ttu-id="3f031-122">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="3f031-122">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="3f031-123">Tipo de ação para o aplicativo do Intune.</span><span class="sxs-lookup"><span data-stu-id="3f031-123">Action type for Intune Application.</span></span> <span data-ttu-id="3f031-124">Os valores possíveis são: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="3f031-124">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="3f031-125">runState</span><span class="sxs-lookup"><span data-stu-id="3f031-125">runState</span></span>|[<span data-ttu-id="3f031-126">runState</span><span class="sxs-lookup"><span data-stu-id="3f031-126">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="3f031-127">Status do item.</span><span class="sxs-lookup"><span data-stu-id="3f031-127">Status of the item.</span></span> <span data-ttu-id="3f031-128">Os valores possíveis são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="3f031-128">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="3f031-129">errorCode</span><span class="sxs-lookup"><span data-stu-id="3f031-129">errorCode</span></span>|<span data-ttu-id="3f031-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f031-130">String</span></span>|<span data-ttu-id="3f031-131">Código de erro para a falha, vazio se não houver falha.</span><span class="sxs-lookup"><span data-stu-id="3f031-131">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f031-132">Relações</span><span class="sxs-lookup"><span data-stu-id="3f031-132">Relationships</span></span>
<span data-ttu-id="3f031-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f031-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f031-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f031-134">JSON Representation</span></span>
<span data-ttu-id="3f031-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f031-135">Here is a JSON representation of the resource.</span></span>
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



