---
title: tipo de recurso de windows10AppsForceUpdateSchedule
description: Agendamento de atualização do Windows 10 force para aplicativos
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e0bd9b0963f8547b03243aa7ef791a351dc2b08
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418831"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="ac1d2-103">tipo de recurso de windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="ac1d2-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="ac1d2-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ac1d2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ac1d2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ac1d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ac1d2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ac1d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac1d2-107">Agendamento de atualização do Windows 10 force para aplicativos</span><span class="sxs-lookup"><span data-stu-id="ac1d2-107">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="ac1d2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac1d2-108">Properties</span></span>
|<span data-ttu-id="ac1d2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac1d2-109">Property</span></span>|<span data-ttu-id="ac1d2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac1d2-110">Type</span></span>|<span data-ttu-id="ac1d2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac1d2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac1d2-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ac1d2-112">startDateTime</span></span>|<span data-ttu-id="ac1d2-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac1d2-113">DateTimeOffset</span></span>|<span data-ttu-id="ac1d2-114">A hora de início para a força reinicie.</span><span class="sxs-lookup"><span data-stu-id="ac1d2-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="ac1d2-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="ac1d2-115">recurrence</span></span>|[<span data-ttu-id="ac1d2-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="ac1d2-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="ac1d2-117">Plano de recorrência.</span><span class="sxs-lookup"><span data-stu-id="ac1d2-117">Recurrence schedule.</span></span> <span data-ttu-id="ac1d2-118">Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="ac1d2-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="ac1d2-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="ac1d2-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="ac1d2-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac1d2-120">Boolean</span></span>|<span data-ttu-id="ac1d2-121">Se for true, executa a tarefa imediatamente se StartDateTime está no passado, para outro, será executada na próxima recorrência.</span><span class="sxs-lookup"><span data-stu-id="ac1d2-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac1d2-122">Relações</span><span class="sxs-lookup"><span data-stu-id="ac1d2-122">Relationships</span></span>
<span data-ttu-id="ac1d2-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac1d2-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac1d2-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac1d2-124">JSON Representation</span></span>
<span data-ttu-id="ac1d2-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac1d2-125">Here is a JSON representation of the resource.</span></span>
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




