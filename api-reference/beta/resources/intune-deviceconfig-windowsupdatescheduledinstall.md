---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ee91ed2541c02adbb7a130f0a9de869d86044632
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395626"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="438f8-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="438f8-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="438f8-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="438f8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="438f8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="438f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="438f8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="438f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="438f8-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="438f8-107">Not yet documented</span></span>


<span data-ttu-id="438f8-108">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="438f8-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="438f8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="438f8-109">Properties</span></span>
|<span data-ttu-id="438f8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="438f8-110">Property</span></span>|<span data-ttu-id="438f8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="438f8-111">Type</span></span>|<span data-ttu-id="438f8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="438f8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="438f8-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="438f8-113">scheduledInstallDay</span></span>|[<span data-ttu-id="438f8-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="438f8-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="438f8-115">Agendada instalar o dia na semana.</span><span class="sxs-lookup"><span data-stu-id="438f8-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="438f8-116">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="438f8-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="438f8-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="438f8-117">scheduledInstallTime</span></span>|<span data-ttu-id="438f8-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="438f8-118">TimeOfDay</span></span>|<span data-ttu-id="438f8-119">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="438f8-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="438f8-120">Relações</span><span class="sxs-lookup"><span data-stu-id="438f8-120">Relationships</span></span>
<span data-ttu-id="438f8-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="438f8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="438f8-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="438f8-122">JSON Representation</span></span>
<span data-ttu-id="438f8-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="438f8-123">Here is a JSON representation of the resource.</span></span>
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




