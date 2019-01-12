---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ad513d4022b991917a7afe8ce9bdf012095621de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931241"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="70fc8-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="70fc8-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="70fc8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="70fc8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70fc8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="70fc8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70fc8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="70fc8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70fc8-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="70fc8-107">Not yet documented</span></span>

<span data-ttu-id="70fc8-108">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="70fc8-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="70fc8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70fc8-109">Properties</span></span>
|<span data-ttu-id="70fc8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70fc8-110">Property</span></span>|<span data-ttu-id="70fc8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="70fc8-111">Type</span></span>|<span data-ttu-id="70fc8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="70fc8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70fc8-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="70fc8-113">activeHoursStart</span></span>|<span data-ttu-id="70fc8-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="70fc8-114">TimeOfDay</span></span>|<span data-ttu-id="70fc8-115">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="70fc8-115">Active Hours Start</span></span>|
|<span data-ttu-id="70fc8-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="70fc8-116">activeHoursEnd</span></span>|<span data-ttu-id="70fc8-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="70fc8-117">TimeOfDay</span></span>|<span data-ttu-id="70fc8-118">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="70fc8-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="70fc8-119">Relações</span><span class="sxs-lookup"><span data-stu-id="70fc8-119">Relationships</span></span>
<span data-ttu-id="70fc8-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70fc8-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="70fc8-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70fc8-121">JSON Representation</span></span>
<span data-ttu-id="70fc8-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70fc8-122">Here is a JSON representation of the resource.</span></span>
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





