---
title: tipo de recurso mobileAppTroubleshootingAppPolicyCreationHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 858beb604d8f677142685f85f41c05ecaa6dc2ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003532"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="1e86e-103">tipo de recurso mobileAppTroubleshootingAppPolicyCreationHistory</span><span class="sxs-lookup"><span data-stu-id="1e86e-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

<span data-ttu-id="1e86e-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1e86e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e86e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e86e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e86e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e86e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e86e-107">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="1e86e-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="1e86e-108">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="1e86e-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1e86e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e86e-109">Properties</span></span>
|<span data-ttu-id="1e86e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e86e-110">Property</span></span>|<span data-ttu-id="1e86e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e86e-111">Type</span></span>|<span data-ttu-id="1e86e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e86e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e86e-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="1e86e-113">occurrenceDateTime</span></span>|<span data-ttu-id="1e86e-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e86e-114">DateTimeOffset</span></span>|<span data-ttu-id="1e86e-115">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="1e86e-115">Time when the history item occurred.</span></span> <span data-ttu-id="1e86e-116">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="1e86e-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="1e86e-117">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="1e86e-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="1e86e-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="1e86e-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="1e86e-119">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="1e86e-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="1e86e-120">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="1e86e-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="1e86e-121">runState</span><span class="sxs-lookup"><span data-stu-id="1e86e-121">runState</span></span>|[<span data-ttu-id="1e86e-122">runState</span><span class="sxs-lookup"><span data-stu-id="1e86e-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="1e86e-123">Status do item.</span><span class="sxs-lookup"><span data-stu-id="1e86e-123">Status of the item.</span></span> <span data-ttu-id="1e86e-124">Os valores possíveis são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="1e86e-124">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="1e86e-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="1e86e-125">errorCode</span></span>|<span data-ttu-id="1e86e-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e86e-126">String</span></span>|<span data-ttu-id="1e86e-127">Código de erro para a falha, vazio se não houver falha.</span><span class="sxs-lookup"><span data-stu-id="1e86e-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e86e-128">Relações</span><span class="sxs-lookup"><span data-stu-id="1e86e-128">Relationships</span></span>
<span data-ttu-id="1e86e-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1e86e-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e86e-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e86e-130">JSON Representation</span></span>
<span data-ttu-id="1e86e-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e86e-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory",
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
  "runState": "String",
  "errorCode": "String"
}
```






