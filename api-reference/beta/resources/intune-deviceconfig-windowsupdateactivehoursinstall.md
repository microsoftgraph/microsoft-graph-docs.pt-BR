---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6ae015503909ff6b9c627923ff809cebaa91468d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039696"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="3fdd2-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="3fdd2-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="3fdd2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fdd2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3fdd2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3fdd2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fdd2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3fdd2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fdd2-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3fdd2-107">Not yet documented</span></span>


<span data-ttu-id="3fdd2-108">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="3fdd2-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3fdd2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3fdd2-109">Properties</span></span>
|<span data-ttu-id="3fdd2-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3fdd2-110">Property</span></span>|<span data-ttu-id="3fdd2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fdd2-111">Type</span></span>|<span data-ttu-id="3fdd2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fdd2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fdd2-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="3fdd2-113">activeHoursStart</span></span>|<span data-ttu-id="3fdd2-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="3fdd2-114">TimeOfDay</span></span>|<span data-ttu-id="3fdd2-115">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="3fdd2-115">Active Hours Start</span></span>|
|<span data-ttu-id="3fdd2-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="3fdd2-116">activeHoursEnd</span></span>|<span data-ttu-id="3fdd2-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="3fdd2-117">TimeOfDay</span></span>|<span data-ttu-id="3fdd2-118">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="3fdd2-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="3fdd2-119">Relações</span><span class="sxs-lookup"><span data-stu-id="3fdd2-119">Relationships</span></span>
<span data-ttu-id="3fdd2-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3fdd2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3fdd2-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3fdd2-121">JSON Representation</span></span>
<span data-ttu-id="3fdd2-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3fdd2-122">Here is a JSON representation of the resource.</span></span>
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






