---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 81ccc29bfe0eb9c3d0d943975807cbf5776051a9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758761"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="b7c6d-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="b7c6d-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="b7c6d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7c6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7c6d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7c6d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7c6d-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b7c6d-106">Not yet documented</span></span>


<span data-ttu-id="b7c6d-107">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="b7c6d-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b7c6d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7c6d-108">Properties</span></span>
|<span data-ttu-id="b7c6d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7c6d-109">Property</span></span>|<span data-ttu-id="b7c6d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7c6d-110">Type</span></span>|<span data-ttu-id="b7c6d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7c6d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7c6d-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="b7c6d-112">activeHoursStart</span></span>|<span data-ttu-id="b7c6d-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b7c6d-113">TimeOfDay</span></span>|<span data-ttu-id="b7c6d-114">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="b7c6d-114">Active Hours Start</span></span>|
|<span data-ttu-id="b7c6d-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="b7c6d-115">activeHoursEnd</span></span>|<span data-ttu-id="b7c6d-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b7c6d-116">TimeOfDay</span></span>|<span data-ttu-id="b7c6d-117">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="b7c6d-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7c6d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="b7c6d-118">Relationships</span></span>
<span data-ttu-id="b7c6d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b7c6d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7c6d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7c6d-120">JSON Representation</span></span>
<span data-ttu-id="b7c6d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b7c6d-121">Here is a JSON representation of the resource.</span></span>
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




