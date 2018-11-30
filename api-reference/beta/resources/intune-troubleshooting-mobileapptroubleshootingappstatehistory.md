---
title: tipo de recurso de mobileAppTroubleshootingAppStateHistory
description: Item de histórico contido no evento Mobile App solução de problemas.
ms.openlocfilehash: 415d018d3650819bce8defe651af8df77e3c6032
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035510"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="2cc47-103">tipo de recurso de mobileAppTroubleshootingAppStateHistory</span><span class="sxs-lookup"><span data-stu-id="2cc47-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="2cc47-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2cc47-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2cc47-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2cc47-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2cc47-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2cc47-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2cc47-107">Item de histórico contido no evento Mobile App solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="2cc47-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="2cc47-108">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="2cc47-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2cc47-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2cc47-109">Properties</span></span>
|<span data-ttu-id="2cc47-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2cc47-110">Property</span></span>|<span data-ttu-id="2cc47-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cc47-111">Type</span></span>|<span data-ttu-id="2cc47-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cc47-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cc47-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="2cc47-113">occurrenceDateTime</span></span>|<span data-ttu-id="2cc47-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cc47-114">DateTimeOffset</span></span>|<span data-ttu-id="2cc47-115">Hora de quando o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="2cc47-115">Time when the history item occurred.</span></span> <span data-ttu-id="2cc47-116">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="2cc47-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="2cc47-117">actionType</span><span class="sxs-lookup"><span data-stu-id="2cc47-117">actionType</span></span>|[<span data-ttu-id="2cc47-118">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="2cc47-118">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="2cc47-119">Identificação de grupo de segurança AAD ao qual ele estava direcionado.</span><span class="sxs-lookup"><span data-stu-id="2cc47-119">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="2cc47-120">Os valores possíveis são: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="2cc47-120">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="2cc47-121">runState</span><span class="sxs-lookup"><span data-stu-id="2cc47-121">runState</span></span>|[<span data-ttu-id="2cc47-122">runState</span><span class="sxs-lookup"><span data-stu-id="2cc47-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="2cc47-123">Status do item.</span><span class="sxs-lookup"><span data-stu-id="2cc47-123">Status of the item.</span></span> <span data-ttu-id="2cc47-124">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="2cc47-124">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="2cc47-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="2cc47-125">errorCode</span></span>|<span data-ttu-id="2cc47-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2cc47-126">String</span></span>|<span data-ttu-id="2cc47-127">Código de erro da falha, vazia se nenhum falha.</span><span class="sxs-lookup"><span data-stu-id="2cc47-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cc47-128">Relações</span><span class="sxs-lookup"><span data-stu-id="2cc47-128">Relationships</span></span>
<span data-ttu-id="2cc47-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2cc47-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2cc47-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2cc47-130">JSON Representation</span></span>
<span data-ttu-id="2cc47-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2cc47-131">Here is a JSON representation of the resource.</span></span>
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





