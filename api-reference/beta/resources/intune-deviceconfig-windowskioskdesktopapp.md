---
title: tipo de recurso Complexowindowskioskdesktopapp
description: A classe base de um tipo de aplicativo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89f309b53e44b0f2843145dd7c0f4d3ffa6d7f98
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453961"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="5b313-103">tipo de recurso Complexowindowskioskdesktopapp</span><span class="sxs-lookup"><span data-stu-id="5b313-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="5b313-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5b313-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b313-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b313-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b313-106">A classe base de um tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b313-106">The base class for a type of apps</span></span>


<span data-ttu-id="5b313-107">Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="5b313-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5b313-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b313-108">Properties</span></span>
|<span data-ttu-id="5b313-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b313-109">Property</span></span>|<span data-ttu-id="5b313-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b313-110">Type</span></span>|<span data-ttu-id="5b313-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b313-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b313-112">Propriedadesstartlayouttilesize</span><span class="sxs-lookup"><span data-stu-id="5b313-112">startLayoutTileSize</span></span>|[<span data-ttu-id="5b313-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="5b313-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="5b313-114">O tamanho do bloco do aplicativo para o layout inicial herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="5b313-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="5b313-115">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="5b313-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="5b313-116">nome</span><span class="sxs-lookup"><span data-stu-id="5b313-116">name</span></span>|<span data-ttu-id="5b313-117">String</span><span class="sxs-lookup"><span data-stu-id="5b313-117">String</span></span>|<span data-ttu-id="5b313-118">Representa o nome amigável de um aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="5b313-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="5b313-119">appType</span><span class="sxs-lookup"><span data-stu-id="5b313-119">appType</span></span>|[<span data-ttu-id="5b313-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="5b313-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="5b313-121">O tipo de aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="5b313-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="5b313-122">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="5b313-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="5b313-123">autoLançamento</span><span class="sxs-lookup"><span data-stu-id="5b313-123">autoLaunch</span></span>|<span data-ttu-id="5b313-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b313-124">Boolean</span></span>|<span data-ttu-id="5b313-125">Permitir que o aplicativo seja iniciado automaticamente no modo de quiosque de vários aplicativos herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="5b313-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="5b313-126">caminho</span><span class="sxs-lookup"><span data-stu-id="5b313-126">path</span></span>|<span data-ttu-id="5b313-127">String</span><span class="sxs-lookup"><span data-stu-id="5b313-127">String</span></span>|<span data-ttu-id="5b313-128">Definir o caminho de um aplicativo de área de trabalho</span><span class="sxs-lookup"><span data-stu-id="5b313-128">Define the path of a desktop app</span></span>|
|<span data-ttu-id="5b313-129">Propriedadesdesktopapplicationid</span><span class="sxs-lookup"><span data-stu-id="5b313-129">desktopApplicationId</span></span>|<span data-ttu-id="5b313-130">String</span><span class="sxs-lookup"><span data-stu-id="5b313-130">String</span></span>|<span data-ttu-id="5b313-131">Definir o Propriedadesdesktopapplicationid do aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b313-131">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="5b313-132">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="5b313-132">desktopApplicationLinkPath</span></span>|<span data-ttu-id="5b313-133">String</span><span class="sxs-lookup"><span data-stu-id="5b313-133">String</span></span>|<span data-ttu-id="5b313-134">Definir o DesktopApplicationLinkPath do aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b313-134">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b313-135">Relações</span><span class="sxs-lookup"><span data-stu-id="5b313-135">Relationships</span></span>
<span data-ttu-id="5b313-136">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="5b313-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b313-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b313-137">JSON Representation</span></span>
<span data-ttu-id="5b313-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b313-138">Here is a JSON representation of the resource.</span></span>
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





