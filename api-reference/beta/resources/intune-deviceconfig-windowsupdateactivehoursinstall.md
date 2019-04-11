---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f65d986fa59a3087a5fe1578eec626a27a4154b0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792717"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="6a972-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="6a972-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="6a972-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a972-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a972-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a972-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a972-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6a972-106">Not yet documented</span></span>


<span data-ttu-id="6a972-107">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="6a972-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6a972-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a972-108">Properties</span></span>
|<span data-ttu-id="6a972-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a972-109">Property</span></span>|<span data-ttu-id="6a972-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a972-110">Type</span></span>|<span data-ttu-id="6a972-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a972-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a972-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="6a972-112">activeHoursStart</span></span>|<span data-ttu-id="6a972-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6a972-113">TimeOfDay</span></span>|<span data-ttu-id="6a972-114">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="6a972-114">Active Hours Start</span></span>|
|<span data-ttu-id="6a972-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="6a972-115">activeHoursEnd</span></span>|<span data-ttu-id="6a972-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6a972-116">TimeOfDay</span></span>|<span data-ttu-id="6a972-117">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="6a972-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a972-118">Relações</span><span class="sxs-lookup"><span data-stu-id="6a972-118">Relationships</span></span>
<span data-ttu-id="6a972-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6a972-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a972-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a972-120">JSON Representation</span></span>
<span data-ttu-id="6a972-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a972-121">Here is a JSON representation of the resource.</span></span>
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





