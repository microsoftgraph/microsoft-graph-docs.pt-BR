---
title: tipo de recurso mobileAppTroubleshootingAppStateHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c3f3b466d234c1f49a44cab8170366d8203bd26
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988080"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="7b4d5-103">tipo de recurso mobileAppTroubleshootingAppStateHistory</span><span class="sxs-lookup"><span data-stu-id="7b4d5-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="7b4d5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b4d5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b4d5-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="7b4d5-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="7b4d5-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7b4d5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b4d5-108">Properties</span></span>
|<span data-ttu-id="7b4d5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b4d5-109">Property</span></span>|<span data-ttu-id="7b4d5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b4d5-110">Type</span></span>|<span data-ttu-id="7b4d5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b4d5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b4d5-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="7b4d5-112">occurrenceDateTime</span></span>|<span data-ttu-id="7b4d5-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b4d5-113">DateTimeOffset</span></span>|<span data-ttu-id="7b4d5-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-114">Time when the history item occurred.</span></span> <span data-ttu-id="7b4d5-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="7b4d5-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="7b4d5-116">actionType</span><span class="sxs-lookup"><span data-stu-id="7b4d5-116">actionType</span></span>|[<span data-ttu-id="7b4d5-117">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="7b4d5-117">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="7b4d5-118">ID do grupo de segurança do AAD para o qual foi direcionado.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-118">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="7b4d5-119">Os valores possíveis são: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-119">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="7b4d5-120">runState</span><span class="sxs-lookup"><span data-stu-id="7b4d5-120">runState</span></span>|[<span data-ttu-id="7b4d5-121">runState</span><span class="sxs-lookup"><span data-stu-id="7b4d5-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="7b4d5-122">Status do item.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-122">Status of the item.</span></span> <span data-ttu-id="7b4d5-123">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="7b4d5-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="7b4d5-124">errorCode</span></span>|<span data-ttu-id="7b4d5-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7b4d5-125">String</span></span>|<span data-ttu-id="7b4d5-126">Código de erro para a falha, vazio se não houver falha.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b4d5-127">Relações</span><span class="sxs-lookup"><span data-stu-id="7b4d5-127">Relationships</span></span>
<span data-ttu-id="7b4d5-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b4d5-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b4d5-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b4d5-129">JSON Representation</span></span>
<span data-ttu-id="7b4d5-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-130">Here is a JSON representation of the resource.</span></span>
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





