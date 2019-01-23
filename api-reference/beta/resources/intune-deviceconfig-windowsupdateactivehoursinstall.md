---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 28f40501123f465d8fcbfa05c3febb8ffab6f27a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409465"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="7cd39-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="7cd39-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="7cd39-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7cd39-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7cd39-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7cd39-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7cd39-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7cd39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cd39-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7cd39-107">Not yet documented</span></span>


<span data-ttu-id="7cd39-108">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="7cd39-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7cd39-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7cd39-109">Properties</span></span>
|<span data-ttu-id="7cd39-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7cd39-110">Property</span></span>|<span data-ttu-id="7cd39-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7cd39-111">Type</span></span>|<span data-ttu-id="7cd39-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cd39-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cd39-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="7cd39-113">activeHoursStart</span></span>|<span data-ttu-id="7cd39-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7cd39-114">TimeOfDay</span></span>|<span data-ttu-id="7cd39-115">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="7cd39-115">Active Hours Start</span></span>|
|<span data-ttu-id="7cd39-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="7cd39-116">activeHoursEnd</span></span>|<span data-ttu-id="7cd39-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7cd39-117">TimeOfDay</span></span>|<span data-ttu-id="7cd39-118">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="7cd39-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="7cd39-119">Relações</span><span class="sxs-lookup"><span data-stu-id="7cd39-119">Relationships</span></span>
<span data-ttu-id="7cd39-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7cd39-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7cd39-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7cd39-121">JSON Representation</span></span>
<span data-ttu-id="7cd39-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7cd39-122">Here is a JSON representation of the resource.</span></span>
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




