---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f65d986fa59a3087a5fe1578eec626a27a4154b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555189"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="69d60-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="69d60-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="69d60-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69d60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69d60-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69d60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69d60-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="69d60-106">Not yet documented</span></span>


<span data-ttu-id="69d60-107">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="69d60-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="69d60-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69d60-108">Properties</span></span>
|<span data-ttu-id="69d60-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69d60-109">Property</span></span>|<span data-ttu-id="69d60-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="69d60-110">Type</span></span>|<span data-ttu-id="69d60-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="69d60-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69d60-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="69d60-112">activeHoursStart</span></span>|<span data-ttu-id="69d60-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="69d60-113">TimeOfDay</span></span>|<span data-ttu-id="69d60-114">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="69d60-114">Active Hours Start</span></span>|
|<span data-ttu-id="69d60-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="69d60-115">activeHoursEnd</span></span>|<span data-ttu-id="69d60-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="69d60-116">TimeOfDay</span></span>|<span data-ttu-id="69d60-117">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="69d60-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="69d60-118">Relações</span><span class="sxs-lookup"><span data-stu-id="69d60-118">Relationships</span></span>
<span data-ttu-id="69d60-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69d60-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69d60-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69d60-120">JSON Representation</span></span>
<span data-ttu-id="69d60-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69d60-121">Here is a JSON representation of the resource.</span></span>
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





