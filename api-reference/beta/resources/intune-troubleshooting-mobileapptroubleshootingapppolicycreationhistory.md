---
title: tipo de recurso mobileAppTroubleshootingAppPolicyCreationHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e0d83f07cfa71c84cb0db99b7ea6e26822177f8f
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159077"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="9fc23-103">tipo de recurso mobileAppTroubleshootingAppPolicyCreationHistory</span><span class="sxs-lookup"><span data-stu-id="9fc23-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="9fc23-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9fc23-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fc23-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9fc23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fc23-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="9fc23-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="9fc23-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="9fc23-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9fc23-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9fc23-108">Properties</span></span>
|<span data-ttu-id="9fc23-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fc23-109">Property</span></span>|<span data-ttu-id="9fc23-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fc23-110">Type</span></span>|<span data-ttu-id="9fc23-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fc23-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fc23-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="9fc23-112">occurrenceDateTime</span></span>|<span data-ttu-id="9fc23-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fc23-113">DateTimeOffset</span></span>|<span data-ttu-id="9fc23-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="9fc23-114">Time when the history item occurred.</span></span> <span data-ttu-id="9fc23-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="9fc23-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="9fc23-116">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="9fc23-116">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="9fc23-117">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="9fc23-117">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="9fc23-118">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="9fc23-118">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="9fc23-119">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="9fc23-119">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="9fc23-120">runState</span><span class="sxs-lookup"><span data-stu-id="9fc23-120">runState</span></span>|[<span data-ttu-id="9fc23-121">runState</span><span class="sxs-lookup"><span data-stu-id="9fc23-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="9fc23-122">Status do item.</span><span class="sxs-lookup"><span data-stu-id="9fc23-122">Status of the item.</span></span> <span data-ttu-id="9fc23-123">Os valores possíveis são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="9fc23-123">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="9fc23-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="9fc23-124">errorCode</span></span>|<span data-ttu-id="9fc23-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9fc23-125">String</span></span>|<span data-ttu-id="9fc23-126">Código de erro para a falha, vazio se não houver falha.</span><span class="sxs-lookup"><span data-stu-id="9fc23-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fc23-127">Relações</span><span class="sxs-lookup"><span data-stu-id="9fc23-127">Relationships</span></span>
<span data-ttu-id="9fc23-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9fc23-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fc23-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9fc23-129">JSON Representation</span></span>
<span data-ttu-id="9fc23-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9fc23-130">Here is a JSON representation of the resource.</span></span>
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



