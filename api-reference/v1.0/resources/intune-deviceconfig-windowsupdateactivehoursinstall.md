---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 124ac24616ee8662bd0224fd2a063e523dfdb260
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451396"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="a2cd8-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="a2cd8-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="a2cd8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2cd8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2cd8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2cd8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2cd8-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a2cd8-106">Not yet documented</span></span>


<span data-ttu-id="a2cd8-107">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="a2cd8-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a2cd8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2cd8-108">Properties</span></span>
|<span data-ttu-id="a2cd8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2cd8-109">Property</span></span>|<span data-ttu-id="a2cd8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2cd8-110">Type</span></span>|<span data-ttu-id="a2cd8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2cd8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2cd8-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="a2cd8-112">activeHoursStart</span></span>|<span data-ttu-id="a2cd8-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a2cd8-113">TimeOfDay</span></span>|<span data-ttu-id="a2cd8-114">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="a2cd8-114">Active Hours Start</span></span>|
|<span data-ttu-id="a2cd8-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="a2cd8-115">activeHoursEnd</span></span>|<span data-ttu-id="a2cd8-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a2cd8-116">TimeOfDay</span></span>|<span data-ttu-id="a2cd8-117">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="a2cd8-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2cd8-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a2cd8-118">Relationships</span></span>
<span data-ttu-id="a2cd8-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a2cd8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2cd8-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2cd8-120">JSON Representation</span></span>
<span data-ttu-id="a2cd8-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2cd8-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```







