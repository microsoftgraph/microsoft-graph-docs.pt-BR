---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49238831005d579baba2dd55e431f1ac684e67d3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943652"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="c4d13-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="c4d13-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="c4d13-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4d13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4d13-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4d13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4d13-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c4d13-106">Not yet documented</span></span>


<span data-ttu-id="c4d13-107">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="c4d13-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c4d13-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c4d13-108">Properties</span></span>
|<span data-ttu-id="c4d13-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4d13-109">Property</span></span>|<span data-ttu-id="c4d13-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4d13-110">Type</span></span>|<span data-ttu-id="c4d13-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4d13-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4d13-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="c4d13-112">activeHoursStart</span></span>|<span data-ttu-id="c4d13-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c4d13-113">TimeOfDay</span></span>|<span data-ttu-id="c4d13-114">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="c4d13-114">Active Hours Start</span></span>|
|<span data-ttu-id="c4d13-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="c4d13-115">activeHoursEnd</span></span>|<span data-ttu-id="c4d13-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c4d13-116">TimeOfDay</span></span>|<span data-ttu-id="c4d13-117">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="c4d13-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4d13-118">Relações</span><span class="sxs-lookup"><span data-stu-id="c4d13-118">Relationships</span></span>
<span data-ttu-id="c4d13-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c4d13-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4d13-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c4d13-120">JSON Representation</span></span>
<span data-ttu-id="c4d13-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c4d13-121">Here is a JSON representation of the resource.</span></span>
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




