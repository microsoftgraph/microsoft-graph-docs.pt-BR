---
title: tipo de recurso mobileAppTroubleshootingAppTargetHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da07e7873243c4c626d615ac91bda8f8e33b0b0c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42764450"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="e8a83-103">tipo de recurso mobileAppTroubleshootingAppTargetHistory</span><span class="sxs-lookup"><span data-stu-id="e8a83-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="e8a83-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8a83-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8a83-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8a83-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8a83-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e8a83-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="e8a83-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e8a83-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e8a83-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8a83-108">Properties</span></span>
|<span data-ttu-id="e8a83-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8a83-109">Property</span></span>|<span data-ttu-id="e8a83-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8a83-110">Type</span></span>|<span data-ttu-id="e8a83-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8a83-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8a83-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="e8a83-112">occurrenceDateTime</span></span>|<span data-ttu-id="e8a83-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8a83-113">DateTimeOffset</span></span>|<span data-ttu-id="e8a83-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="e8a83-114">Time when the history item occurred.</span></span> <span data-ttu-id="e8a83-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e8a83-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="e8a83-116">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e8a83-116">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="e8a83-117">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e8a83-117">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="e8a83-118">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="e8a83-118">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="e8a83-119">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e8a83-119">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="e8a83-120">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="e8a83-120">securityGroupId</span></span>|<span data-ttu-id="e8a83-121">String</span><span class="sxs-lookup"><span data-stu-id="e8a83-121">String</span></span>|<span data-ttu-id="e8a83-122">ID do grupo de segurança do AAD para o qual foi direcionado.</span><span class="sxs-lookup"><span data-stu-id="e8a83-122">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="e8a83-123">runState</span><span class="sxs-lookup"><span data-stu-id="e8a83-123">runState</span></span>|[<span data-ttu-id="e8a83-124">runState</span><span class="sxs-lookup"><span data-stu-id="e8a83-124">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="e8a83-125">Status do item.</span><span class="sxs-lookup"><span data-stu-id="e8a83-125">Status of the item.</span></span> <span data-ttu-id="e8a83-126">Os valores possíveis são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="e8a83-126">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="e8a83-127">errorCode</span><span class="sxs-lookup"><span data-stu-id="e8a83-127">errorCode</span></span>|<span data-ttu-id="e8a83-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8a83-128">String</span></span>|<span data-ttu-id="e8a83-129">Código de erro para a falha, vazio se não houver falha.</span><span class="sxs-lookup"><span data-stu-id="e8a83-129">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8a83-130">Relações</span><span class="sxs-lookup"><span data-stu-id="e8a83-130">Relationships</span></span>
<span data-ttu-id="e8a83-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e8a83-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8a83-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8a83-132">JSON Representation</span></span>
<span data-ttu-id="e8a83-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8a83-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppTargetHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppTargetHistory",
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
  "securityGroupId": "String",
  "runState": "String",
  "errorCode": "String"
}
```



