---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3d9460051726b93f61d10a2f9127bdaada76d397
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091457"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="273ad-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="273ad-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="273ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="273ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="273ad-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="273ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="273ad-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="273ad-106">Not yet documented</span></span>


<span data-ttu-id="273ad-107">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="273ad-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="273ad-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="273ad-108">Properties</span></span>
|<span data-ttu-id="273ad-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="273ad-109">Property</span></span>|<span data-ttu-id="273ad-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="273ad-110">Type</span></span>|<span data-ttu-id="273ad-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="273ad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="273ad-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="273ad-112">activeHoursStart</span></span>|<span data-ttu-id="273ad-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="273ad-113">TimeOfDay</span></span>|<span data-ttu-id="273ad-114">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="273ad-114">Active Hours Start</span></span>|
|<span data-ttu-id="273ad-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="273ad-115">activeHoursEnd</span></span>|<span data-ttu-id="273ad-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="273ad-116">TimeOfDay</span></span>|<span data-ttu-id="273ad-117">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="273ad-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="273ad-118">Relações</span><span class="sxs-lookup"><span data-stu-id="273ad-118">Relationships</span></span>
<span data-ttu-id="273ad-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="273ad-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="273ad-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="273ad-120">JSON Representation</span></span>
<span data-ttu-id="273ad-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="273ad-121">Here is a JSON representation of the resource.</span></span>
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









