---
title: tipo de recurso de mobileAppTroubleshootingAppStateHistory
description: Item de histórico contido no evento Mobile App solução de problemas.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 65ee72ed0c265f2e989e82dfdcc28d27605d4753
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885565"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="8062c-103">tipo de recurso de mobileAppTroubleshootingAppStateHistory</span><span class="sxs-lookup"><span data-stu-id="8062c-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="8062c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8062c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8062c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8062c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8062c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8062c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8062c-107">Item de histórico contido no evento Mobile App solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="8062c-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="8062c-108">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="8062c-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8062c-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8062c-109">Properties</span></span>
|<span data-ttu-id="8062c-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8062c-110">Property</span></span>|<span data-ttu-id="8062c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="8062c-111">Type</span></span>|<span data-ttu-id="8062c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8062c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8062c-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="8062c-113">occurrenceDateTime</span></span>|<span data-ttu-id="8062c-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8062c-114">DateTimeOffset</span></span>|<span data-ttu-id="8062c-115">Hora de quando o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="8062c-115">Time when the history item occurred.</span></span> <span data-ttu-id="8062c-116">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="8062c-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="8062c-117">actionType</span><span class="sxs-lookup"><span data-stu-id="8062c-117">actionType</span></span>|[<span data-ttu-id="8062c-118">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="8062c-118">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="8062c-119">Identificação de grupo de segurança AAD ao qual ele estava direcionado.</span><span class="sxs-lookup"><span data-stu-id="8062c-119">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="8062c-120">Os valores possíveis são: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="8062c-120">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="8062c-121">runState</span><span class="sxs-lookup"><span data-stu-id="8062c-121">runState</span></span>|[<span data-ttu-id="8062c-122">runState</span><span class="sxs-lookup"><span data-stu-id="8062c-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="8062c-123">Status do item.</span><span class="sxs-lookup"><span data-stu-id="8062c-123">Status of the item.</span></span> <span data-ttu-id="8062c-124">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="8062c-124">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="8062c-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="8062c-125">errorCode</span></span>|<span data-ttu-id="8062c-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8062c-126">String</span></span>|<span data-ttu-id="8062c-127">Código de erro da falha, vazia se nenhum falha.</span><span class="sxs-lookup"><span data-stu-id="8062c-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8062c-128">Relações</span><span class="sxs-lookup"><span data-stu-id="8062c-128">Relationships</span></span>
<span data-ttu-id="8062c-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8062c-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8062c-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8062c-130">JSON Representation</span></span>
<span data-ttu-id="8062c-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8062c-131">Here is a JSON representation of the resource.</span></span>
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





