---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e5d5c517e4b146c94b931caf09f354ed5a348080
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369567"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="9b870-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="9b870-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="9b870-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9b870-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b870-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b870-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b870-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b870-106">Not yet documented</span></span>


<span data-ttu-id="9b870-107">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="9b870-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9b870-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b870-108">Properties</span></span>
|<span data-ttu-id="9b870-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b870-109">Property</span></span>|<span data-ttu-id="9b870-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b870-110">Type</span></span>|<span data-ttu-id="9b870-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b870-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b870-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="9b870-112">activeHoursStart</span></span>|<span data-ttu-id="9b870-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9b870-113">TimeOfDay</span></span>|<span data-ttu-id="9b870-114">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="9b870-114">Active Hours Start</span></span>|
|<span data-ttu-id="9b870-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="9b870-115">activeHoursEnd</span></span>|<span data-ttu-id="9b870-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9b870-116">TimeOfDay</span></span>|<span data-ttu-id="9b870-117">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="9b870-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b870-118">Relações</span><span class="sxs-lookup"><span data-stu-id="9b870-118">Relationships</span></span>
<span data-ttu-id="9b870-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9b870-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b870-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b870-120">JSON Representation</span></span>
<span data-ttu-id="9b870-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b870-121">Here is a JSON representation of the resource.</span></span>
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



