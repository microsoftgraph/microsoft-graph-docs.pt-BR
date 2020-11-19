---
title: tipo de recurso windows10AppsForceUpdateSchedule
description: Agendamento de atualização forçada do Windows 10 para aplicativos
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20ea28b176f05bb1e6d2e2579715ebe5bdd500a2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273029"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="9577f-103">tipo de recurso windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="9577f-103">windows10AppsForceUpdateSchedule resource type</span></span>

<span data-ttu-id="9577f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9577f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9577f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9577f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9577f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9577f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9577f-107">Agendamento de atualização forçada do Windows 10 para aplicativos</span><span class="sxs-lookup"><span data-stu-id="9577f-107">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="9577f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9577f-108">Properties</span></span>
|<span data-ttu-id="9577f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9577f-109">Property</span></span>|<span data-ttu-id="9577f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9577f-110">Type</span></span>|<span data-ttu-id="9577f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9577f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9577f-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9577f-112">startDateTime</span></span>|<span data-ttu-id="9577f-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9577f-113">DateTimeOffset</span></span>|<span data-ttu-id="9577f-114">A hora de início da reinicialização forçada.</span><span class="sxs-lookup"><span data-stu-id="9577f-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="9577f-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="9577f-115">recurrence</span></span>|[<span data-ttu-id="9577f-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="9577f-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="9577f-117">Agenda de recorrência.</span><span class="sxs-lookup"><span data-stu-id="9577f-117">Recurrence schedule.</span></span> <span data-ttu-id="9577f-118">Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="9577f-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="9577f-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="9577f-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="9577f-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="9577f-120">Boolean</span></span>|<span data-ttu-id="9577f-121">Se true, executará a tarefa imediatamente se StartDatetime estiver no passado, senão, será executado na próxima recorrência.</span><span class="sxs-lookup"><span data-stu-id="9577f-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9577f-122">Relações</span><span class="sxs-lookup"><span data-stu-id="9577f-122">Relationships</span></span>
<span data-ttu-id="9577f-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9577f-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9577f-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9577f-124">JSON Representation</span></span>
<span data-ttu-id="9577f-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9577f-125">Here is a JSON representation of the resource.</span></span>
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




