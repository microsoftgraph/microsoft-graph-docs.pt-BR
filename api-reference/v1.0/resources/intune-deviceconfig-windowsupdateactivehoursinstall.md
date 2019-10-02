---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 29b885bcfd728f412d2e94ecdbdbdfc23ee9fb76
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357161"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="a7bea-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="a7bea-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="a7bea-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a7bea-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7bea-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a7bea-105">Not yet documented</span></span>


<span data-ttu-id="a7bea-106">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="a7bea-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a7bea-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a7bea-107">Properties</span></span>
|<span data-ttu-id="a7bea-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7bea-108">Property</span></span>|<span data-ttu-id="a7bea-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7bea-109">Type</span></span>|<span data-ttu-id="a7bea-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7bea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7bea-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="a7bea-111">activeHoursStart</span></span>|<span data-ttu-id="a7bea-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a7bea-112">TimeOfDay</span></span>|<span data-ttu-id="a7bea-113">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="a7bea-113">Active Hours Start</span></span>|
|<span data-ttu-id="a7bea-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="a7bea-114">activeHoursEnd</span></span>|<span data-ttu-id="a7bea-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a7bea-115">TimeOfDay</span></span>|<span data-ttu-id="a7bea-116">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="a7bea-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7bea-117">Relações</span><span class="sxs-lookup"><span data-stu-id="a7bea-117">Relationships</span></span>
<span data-ttu-id="a7bea-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a7bea-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7bea-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a7bea-119">JSON Representation</span></span>
<span data-ttu-id="a7bea-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a7bea-120">Here is a JSON representation of the resource.</span></span>
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




