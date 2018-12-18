---
title: tipo de recurso de windows10AppsForceUpdateSchedule
description: Agendamento de atualização do Windows 10 force para aplicativos
author: tfitzmac
ms.openlocfilehash: 851f22e092f2669dfc44911783df6182cda1dc6d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323699"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="63708-103">tipo de recurso de windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="63708-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="63708-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="63708-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63708-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="63708-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63708-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="63708-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63708-107">Agendamento de atualização do Windows 10 force para aplicativos</span><span class="sxs-lookup"><span data-stu-id="63708-107">Windows 10 force update schedule for Apps</span></span>
## <a name="properties"></a><span data-ttu-id="63708-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63708-108">Properties</span></span>
|<span data-ttu-id="63708-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63708-109">Property</span></span>|<span data-ttu-id="63708-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="63708-110">Type</span></span>|<span data-ttu-id="63708-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="63708-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63708-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="63708-112">startDateTime</span></span>|<span data-ttu-id="63708-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63708-113">DateTimeOffset</span></span>|<span data-ttu-id="63708-114">A hora de início para a força reinicie.</span><span class="sxs-lookup"><span data-stu-id="63708-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="63708-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="63708-115">recurrence</span></span>|[<span data-ttu-id="63708-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="63708-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="63708-117">Plano de recorrência.</span><span class="sxs-lookup"><span data-stu-id="63708-117">Recurrence schedule.</span></span> <span data-ttu-id="63708-118">Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="63708-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="63708-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="63708-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="63708-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="63708-120">Boolean</span></span>|<span data-ttu-id="63708-121">Se for true, executa a tarefa imediatamente se StartDateTime está no passado, para outro, será executada na próxima recorrência.</span><span class="sxs-lookup"><span data-stu-id="63708-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63708-122">Relações</span><span class="sxs-lookup"><span data-stu-id="63708-122">Relationships</span></span>
<span data-ttu-id="63708-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="63708-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="63708-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63708-124">JSON Representation</span></span>
<span data-ttu-id="63708-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="63708-125">Here is a JSON representation of the resource.</span></span>
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





