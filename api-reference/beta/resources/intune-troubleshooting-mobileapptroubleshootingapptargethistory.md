---
title: tipo de recurso mobileAppTroubleshootingAppTargetHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 52fc89c4c3b9b77be30cf3cc8c651bde7e696bf2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003504"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="32674-103">tipo de recurso mobileAppTroubleshootingAppTargetHistory</span><span class="sxs-lookup"><span data-stu-id="32674-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

<span data-ttu-id="32674-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="32674-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32674-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="32674-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32674-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="32674-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32674-107">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="32674-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="32674-108">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="32674-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="32674-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32674-109">Properties</span></span>
|<span data-ttu-id="32674-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32674-110">Property</span></span>|<span data-ttu-id="32674-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="32674-111">Type</span></span>|<span data-ttu-id="32674-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="32674-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32674-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="32674-113">occurrenceDateTime</span></span>|<span data-ttu-id="32674-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32674-114">DateTimeOffset</span></span>|<span data-ttu-id="32674-115">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="32674-115">Time when the history item occurred.</span></span> <span data-ttu-id="32674-116">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="32674-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="32674-117">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="32674-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="32674-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="32674-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="32674-119">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="32674-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="32674-120">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="32674-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="32674-121">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="32674-121">securityGroupId</span></span>|<span data-ttu-id="32674-122">String</span><span class="sxs-lookup"><span data-stu-id="32674-122">String</span></span>|<span data-ttu-id="32674-123">ID do grupo de segurança do AAD para o qual foi direcionado.</span><span class="sxs-lookup"><span data-stu-id="32674-123">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="32674-124">runState</span><span class="sxs-lookup"><span data-stu-id="32674-124">runState</span></span>|[<span data-ttu-id="32674-125">runState</span><span class="sxs-lookup"><span data-stu-id="32674-125">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="32674-126">Status do item.</span><span class="sxs-lookup"><span data-stu-id="32674-126">Status of the item.</span></span> <span data-ttu-id="32674-127">Os valores possíveis são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="32674-127">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="32674-128">errorCode</span><span class="sxs-lookup"><span data-stu-id="32674-128">errorCode</span></span>|<span data-ttu-id="32674-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32674-129">String</span></span>|<span data-ttu-id="32674-130">Código de erro para a falha, vazio se não houver falha.</span><span class="sxs-lookup"><span data-stu-id="32674-130">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32674-131">Relações</span><span class="sxs-lookup"><span data-stu-id="32674-131">Relationships</span></span>
<span data-ttu-id="32674-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="32674-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32674-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32674-133">JSON Representation</span></span>
<span data-ttu-id="32674-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32674-134">Here is a JSON representation of the resource.</span></span>
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






