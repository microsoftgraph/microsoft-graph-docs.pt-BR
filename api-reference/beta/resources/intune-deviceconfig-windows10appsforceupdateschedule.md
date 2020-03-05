---
title: tipo de recurso windows10AppsForceUpdateSchedule
description: Agendamento de atualização forçada do Windows 10 para aplicativos
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f5c1e1c832e961b00161ef0a3d98cd8c278dc97e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529239"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="55944-103">tipo de recurso windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="55944-103">windows10AppsForceUpdateSchedule resource type</span></span>

<span data-ttu-id="55944-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="55944-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55944-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="55944-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55944-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55944-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55944-107">Agendamento de atualização forçada do Windows 10 para aplicativos</span><span class="sxs-lookup"><span data-stu-id="55944-107">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="55944-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55944-108">Properties</span></span>
|<span data-ttu-id="55944-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55944-109">Property</span></span>|<span data-ttu-id="55944-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="55944-110">Type</span></span>|<span data-ttu-id="55944-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="55944-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55944-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="55944-112">startDateTime</span></span>|<span data-ttu-id="55944-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55944-113">DateTimeOffset</span></span>|<span data-ttu-id="55944-114">A hora de início da reinicialização forçada.</span><span class="sxs-lookup"><span data-stu-id="55944-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="55944-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="55944-115">recurrence</span></span>|[<span data-ttu-id="55944-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="55944-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="55944-117">Agenda de recorrência.</span><span class="sxs-lookup"><span data-stu-id="55944-117">Recurrence schedule.</span></span> <span data-ttu-id="55944-118">Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="55944-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="55944-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="55944-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="55944-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="55944-120">Boolean</span></span>|<span data-ttu-id="55944-121">Se true, executará a tarefa imediatamente se StartDatetime estiver no passado, senão, será executado na próxima recorrência.</span><span class="sxs-lookup"><span data-stu-id="55944-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55944-122">Relações</span><span class="sxs-lookup"><span data-stu-id="55944-122">Relationships</span></span>
<span data-ttu-id="55944-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55944-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55944-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55944-124">JSON Representation</span></span>
<span data-ttu-id="55944-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55944-125">Here is a JSON representation of the resource.</span></span>
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



