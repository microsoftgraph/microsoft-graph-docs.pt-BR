---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8ae4cb747cb4648cd9f4cc9550933688d180dd38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952038"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="6d82e-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="6d82e-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="6d82e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6d82e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d82e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6d82e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d82e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6d82e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d82e-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6d82e-107">Not yet documented</span></span>

<span data-ttu-id="6d82e-108">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="6d82e-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6d82e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d82e-109">Properties</span></span>
|<span data-ttu-id="6d82e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d82e-110">Property</span></span>|<span data-ttu-id="6d82e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d82e-111">Type</span></span>|<span data-ttu-id="6d82e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d82e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d82e-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="6d82e-113">scheduledInstallDay</span></span>|[<span data-ttu-id="6d82e-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="6d82e-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="6d82e-115">Agendada instalar o dia na semana.</span><span class="sxs-lookup"><span data-stu-id="6d82e-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="6d82e-116">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="6d82e-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="6d82e-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="6d82e-117">scheduledInstallTime</span></span>|<span data-ttu-id="6d82e-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6d82e-118">TimeOfDay</span></span>|<span data-ttu-id="6d82e-119">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="6d82e-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d82e-120">Relações</span><span class="sxs-lookup"><span data-stu-id="6d82e-120">Relationships</span></span>
<span data-ttu-id="6d82e-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6d82e-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6d82e-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d82e-122">JSON Representation</span></span>
<span data-ttu-id="6d82e-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d82e-123">Here is a JSON representation of the resource.</span></span>
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





