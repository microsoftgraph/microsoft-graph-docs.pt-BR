---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 556e0f22bb249a8606b3bbf9bb3252d3721793b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845735"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="b9194-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="b9194-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="b9194-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b9194-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9194-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b9194-105">Not yet documented</span></span>

<span data-ttu-id="b9194-106">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="b9194-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b9194-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9194-107">Properties</span></span>
|<span data-ttu-id="b9194-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9194-108">Property</span></span>|<span data-ttu-id="b9194-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9194-109">Type</span></span>|<span data-ttu-id="b9194-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9194-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9194-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="b9194-111">activeHoursStart</span></span>|<span data-ttu-id="b9194-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b9194-112">TimeOfDay</span></span>|<span data-ttu-id="b9194-113">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="b9194-113">Active Hours Start</span></span>|
|<span data-ttu-id="b9194-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="b9194-114">activeHoursEnd</span></span>|<span data-ttu-id="b9194-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b9194-115">TimeOfDay</span></span>|<span data-ttu-id="b9194-116">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="b9194-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9194-117">Relações</span><span class="sxs-lookup"><span data-stu-id="b9194-117">Relationships</span></span>
<span data-ttu-id="b9194-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9194-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b9194-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9194-119">JSON Representation</span></span>
<span data-ttu-id="b9194-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9194-120">Here is a JSON representation of the resource.</span></span>
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



