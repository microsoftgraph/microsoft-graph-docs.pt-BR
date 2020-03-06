---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d66aae6ed12abe546b5a7776e864015e20896ee7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530338"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="c0fc4-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="c0fc4-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="c0fc4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0fc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0fc4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0fc4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0fc4-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c0fc4-106">Not yet documented</span></span>


<span data-ttu-id="c0fc4-107">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="c0fc4-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c0fc4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0fc4-108">Properties</span></span>
|<span data-ttu-id="c0fc4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0fc4-109">Property</span></span>|<span data-ttu-id="c0fc4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0fc4-110">Type</span></span>|<span data-ttu-id="c0fc4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0fc4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0fc4-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="c0fc4-112">activeHoursStart</span></span>|<span data-ttu-id="c0fc4-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c0fc4-113">TimeOfDay</span></span>|<span data-ttu-id="c0fc4-114">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="c0fc4-114">Active Hours Start</span></span>|
|<span data-ttu-id="c0fc4-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="c0fc4-115">activeHoursEnd</span></span>|<span data-ttu-id="c0fc4-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c0fc4-116">TimeOfDay</span></span>|<span data-ttu-id="c0fc4-117">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="c0fc4-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0fc4-118">Relações</span><span class="sxs-lookup"><span data-stu-id="c0fc4-118">Relationships</span></span>
<span data-ttu-id="c0fc4-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c0fc4-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0fc4-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0fc4-120">JSON Representation</span></span>
<span data-ttu-id="c0fc4-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0fc4-121">Here is a JSON representation of the resource.</span></span>
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




