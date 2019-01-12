---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ed4f909db5dd31195ace7d98151b226b03849c81
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967179"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="573dd-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="573dd-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="573dd-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="573dd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="573dd-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="573dd-105">Not yet documented</span></span>

<span data-ttu-id="573dd-106">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="573dd-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="573dd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="573dd-107">Properties</span></span>
|<span data-ttu-id="573dd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="573dd-108">Property</span></span>|<span data-ttu-id="573dd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="573dd-109">Type</span></span>|<span data-ttu-id="573dd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="573dd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="573dd-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="573dd-111">activeHoursStart</span></span>|<span data-ttu-id="573dd-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="573dd-112">TimeOfDay</span></span>|<span data-ttu-id="573dd-113">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="573dd-113">Active Hours Start</span></span>|
|<span data-ttu-id="573dd-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="573dd-114">activeHoursEnd</span></span>|<span data-ttu-id="573dd-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="573dd-115">TimeOfDay</span></span>|<span data-ttu-id="573dd-116">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="573dd-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="573dd-117">Relações</span><span class="sxs-lookup"><span data-stu-id="573dd-117">Relationships</span></span>
<span data-ttu-id="573dd-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="573dd-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="573dd-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="573dd-119">JSON Representation</span></span>
<span data-ttu-id="573dd-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="573dd-120">Here is a JSON representation of the resource.</span></span>
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



