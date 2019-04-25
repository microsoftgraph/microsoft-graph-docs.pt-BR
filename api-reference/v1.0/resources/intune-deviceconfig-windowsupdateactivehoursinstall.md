---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42d0ecbb7745346d5fc8d25fbc1aa595c8f1887f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573456"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="8c3e0-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="8c3e0-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="8c3e0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c3e0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c3e0-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8c3e0-105">Not yet documented</span></span>


<span data-ttu-id="8c3e0-106">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="8c3e0-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8c3e0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c3e0-107">Properties</span></span>
|<span data-ttu-id="8c3e0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c3e0-108">Property</span></span>|<span data-ttu-id="8c3e0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c3e0-109">Type</span></span>|<span data-ttu-id="8c3e0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c3e0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c3e0-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="8c3e0-111">activeHoursStart</span></span>|<span data-ttu-id="8c3e0-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8c3e0-112">TimeOfDay</span></span>|<span data-ttu-id="8c3e0-113">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="8c3e0-113">Active Hours Start</span></span>|
|<span data-ttu-id="8c3e0-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="8c3e0-114">activeHoursEnd</span></span>|<span data-ttu-id="8c3e0-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8c3e0-115">TimeOfDay</span></span>|<span data-ttu-id="8c3e0-116">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="8c3e0-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c3e0-117">Relações</span><span class="sxs-lookup"><span data-stu-id="8c3e0-117">Relationships</span></span>
<span data-ttu-id="8c3e0-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8c3e0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c3e0-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c3e0-119">JSON Representation</span></span>
<span data-ttu-id="8c3e0-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c3e0-120">Here is a JSON representation of the resource.</span></span>
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



