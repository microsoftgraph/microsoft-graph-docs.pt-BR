---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d217a9c6b3cb73a15a863491798115fef3a4c556
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49231314"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="2bd0b-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="2bd0b-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="2bd0b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bd0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2bd0b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2bd0b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bd0b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2bd0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bd0b-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2bd0b-107">Not yet documented</span></span>


<span data-ttu-id="2bd0b-108">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="2bd0b-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2bd0b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2bd0b-109">Properties</span></span>
|<span data-ttu-id="2bd0b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2bd0b-110">Property</span></span>|<span data-ttu-id="2bd0b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bd0b-111">Type</span></span>|<span data-ttu-id="2bd0b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bd0b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bd0b-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="2bd0b-113">activeHoursStart</span></span>|<span data-ttu-id="2bd0b-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2bd0b-114">TimeOfDay</span></span>|<span data-ttu-id="2bd0b-115">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="2bd0b-115">Active Hours Start</span></span>|
|<span data-ttu-id="2bd0b-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="2bd0b-116">activeHoursEnd</span></span>|<span data-ttu-id="2bd0b-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2bd0b-117">TimeOfDay</span></span>|<span data-ttu-id="2bd0b-118">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="2bd0b-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bd0b-119">Relações</span><span class="sxs-lookup"><span data-stu-id="2bd0b-119">Relationships</span></span>
<span data-ttu-id="2bd0b-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2bd0b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2bd0b-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2bd0b-121">JSON Representation</span></span>
<span data-ttu-id="2bd0b-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2bd0b-122">Here is a JSON representation of the resource.</span></span>
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




