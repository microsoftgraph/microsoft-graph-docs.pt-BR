---
title: tipo de recurso Complexowindowskioskdesktopapp
description: A classe base de um tipo de aplicativo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0487fa24ecd2d27817349b68063cf606a2401944
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170473"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="3f294-103">tipo de recurso Complexowindowskioskdesktopapp</span><span class="sxs-lookup"><span data-stu-id="3f294-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="3f294-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3f294-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f294-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3f294-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f294-106">A classe base de um tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f294-106">The base class for a type of apps</span></span>


<span data-ttu-id="3f294-107">Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="3f294-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3f294-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f294-108">Properties</span></span>
|<span data-ttu-id="3f294-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f294-109">Property</span></span>|<span data-ttu-id="3f294-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f294-110">Type</span></span>|<span data-ttu-id="3f294-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f294-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f294-112">Propriedadesstartlayouttilesize</span><span class="sxs-lookup"><span data-stu-id="3f294-112">startLayoutTileSize</span></span>|[<span data-ttu-id="3f294-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="3f294-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="3f294-114">O tamanho do bloco do aplicativo para o layout inicial herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="3f294-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="3f294-115">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="3f294-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="3f294-116">name</span><span class="sxs-lookup"><span data-stu-id="3f294-116">name</span></span>|<span data-ttu-id="3f294-117">String</span><span class="sxs-lookup"><span data-stu-id="3f294-117">String</span></span>|<span data-ttu-id="3f294-118">Representa o nome amigável de um aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="3f294-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="3f294-119">appType</span><span class="sxs-lookup"><span data-stu-id="3f294-119">appType</span></span>|[<span data-ttu-id="3f294-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="3f294-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="3f294-121">O tipo de aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="3f294-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="3f294-122">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="3f294-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="3f294-123">caminho</span><span class="sxs-lookup"><span data-stu-id="3f294-123">path</span></span>|<span data-ttu-id="3f294-124">String</span><span class="sxs-lookup"><span data-stu-id="3f294-124">String</span></span>|<span data-ttu-id="3f294-125">Definir o caminho de um aplicativo de área de trabalho</span><span class="sxs-lookup"><span data-stu-id="3f294-125">Define the path of a desktop app</span></span>|
|<span data-ttu-id="3f294-126">Propriedadesdesktopapplicationid</span><span class="sxs-lookup"><span data-stu-id="3f294-126">desktopApplicationId</span></span>|<span data-ttu-id="3f294-127">String</span><span class="sxs-lookup"><span data-stu-id="3f294-127">String</span></span>|<span data-ttu-id="3f294-128">Definir o Propriedadesdesktopapplicationid do aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f294-128">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="3f294-129">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="3f294-129">desktopApplicationLinkPath</span></span>|<span data-ttu-id="3f294-130">String</span><span class="sxs-lookup"><span data-stu-id="3f294-130">String</span></span>|<span data-ttu-id="3f294-131">Definir o DesktopApplicationLinkPath do aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f294-131">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f294-132">Relações</span><span class="sxs-lookup"><span data-stu-id="3f294-132">Relationships</span></span>
<span data-ttu-id="3f294-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f294-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f294-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f294-134">JSON Representation</span></span>
<span data-ttu-id="3f294-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f294-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskDesktopApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```




