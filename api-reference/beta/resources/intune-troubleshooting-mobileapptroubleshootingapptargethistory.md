---
title: tipo de recurso mobileAppTroubleshootingAppTargetHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d53c03b508dc0298c9ed928acc406cdc63e08781
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159049"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="9f008-103">tipo de recurso mobileAppTroubleshootingAppTargetHistory</span><span class="sxs-lookup"><span data-stu-id="9f008-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="9f008-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9f008-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f008-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9f008-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f008-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="9f008-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="9f008-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="9f008-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9f008-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f008-108">Properties</span></span>
|<span data-ttu-id="9f008-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f008-109">Property</span></span>|<span data-ttu-id="9f008-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f008-110">Type</span></span>|<span data-ttu-id="9f008-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f008-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f008-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="9f008-112">occurrenceDateTime</span></span>|<span data-ttu-id="9f008-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f008-113">DateTimeOffset</span></span>|<span data-ttu-id="9f008-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="9f008-114">Time when the history item occurred.</span></span> <span data-ttu-id="9f008-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="9f008-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="9f008-116">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="9f008-116">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="9f008-117">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="9f008-117">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="9f008-118">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="9f008-118">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="9f008-119">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="9f008-119">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="9f008-120">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="9f008-120">securityGroupId</span></span>|<span data-ttu-id="9f008-121">String</span><span class="sxs-lookup"><span data-stu-id="9f008-121">String</span></span>|<span data-ttu-id="9f008-122">ID do grupo de segurança do AAD para o qual foi direcionado.</span><span class="sxs-lookup"><span data-stu-id="9f008-122">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="9f008-123">runState</span><span class="sxs-lookup"><span data-stu-id="9f008-123">runState</span></span>|[<span data-ttu-id="9f008-124">runState</span><span class="sxs-lookup"><span data-stu-id="9f008-124">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="9f008-125">Status do item.</span><span class="sxs-lookup"><span data-stu-id="9f008-125">Status of the item.</span></span> <span data-ttu-id="9f008-126">Os valores possíveis são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="9f008-126">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="9f008-127">errorCode</span><span class="sxs-lookup"><span data-stu-id="9f008-127">errorCode</span></span>|<span data-ttu-id="9f008-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f008-128">String</span></span>|<span data-ttu-id="9f008-129">Código de erro para a falha, vazio se não houver falha.</span><span class="sxs-lookup"><span data-stu-id="9f008-129">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f008-130">Relações</span><span class="sxs-lookup"><span data-stu-id="9f008-130">Relationships</span></span>
<span data-ttu-id="9f008-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f008-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f008-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f008-132">JSON Representation</span></span>
<span data-ttu-id="9f008-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f008-133">Here is a JSON representation of the resource.</span></span>
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



