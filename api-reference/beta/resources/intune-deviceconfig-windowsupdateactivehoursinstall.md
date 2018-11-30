---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
ms.openlocfilehash: 7a40a791a9a00d7cfd60287bade1759592e1bcf2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039682"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="1817b-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="1817b-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="1817b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1817b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1817b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1817b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1817b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1817b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1817b-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1817b-107">Not yet documented</span></span>

<span data-ttu-id="1817b-108">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="1817b-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1817b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1817b-109">Properties</span></span>
|<span data-ttu-id="1817b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1817b-110">Property</span></span>|<span data-ttu-id="1817b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1817b-111">Type</span></span>|<span data-ttu-id="1817b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1817b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1817b-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="1817b-113">activeHoursStart</span></span>|<span data-ttu-id="1817b-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1817b-114">TimeOfDay</span></span>|<span data-ttu-id="1817b-115">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="1817b-115">Active Hours Start</span></span>|
|<span data-ttu-id="1817b-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="1817b-116">activeHoursEnd</span></span>|<span data-ttu-id="1817b-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1817b-117">TimeOfDay</span></span>|<span data-ttu-id="1817b-118">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="1817b-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="1817b-119">Relações</span><span class="sxs-lookup"><span data-stu-id="1817b-119">Relationships</span></span>
<span data-ttu-id="1817b-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1817b-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1817b-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1817b-121">JSON Representation</span></span>
<span data-ttu-id="1817b-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1817b-122">Here is a JSON representation of the resource.</span></span>
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





