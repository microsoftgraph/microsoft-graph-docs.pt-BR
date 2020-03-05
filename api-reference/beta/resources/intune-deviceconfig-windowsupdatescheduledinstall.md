---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 13c6df3f312872b1fab64c320c17ae3c3115c99e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528931"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="2c116-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="2c116-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="2c116-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2c116-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c116-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2c116-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c116-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c116-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c116-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2c116-107">Not yet documented</span></span>


<span data-ttu-id="2c116-108">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="2c116-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2c116-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c116-109">Properties</span></span>
|<span data-ttu-id="2c116-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c116-110">Property</span></span>|<span data-ttu-id="2c116-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c116-111">Type</span></span>|<span data-ttu-id="2c116-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c116-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c116-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="2c116-113">scheduledInstallDay</span></span>|[<span data-ttu-id="2c116-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="2c116-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="2c116-115">Dia da instalação agendada da semana.</span><span class="sxs-lookup"><span data-stu-id="2c116-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="2c116-116">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="2c116-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="2c116-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="2c116-117">scheduledInstallTime</span></span>|<span data-ttu-id="2c116-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2c116-118">TimeOfDay</span></span>|<span data-ttu-id="2c116-119">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="2c116-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c116-120">Relações</span><span class="sxs-lookup"><span data-stu-id="2c116-120">Relationships</span></span>
<span data-ttu-id="2c116-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c116-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c116-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c116-122">JSON Representation</span></span>
<span data-ttu-id="2c116-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c116-123">Here is a JSON representation of the resource.</span></span>
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



