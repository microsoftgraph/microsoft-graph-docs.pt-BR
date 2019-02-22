---
title: tipo de recurso windows10AppsForceUpdateSchedule
description: Agendamento de atualização forçada do Windows 10 para aplicativos
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7aa5573c3d644299b9c0aa424f348a67db8379d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158223"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="a9c5b-103">tipo de recurso windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="a9c5b-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="a9c5b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a9c5b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9c5b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9c5b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9c5b-106">Agendamento de atualização forçada do Windows 10 para aplicativos</span><span class="sxs-lookup"><span data-stu-id="a9c5b-106">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="a9c5b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9c5b-107">Properties</span></span>
|<span data-ttu-id="a9c5b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9c5b-108">Property</span></span>|<span data-ttu-id="a9c5b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9c5b-109">Type</span></span>|<span data-ttu-id="a9c5b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9c5b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9c5b-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a9c5b-111">startDateTime</span></span>|<span data-ttu-id="a9c5b-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9c5b-112">DateTimeOffset</span></span>|<span data-ttu-id="a9c5b-113">A hora de início da reinicialização forçada.</span><span class="sxs-lookup"><span data-stu-id="a9c5b-113">The start time for the force restart.</span></span>|
|<span data-ttu-id="a9c5b-114">recurrence</span><span class="sxs-lookup"><span data-stu-id="a9c5b-114">recurrence</span></span>|[<span data-ttu-id="a9c5b-115">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="a9c5b-115">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="a9c5b-116">Agenda de reCorrência.</span><span class="sxs-lookup"><span data-stu-id="a9c5b-116">Recurrence schedule.</span></span> <span data-ttu-id="a9c5b-117">Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="a9c5b-117">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="a9c5b-118">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="a9c5b-118">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="a9c5b-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="a9c5b-119">Boolean</span></span>|<span data-ttu-id="a9c5b-120">Se true, executará a tarefa imediatamente se StartDatetime estiver no passado, senão, será executado na próxima recorrência.</span><span class="sxs-lookup"><span data-stu-id="a9c5b-120">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9c5b-121">Relações</span><span class="sxs-lookup"><span data-stu-id="a9c5b-121">Relationships</span></span>
<span data-ttu-id="a9c5b-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a9c5b-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9c5b-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9c5b-123">JSON Representation</span></span>
<span data-ttu-id="a9c5b-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a9c5b-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AppsForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "runImmediatelyIfAfterStartDateTime": true
}
```




