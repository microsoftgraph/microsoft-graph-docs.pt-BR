---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3635441f015d49ffb402f5314896e9e68b15e8e7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030923"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="6aaa8-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="6aaa8-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="6aaa8-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6aaa8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6aaa8-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6aaa8-105">Not yet documented</span></span>


<span data-ttu-id="6aaa8-106">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="6aaa8-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6aaa8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6aaa8-107">Properties</span></span>
|<span data-ttu-id="6aaa8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6aaa8-108">Property</span></span>|<span data-ttu-id="6aaa8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6aaa8-109">Type</span></span>|<span data-ttu-id="6aaa8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6aaa8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6aaa8-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="6aaa8-111">activeHoursStart</span></span>|<span data-ttu-id="6aaa8-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6aaa8-112">TimeOfDay</span></span>|<span data-ttu-id="6aaa8-113">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="6aaa8-113">Active Hours Start</span></span>|
|<span data-ttu-id="6aaa8-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="6aaa8-114">activeHoursEnd</span></span>|<span data-ttu-id="6aaa8-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6aaa8-115">TimeOfDay</span></span>|<span data-ttu-id="6aaa8-116">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="6aaa8-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="6aaa8-117">Relações</span><span class="sxs-lookup"><span data-stu-id="6aaa8-117">Relationships</span></span>
<span data-ttu-id="6aaa8-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6aaa8-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6aaa8-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6aaa8-119">JSON Representation</span></span>
<span data-ttu-id="6aaa8-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6aaa8-120">Here is a JSON representation of the resource.</span></span>
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



