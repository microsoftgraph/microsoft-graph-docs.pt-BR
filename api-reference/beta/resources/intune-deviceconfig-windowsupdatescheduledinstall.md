---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 47518277f54526e84cc3152a96ba3b49ec8a199e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835998"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="2b471-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="2b471-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="2b471-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2b471-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b471-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2b471-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b471-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2b471-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b471-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2b471-107">Not yet documented</span></span>

<span data-ttu-id="2b471-108">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="2b471-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2b471-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b471-109">Properties</span></span>
|<span data-ttu-id="2b471-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b471-110">Property</span></span>|<span data-ttu-id="2b471-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b471-111">Type</span></span>|<span data-ttu-id="2b471-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b471-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b471-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="2b471-113">scheduledInstallDay</span></span>|[<span data-ttu-id="2b471-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="2b471-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="2b471-115">Agendada instalar o dia na semana.</span><span class="sxs-lookup"><span data-stu-id="2b471-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="2b471-116">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="2b471-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="2b471-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="2b471-117">scheduledInstallTime</span></span>|<span data-ttu-id="2b471-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2b471-118">TimeOfDay</span></span>|<span data-ttu-id="2b471-119">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="2b471-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b471-120">Relações</span><span class="sxs-lookup"><span data-stu-id="2b471-120">Relationships</span></span>
<span data-ttu-id="2b471-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b471-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2b471-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b471-122">JSON Representation</span></span>
<span data-ttu-id="2b471-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b471-123">Here is a JSON representation of the resource.</span></span>
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





