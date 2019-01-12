---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3c0a58bf0bb6bc95c0208e1195566d5fc125073d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971848"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="0ba76-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="0ba76-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="0ba76-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0ba76-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ba76-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0ba76-105">Not yet documented</span></span>

<span data-ttu-id="0ba76-106">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="0ba76-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0ba76-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ba76-107">Properties</span></span>
|<span data-ttu-id="0ba76-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ba76-108">Property</span></span>|<span data-ttu-id="0ba76-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ba76-109">Type</span></span>|<span data-ttu-id="0ba76-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ba76-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ba76-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="0ba76-111">scheduledInstallDay</span></span>|[<span data-ttu-id="0ba76-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="0ba76-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="0ba76-113">Agendada instalar o dia na semana.</span><span class="sxs-lookup"><span data-stu-id="0ba76-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="0ba76-114">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="0ba76-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="0ba76-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="0ba76-115">scheduledInstallTime</span></span>|<span data-ttu-id="0ba76-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0ba76-116">TimeOfDay</span></span>|<span data-ttu-id="0ba76-117">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="0ba76-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ba76-118">Relações</span><span class="sxs-lookup"><span data-stu-id="0ba76-118">Relationships</span></span>
<span data-ttu-id="0ba76-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0ba76-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0ba76-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ba76-120">JSON Representation</span></span>
<span data-ttu-id="0ba76-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ba76-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```



