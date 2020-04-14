---
title: tipo de recurso windows10AppsForceUpdateSchedule
description: Agendamento de atualização forçada do Windows 10 para aplicativos
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eb590d65a6ae60eeede42b3ce6b5d422f306b8c8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466309"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="cd147-103">tipo de recurso windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="cd147-103">windows10AppsForceUpdateSchedule resource type</span></span>

<span data-ttu-id="cd147-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd147-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd147-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cd147-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd147-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cd147-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd147-107">Agendamento de atualização forçada do Windows 10 para aplicativos</span><span class="sxs-lookup"><span data-stu-id="cd147-107">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="cd147-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd147-108">Properties</span></span>
|<span data-ttu-id="cd147-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd147-109">Property</span></span>|<span data-ttu-id="cd147-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd147-110">Type</span></span>|<span data-ttu-id="cd147-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd147-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd147-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cd147-112">startDateTime</span></span>|<span data-ttu-id="cd147-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd147-113">DateTimeOffset</span></span>|<span data-ttu-id="cd147-114">A hora de início da reinicialização forçada.</span><span class="sxs-lookup"><span data-stu-id="cd147-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="cd147-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="cd147-115">recurrence</span></span>|[<span data-ttu-id="cd147-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="cd147-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="cd147-117">Agenda de recorrência.</span><span class="sxs-lookup"><span data-stu-id="cd147-117">Recurrence schedule.</span></span> <span data-ttu-id="cd147-118">Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="cd147-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="cd147-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="cd147-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="cd147-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="cd147-120">Boolean</span></span>|<span data-ttu-id="cd147-121">Se true, executará a tarefa imediatamente se StartDatetime estiver no passado, senão, será executado na próxima recorrência.</span><span class="sxs-lookup"><span data-stu-id="cd147-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd147-122">Relações</span><span class="sxs-lookup"><span data-stu-id="cd147-122">Relationships</span></span>
<span data-ttu-id="cd147-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cd147-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd147-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd147-124">JSON Representation</span></span>
<span data-ttu-id="cd147-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd147-125">Here is a JSON representation of the resource.</span></span>
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



