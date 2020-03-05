---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 20a3164a11c940538bc6ffc67ac4b1911df85f27
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525387"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="12719-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="12719-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="12719-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="12719-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12719-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="12719-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12719-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12719-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12719-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="12719-107">Not yet documented</span></span>


<span data-ttu-id="12719-108">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="12719-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="12719-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12719-109">Properties</span></span>
|<span data-ttu-id="12719-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12719-110">Property</span></span>|<span data-ttu-id="12719-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="12719-111">Type</span></span>|<span data-ttu-id="12719-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="12719-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12719-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="12719-113">activeHoursStart</span></span>|<span data-ttu-id="12719-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="12719-114">TimeOfDay</span></span>|<span data-ttu-id="12719-115">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="12719-115">Active Hours Start</span></span>|
|<span data-ttu-id="12719-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="12719-116">activeHoursEnd</span></span>|<span data-ttu-id="12719-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="12719-117">TimeOfDay</span></span>|<span data-ttu-id="12719-118">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="12719-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="12719-119">Relações</span><span class="sxs-lookup"><span data-stu-id="12719-119">Relationships</span></span>
<span data-ttu-id="12719-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12719-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="12719-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12719-121">JSON Representation</span></span>
<span data-ttu-id="12719-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12719-122">Here is a JSON representation of the resource.</span></span>
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



