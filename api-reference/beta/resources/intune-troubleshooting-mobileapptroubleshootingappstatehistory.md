---
title: tipo de recurso de mobileAppTroubleshootingAppStateHistory
description: Item de histórico contido no evento Mobile App solução de problemas.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 57e10fcabc0aa3def07872c0e520f09c6ee90fc3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411236"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="25026-103">tipo de recurso de mobileAppTroubleshootingAppStateHistory</span><span class="sxs-lookup"><span data-stu-id="25026-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="25026-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="25026-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="25026-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="25026-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="25026-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="25026-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25026-107">Item de histórico contido no evento Mobile App solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="25026-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="25026-108">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="25026-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="25026-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25026-109">Properties</span></span>
|<span data-ttu-id="25026-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25026-110">Property</span></span>|<span data-ttu-id="25026-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="25026-111">Type</span></span>|<span data-ttu-id="25026-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="25026-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25026-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="25026-113">occurrenceDateTime</span></span>|<span data-ttu-id="25026-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25026-114">DateTimeOffset</span></span>|<span data-ttu-id="25026-115">Hora de quando o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="25026-115">Time when the history item occurred.</span></span> <span data-ttu-id="25026-116">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="25026-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="25026-117">actionType</span><span class="sxs-lookup"><span data-stu-id="25026-117">actionType</span></span>|[<span data-ttu-id="25026-118">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="25026-118">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="25026-119">Identificação de grupo de segurança AAD ao qual ele estava direcionado.</span><span class="sxs-lookup"><span data-stu-id="25026-119">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="25026-120">Os valores possíveis são: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="25026-120">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="25026-121">runState</span><span class="sxs-lookup"><span data-stu-id="25026-121">runState</span></span>|[<span data-ttu-id="25026-122">runState</span><span class="sxs-lookup"><span data-stu-id="25026-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="25026-123">Status do item.</span><span class="sxs-lookup"><span data-stu-id="25026-123">Status of the item.</span></span> <span data-ttu-id="25026-124">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="25026-124">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="25026-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="25026-125">errorCode</span></span>|<span data-ttu-id="25026-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25026-126">String</span></span>|<span data-ttu-id="25026-127">Código de erro da falha, vazia se nenhum falha.</span><span class="sxs-lookup"><span data-stu-id="25026-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25026-128">Relações</span><span class="sxs-lookup"><span data-stu-id="25026-128">Relationships</span></span>
<span data-ttu-id="25026-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25026-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="25026-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25026-130">JSON Representation</span></span>
<span data-ttu-id="25026-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25026-131">Here is a JSON representation of the resource.</span></span>
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




