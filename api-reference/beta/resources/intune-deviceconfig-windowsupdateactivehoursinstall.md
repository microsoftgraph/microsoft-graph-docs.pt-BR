---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0c40fc7ade30a73212d1917294671fdb5423483
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978763"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="b61b1-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="b61b1-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="b61b1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b61b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b61b1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b61b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b61b1-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b61b1-106">Not yet documented</span></span>


<span data-ttu-id="b61b1-107">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="b61b1-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b61b1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b61b1-108">Properties</span></span>
|<span data-ttu-id="b61b1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b61b1-109">Property</span></span>|<span data-ttu-id="b61b1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b61b1-110">Type</span></span>|<span data-ttu-id="b61b1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b61b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b61b1-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="b61b1-112">activeHoursStart</span></span>|<span data-ttu-id="b61b1-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b61b1-113">TimeOfDay</span></span>|<span data-ttu-id="b61b1-114">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="b61b1-114">Active Hours Start</span></span>|
|<span data-ttu-id="b61b1-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="b61b1-115">activeHoursEnd</span></span>|<span data-ttu-id="b61b1-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b61b1-116">TimeOfDay</span></span>|<span data-ttu-id="b61b1-117">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="b61b1-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="b61b1-118">Relações</span><span class="sxs-lookup"><span data-stu-id="b61b1-118">Relationships</span></span>
<span data-ttu-id="b61b1-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b61b1-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b61b1-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b61b1-120">JSON Representation</span></span>
<span data-ttu-id="b61b1-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b61b1-121">Here is a JSON representation of the resource.</span></span>
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





