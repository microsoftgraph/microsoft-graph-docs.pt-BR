---
title: tipo de recurso Complexowindowskioskdesktopapp
description: A classe base de um tipo de aplicativo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: af8e97b8b1aac3fcee5592da78b96bc2ccfd5143
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463461"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="d472e-103">tipo de recurso Complexowindowskioskdesktopapp</span><span class="sxs-lookup"><span data-stu-id="d472e-103">windowsKioskDesktopApp resource type</span></span>

<span data-ttu-id="d472e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d472e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d472e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d472e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d472e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d472e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d472e-107">A classe base de um tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="d472e-107">The base class for a type of apps</span></span>


<span data-ttu-id="d472e-108">Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="d472e-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d472e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d472e-109">Properties</span></span>
|<span data-ttu-id="d472e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d472e-110">Property</span></span>|<span data-ttu-id="d472e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d472e-111">Type</span></span>|<span data-ttu-id="d472e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d472e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d472e-113">Propriedadesstartlayouttilesize</span><span class="sxs-lookup"><span data-stu-id="d472e-113">startLayoutTileSize</span></span>|[<span data-ttu-id="d472e-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="d472e-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="d472e-115">O tamanho do bloco do aplicativo para o layout inicial herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="d472e-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="d472e-116">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="d472e-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="d472e-117">nome</span><span class="sxs-lookup"><span data-stu-id="d472e-117">name</span></span>|<span data-ttu-id="d472e-118">String</span><span class="sxs-lookup"><span data-stu-id="d472e-118">String</span></span>|<span data-ttu-id="d472e-119">Representa o nome amigável de um aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="d472e-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="d472e-120">appType</span><span class="sxs-lookup"><span data-stu-id="d472e-120">appType</span></span>|[<span data-ttu-id="d472e-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="d472e-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="d472e-122">O tipo de aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="d472e-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="d472e-123">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="d472e-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="d472e-124">autolançamento</span><span class="sxs-lookup"><span data-stu-id="d472e-124">autoLaunch</span></span>|<span data-ttu-id="d472e-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="d472e-125">Boolean</span></span>|<span data-ttu-id="d472e-126">Permitir que o aplicativo seja iniciado automaticamente no modo de quiosque de vários aplicativos herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="d472e-126">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="d472e-127">caminho</span><span class="sxs-lookup"><span data-stu-id="d472e-127">path</span></span>|<span data-ttu-id="d472e-128">String</span><span class="sxs-lookup"><span data-stu-id="d472e-128">String</span></span>|<span data-ttu-id="d472e-129">Definir o caminho de um aplicativo de área de trabalho</span><span class="sxs-lookup"><span data-stu-id="d472e-129">Define the path of a desktop app</span></span>|
|<span data-ttu-id="d472e-130">Propriedadesdesktopapplicationid</span><span class="sxs-lookup"><span data-stu-id="d472e-130">desktopApplicationId</span></span>|<span data-ttu-id="d472e-131">String</span><span class="sxs-lookup"><span data-stu-id="d472e-131">String</span></span>|<span data-ttu-id="d472e-132">Definir o Propriedadesdesktopapplicationid do aplicativo</span><span class="sxs-lookup"><span data-stu-id="d472e-132">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="d472e-133">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="d472e-133">desktopApplicationLinkPath</span></span>|<span data-ttu-id="d472e-134">String</span><span class="sxs-lookup"><span data-stu-id="d472e-134">String</span></span>|<span data-ttu-id="d472e-135">Definir o DesktopApplicationLinkPath do aplicativo</span><span class="sxs-lookup"><span data-stu-id="d472e-135">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="d472e-136">Relações</span><span class="sxs-lookup"><span data-stu-id="d472e-136">Relationships</span></span>
<span data-ttu-id="d472e-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d472e-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d472e-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d472e-138">JSON Representation</span></span>
<span data-ttu-id="d472e-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d472e-139">Here is a JSON representation of the resource.</span></span>
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



