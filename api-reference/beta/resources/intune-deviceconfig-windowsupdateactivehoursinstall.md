---
title: Tipo de recurso windowsUpdateActiveHoursInstall
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 6d1328723f546f553bc31903d36ada2242d8cda3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307102"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="d7bf2-103">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="d7bf2-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="d7bf2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d7bf2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7bf2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d7bf2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7bf2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d7bf2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7bf2-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d7bf2-107">Not yet documented</span></span>

<span data-ttu-id="d7bf2-108">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="d7bf2-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d7bf2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7bf2-109">Properties</span></span>
|<span data-ttu-id="d7bf2-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7bf2-110">Property</span></span>|<span data-ttu-id="d7bf2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7bf2-111">Type</span></span>|<span data-ttu-id="d7bf2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7bf2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7bf2-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="d7bf2-113">activeHoursStart</span></span>|<span data-ttu-id="d7bf2-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d7bf2-114">TimeOfDay</span></span>|<span data-ttu-id="d7bf2-115">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="d7bf2-115">Active Hours Start</span></span>|
|<span data-ttu-id="d7bf2-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="d7bf2-116">activeHoursEnd</span></span>|<span data-ttu-id="d7bf2-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d7bf2-117">TimeOfDay</span></span>|<span data-ttu-id="d7bf2-118">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="d7bf2-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7bf2-119">Relações</span><span class="sxs-lookup"><span data-stu-id="d7bf2-119">Relationships</span></span>
<span data-ttu-id="d7bf2-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d7bf2-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d7bf2-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7bf2-121">JSON Representation</span></span>
<span data-ttu-id="d7bf2-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d7bf2-122">Here is a JSON representation of the resource.</span></span>
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





