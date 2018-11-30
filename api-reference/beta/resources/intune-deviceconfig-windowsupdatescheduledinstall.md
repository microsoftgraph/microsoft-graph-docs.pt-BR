---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
ms.openlocfilehash: 9f39a9716efed39529c54eaddc62cde075b51954
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035204"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="acaac-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="acaac-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="acaac-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="acaac-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acaac-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="acaac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="acaac-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="acaac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="acaac-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="acaac-107">Not yet documented</span></span>

<span data-ttu-id="acaac-108">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="acaac-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="acaac-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="acaac-109">Properties</span></span>
|<span data-ttu-id="acaac-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acaac-110">Property</span></span>|<span data-ttu-id="acaac-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="acaac-111">Type</span></span>|<span data-ttu-id="acaac-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="acaac-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acaac-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="acaac-113">scheduledInstallDay</span></span>|[<span data-ttu-id="acaac-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="acaac-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="acaac-115">Agendada instalar o dia na semana.</span><span class="sxs-lookup"><span data-stu-id="acaac-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="acaac-116">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="acaac-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="acaac-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="acaac-117">scheduledInstallTime</span></span>|<span data-ttu-id="acaac-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="acaac-118">TimeOfDay</span></span>|<span data-ttu-id="acaac-119">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="acaac-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="acaac-120">Relações</span><span class="sxs-lookup"><span data-stu-id="acaac-120">Relationships</span></span>
<span data-ttu-id="acaac-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="acaac-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="acaac-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="acaac-122">JSON Representation</span></span>
<span data-ttu-id="acaac-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="acaac-123">Here is a JSON representation of the resource.</span></span>
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





