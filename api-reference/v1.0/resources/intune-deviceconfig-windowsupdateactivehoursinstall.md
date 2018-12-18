---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: d5ebe214a79e880adc408f3c55c2b9d39f00668d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327689"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="22bf7-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="22bf7-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="22bf7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="22bf7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22bf7-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="22bf7-105">Not yet documented</span></span>

<span data-ttu-id="22bf7-106">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="22bf7-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="22bf7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22bf7-107">Properties</span></span>
|<span data-ttu-id="22bf7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22bf7-108">Property</span></span>|<span data-ttu-id="22bf7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="22bf7-109">Type</span></span>|<span data-ttu-id="22bf7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="22bf7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22bf7-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="22bf7-111">activeHoursStart</span></span>|<span data-ttu-id="22bf7-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="22bf7-112">TimeOfDay</span></span>|<span data-ttu-id="22bf7-113">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="22bf7-113">Active Hours Start</span></span>|
|<span data-ttu-id="22bf7-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="22bf7-114">activeHoursEnd</span></span>|<span data-ttu-id="22bf7-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="22bf7-115">TimeOfDay</span></span>|<span data-ttu-id="22bf7-116">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="22bf7-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="22bf7-117">Relações</span><span class="sxs-lookup"><span data-stu-id="22bf7-117">Relationships</span></span>
<span data-ttu-id="22bf7-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="22bf7-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="22bf7-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22bf7-119">JSON Representation</span></span>
<span data-ttu-id="22bf7-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="22bf7-120">Here is a JSON representation of the resource.</span></span>
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



