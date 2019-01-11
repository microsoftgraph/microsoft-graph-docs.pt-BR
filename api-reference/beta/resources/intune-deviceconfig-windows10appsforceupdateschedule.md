---
title: tipo de recurso de windows10AppsForceUpdateSchedule
description: Agendamento de atualização do Windows 10 force para aplicativos
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ef8a0583bd02a62a4461a3415aae86833e24e948
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811231"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="9b5af-103">tipo de recurso de windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="9b5af-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="9b5af-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9b5af-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b5af-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9b5af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b5af-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9b5af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b5af-107">Agendamento de atualização do Windows 10 force para aplicativos</span><span class="sxs-lookup"><span data-stu-id="9b5af-107">Windows 10 force update schedule for Apps</span></span>
## <a name="properties"></a><span data-ttu-id="9b5af-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b5af-108">Properties</span></span>
|<span data-ttu-id="9b5af-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b5af-109">Property</span></span>|<span data-ttu-id="9b5af-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b5af-110">Type</span></span>|<span data-ttu-id="9b5af-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b5af-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b5af-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9b5af-112">startDateTime</span></span>|<span data-ttu-id="9b5af-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b5af-113">DateTimeOffset</span></span>|<span data-ttu-id="9b5af-114">A hora de início para a força reinicie.</span><span class="sxs-lookup"><span data-stu-id="9b5af-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="9b5af-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="9b5af-115">recurrence</span></span>|[<span data-ttu-id="9b5af-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="9b5af-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="9b5af-117">Plano de recorrência.</span><span class="sxs-lookup"><span data-stu-id="9b5af-117">Recurrence schedule.</span></span> <span data-ttu-id="9b5af-118">Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="9b5af-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="9b5af-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="9b5af-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="9b5af-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="9b5af-120">Boolean</span></span>|<span data-ttu-id="9b5af-121">Se for true, executa a tarefa imediatamente se StartDateTime está no passado, para outro, será executada na próxima recorrência.</span><span class="sxs-lookup"><span data-stu-id="9b5af-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b5af-122">Relações</span><span class="sxs-lookup"><span data-stu-id="9b5af-122">Relationships</span></span>
<span data-ttu-id="9b5af-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9b5af-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9b5af-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b5af-124">JSON Representation</span></span>
<span data-ttu-id="9b5af-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b5af-125">Here is a JSON representation of the resource.</span></span>
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





