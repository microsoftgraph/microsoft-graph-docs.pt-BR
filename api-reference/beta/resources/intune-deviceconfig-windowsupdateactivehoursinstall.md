---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5e9b8f4f55f2709fe5db513e801937e05e0f38a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453423"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="fe993-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="fe993-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="fe993-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe993-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe993-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fe993-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe993-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fe993-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe993-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fe993-107">Not yet documented</span></span>


<span data-ttu-id="fe993-108">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="fe993-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fe993-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe993-109">Properties</span></span>
|<span data-ttu-id="fe993-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe993-110">Property</span></span>|<span data-ttu-id="fe993-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe993-111">Type</span></span>|<span data-ttu-id="fe993-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe993-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe993-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="fe993-113">activeHoursStart</span></span>|<span data-ttu-id="fe993-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fe993-114">TimeOfDay</span></span>|<span data-ttu-id="fe993-115">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="fe993-115">Active Hours Start</span></span>|
|<span data-ttu-id="fe993-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="fe993-116">activeHoursEnd</span></span>|<span data-ttu-id="fe993-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fe993-117">TimeOfDay</span></span>|<span data-ttu-id="fe993-118">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="fe993-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe993-119">Relações</span><span class="sxs-lookup"><span data-stu-id="fe993-119">Relationships</span></span>
<span data-ttu-id="fe993-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fe993-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe993-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe993-121">JSON Representation</span></span>
<span data-ttu-id="fe993-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe993-122">Here is a JSON representation of the resource.</span></span>
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



