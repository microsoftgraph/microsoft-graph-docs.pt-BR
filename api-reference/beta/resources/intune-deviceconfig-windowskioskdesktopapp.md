---
title: tipo de recurso Complexowindowskioskdesktopapp
description: A classe base de um tipo de aplicativo
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a1541b12754307844e89a06c02ab78081856ee4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943883"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="f91e6-103">tipo de recurso Complexowindowskioskdesktopapp</span><span class="sxs-lookup"><span data-stu-id="f91e6-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="f91e6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f91e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f91e6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f91e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f91e6-106">A classe base de um tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="f91e6-106">The base class for a type of apps</span></span>


<span data-ttu-id="f91e6-107">Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="f91e6-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f91e6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f91e6-108">Properties</span></span>
|<span data-ttu-id="f91e6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f91e6-109">Property</span></span>|<span data-ttu-id="f91e6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f91e6-110">Type</span></span>|<span data-ttu-id="f91e6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f91e6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f91e6-112">Propriedadesstartlayouttilesize</span><span class="sxs-lookup"><span data-stu-id="f91e6-112">startLayoutTileSize</span></span>|[<span data-ttu-id="f91e6-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="f91e6-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="f91e6-114">O tamanho do bloco do aplicativo para o layout inicial herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="f91e6-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="f91e6-115">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="f91e6-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="f91e6-116">nome</span><span class="sxs-lookup"><span data-stu-id="f91e6-116">name</span></span>|<span data-ttu-id="f91e6-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f91e6-117">String</span></span>|<span data-ttu-id="f91e6-118">Representa o nome amigável de um aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="f91e6-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="f91e6-119">appType</span><span class="sxs-lookup"><span data-stu-id="f91e6-119">appType</span></span>|[<span data-ttu-id="f91e6-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="f91e6-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="f91e6-121">O tipo de aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="f91e6-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="f91e6-122">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="f91e6-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="f91e6-123">autolançamento</span><span class="sxs-lookup"><span data-stu-id="f91e6-123">autoLaunch</span></span>|<span data-ttu-id="f91e6-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="f91e6-124">Boolean</span></span>|<span data-ttu-id="f91e6-125">Permitir que o aplicativo seja iniciado automaticamente no modo de quiosque de vários aplicativos herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="f91e6-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="f91e6-126">caminho</span><span class="sxs-lookup"><span data-stu-id="f91e6-126">path</span></span>|<span data-ttu-id="f91e6-127">String</span><span class="sxs-lookup"><span data-stu-id="f91e6-127">String</span></span>|<span data-ttu-id="f91e6-128">Definir o caminho de um aplicativo de área de trabalho</span><span class="sxs-lookup"><span data-stu-id="f91e6-128">Define the path of a desktop app</span></span>|
|<span data-ttu-id="f91e6-129">Propriedadesdesktopapplicationid</span><span class="sxs-lookup"><span data-stu-id="f91e6-129">desktopApplicationId</span></span>|<span data-ttu-id="f91e6-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f91e6-130">String</span></span>|<span data-ttu-id="f91e6-131">Definir o Propriedadesdesktopapplicationid do aplicativo</span><span class="sxs-lookup"><span data-stu-id="f91e6-131">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="f91e6-132">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="f91e6-132">desktopApplicationLinkPath</span></span>|<span data-ttu-id="f91e6-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f91e6-133">String</span></span>|<span data-ttu-id="f91e6-134">Definir o DesktopApplicationLinkPath do aplicativo</span><span class="sxs-lookup"><span data-stu-id="f91e6-134">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="f91e6-135">Relações</span><span class="sxs-lookup"><span data-stu-id="f91e6-135">Relationships</span></span>
<span data-ttu-id="f91e6-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f91e6-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f91e6-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f91e6-137">JSON Representation</span></span>
<span data-ttu-id="f91e6-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f91e6-138">Here is a JSON representation of the resource.</span></span>
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
  "autoLaunch": true,
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```




