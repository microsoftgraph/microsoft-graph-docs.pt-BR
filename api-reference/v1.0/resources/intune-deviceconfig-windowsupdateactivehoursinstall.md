---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
ms.openlocfilehash: c9647cda65d680629fda57e3dfdcbffb3d5d8625
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003559"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="ce051-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="ce051-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="ce051-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ce051-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce051-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ce051-105">Not yet documented</span></span>

<span data-ttu-id="ce051-106">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="ce051-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ce051-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce051-107">Properties</span></span>
|<span data-ttu-id="ce051-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce051-108">Property</span></span>|<span data-ttu-id="ce051-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce051-109">Type</span></span>|<span data-ttu-id="ce051-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce051-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce051-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="ce051-111">activeHoursStart</span></span>|<span data-ttu-id="ce051-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ce051-112">TimeOfDay</span></span>|<span data-ttu-id="ce051-113">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="ce051-113">Active Hours Start</span></span>|
|<span data-ttu-id="ce051-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="ce051-114">activeHoursEnd</span></span>|<span data-ttu-id="ce051-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ce051-115">TimeOfDay</span></span>|<span data-ttu-id="ce051-116">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="ce051-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce051-117">Relações</span><span class="sxs-lookup"><span data-stu-id="ce051-117">Relationships</span></span>
<span data-ttu-id="ce051-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ce051-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ce051-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce051-119">JSON Representation</span></span>
<span data-ttu-id="ce051-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce051-120">Here is a JSON representation of the resource.</span></span>
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



