---
title: tipo de recurso mobileAppTroubleshootingAppTargetHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f19de8f81bafa88af2b654860942b001e73b6cfc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43385264"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="aab79-103">tipo de recurso mobileAppTroubleshootingAppTargetHistory</span><span class="sxs-lookup"><span data-stu-id="aab79-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

<span data-ttu-id="aab79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aab79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aab79-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aab79-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aab79-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aab79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aab79-107">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="aab79-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="aab79-108">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="aab79-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aab79-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aab79-109">Properties</span></span>
|<span data-ttu-id="aab79-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aab79-110">Property</span></span>|<span data-ttu-id="aab79-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="aab79-111">Type</span></span>|<span data-ttu-id="aab79-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="aab79-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aab79-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="aab79-113">occurrenceDateTime</span></span>|<span data-ttu-id="aab79-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aab79-114">DateTimeOffset</span></span>|<span data-ttu-id="aab79-115">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="aab79-115">Time when the history item occurred.</span></span> <span data-ttu-id="aab79-116">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="aab79-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="aab79-117">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="aab79-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="aab79-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="aab79-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="aab79-119">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="aab79-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="aab79-120">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="aab79-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="aab79-121">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="aab79-121">securityGroupId</span></span>|<span data-ttu-id="aab79-122">String</span><span class="sxs-lookup"><span data-stu-id="aab79-122">String</span></span>|<span data-ttu-id="aab79-123">ID do grupo de segurança do AAD para o qual foi direcionado.</span><span class="sxs-lookup"><span data-stu-id="aab79-123">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="aab79-124">runState</span><span class="sxs-lookup"><span data-stu-id="aab79-124">runState</span></span>|[<span data-ttu-id="aab79-125">runState</span><span class="sxs-lookup"><span data-stu-id="aab79-125">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="aab79-126">Status do item.</span><span class="sxs-lookup"><span data-stu-id="aab79-126">Status of the item.</span></span> <span data-ttu-id="aab79-127">Os valores possíveis são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="aab79-127">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="aab79-128">errorCode</span><span class="sxs-lookup"><span data-stu-id="aab79-128">errorCode</span></span>|<span data-ttu-id="aab79-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aab79-129">String</span></span>|<span data-ttu-id="aab79-130">Código de erro para a falha, vazio se não houver falha.</span><span class="sxs-lookup"><span data-stu-id="aab79-130">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aab79-131">Relações</span><span class="sxs-lookup"><span data-stu-id="aab79-131">Relationships</span></span>
<span data-ttu-id="aab79-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aab79-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aab79-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aab79-133">JSON Representation</span></span>
<span data-ttu-id="aab79-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aab79-134">Here is a JSON representation of the resource.</span></span>
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



