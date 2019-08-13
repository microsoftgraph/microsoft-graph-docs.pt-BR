---
title: tipo de recurso mobileAppTroubleshootingAppStateHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 62c57d4ed01ab1f454a5356899f9645927680dfd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313045"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="438e6-103">tipo de recurso mobileAppTroubleshootingAppStateHistory</span><span class="sxs-lookup"><span data-stu-id="438e6-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="438e6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="438e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="438e6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="438e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="438e6-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="438e6-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="438e6-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="438e6-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="438e6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="438e6-108">Properties</span></span>
|<span data-ttu-id="438e6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="438e6-109">Property</span></span>|<span data-ttu-id="438e6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="438e6-110">Type</span></span>|<span data-ttu-id="438e6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="438e6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="438e6-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="438e6-112">occurrenceDateTime</span></span>|<span data-ttu-id="438e6-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="438e6-113">DateTimeOffset</span></span>|<span data-ttu-id="438e6-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="438e6-114">Time when the history item occurred.</span></span> <span data-ttu-id="438e6-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="438e6-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="438e6-116">actionType</span><span class="sxs-lookup"><span data-stu-id="438e6-116">actionType</span></span>|[<span data-ttu-id="438e6-117">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="438e6-117">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="438e6-118">ID do grupo de segurança do AAD para o qual foi direcionado.</span><span class="sxs-lookup"><span data-stu-id="438e6-118">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="438e6-119">Os valores possíveis são: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="438e6-119">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="438e6-120">runState</span><span class="sxs-lookup"><span data-stu-id="438e6-120">runState</span></span>|[<span data-ttu-id="438e6-121">runState</span><span class="sxs-lookup"><span data-stu-id="438e6-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="438e6-122">Status do item.</span><span class="sxs-lookup"><span data-stu-id="438e6-122">Status of the item.</span></span> <span data-ttu-id="438e6-123">Os valores possíveis são: `unknown`, `success`, `fail`, `error`, `pending`.</span><span class="sxs-lookup"><span data-stu-id="438e6-123">Possible values are: `unknown`, `success`, `fail`, `error`, `pending`.</span></span>|
|<span data-ttu-id="438e6-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="438e6-124">errorCode</span></span>|<span data-ttu-id="438e6-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="438e6-125">String</span></span>|<span data-ttu-id="438e6-126">Código de erro para a falha, vazio se não houver falha.</span><span class="sxs-lookup"><span data-stu-id="438e6-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="438e6-127">Relações</span><span class="sxs-lookup"><span data-stu-id="438e6-127">Relationships</span></span>
<span data-ttu-id="438e6-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="438e6-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="438e6-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="438e6-129">JSON Representation</span></span>
<span data-ttu-id="438e6-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="438e6-130">Here is a JSON representation of the resource.</span></span>
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



