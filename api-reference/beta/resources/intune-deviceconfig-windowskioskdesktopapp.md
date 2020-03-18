---
title: tipo de recurso Complexowindowskioskdesktopapp
description: A classe base de um tipo de aplicativo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f940a656395a58df4487648a2090455b97d1647b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786387"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="08eac-103">tipo de recurso Complexowindowskioskdesktopapp</span><span class="sxs-lookup"><span data-stu-id="08eac-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="08eac-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="08eac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08eac-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08eac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08eac-106">A classe base de um tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="08eac-106">The base class for a type of apps</span></span>


<span data-ttu-id="08eac-107">Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="08eac-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="08eac-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08eac-108">Properties</span></span>
|<span data-ttu-id="08eac-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08eac-109">Property</span></span>|<span data-ttu-id="08eac-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="08eac-110">Type</span></span>|<span data-ttu-id="08eac-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="08eac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08eac-112">Propriedadesstartlayouttilesize</span><span class="sxs-lookup"><span data-stu-id="08eac-112">startLayoutTileSize</span></span>|[<span data-ttu-id="08eac-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="08eac-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="08eac-114">O tamanho do bloco do aplicativo para o layout inicial herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="08eac-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="08eac-115">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="08eac-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="08eac-116">nome</span><span class="sxs-lookup"><span data-stu-id="08eac-116">name</span></span>|<span data-ttu-id="08eac-117">String</span><span class="sxs-lookup"><span data-stu-id="08eac-117">String</span></span>|<span data-ttu-id="08eac-118">Representa o nome amigável de um aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="08eac-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="08eac-119">appType</span><span class="sxs-lookup"><span data-stu-id="08eac-119">appType</span></span>|[<span data-ttu-id="08eac-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="08eac-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="08eac-121">O tipo de aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="08eac-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="08eac-122">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="08eac-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="08eac-123">autolançamento</span><span class="sxs-lookup"><span data-stu-id="08eac-123">autoLaunch</span></span>|<span data-ttu-id="08eac-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="08eac-124">Boolean</span></span>|<span data-ttu-id="08eac-125">Permitir que o aplicativo seja iniciado automaticamente no modo de quiosque de vários aplicativos herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="08eac-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="08eac-126">caminho</span><span class="sxs-lookup"><span data-stu-id="08eac-126">path</span></span>|<span data-ttu-id="08eac-127">String</span><span class="sxs-lookup"><span data-stu-id="08eac-127">String</span></span>|<span data-ttu-id="08eac-128">Definir o caminho de um aplicativo de área de trabalho</span><span class="sxs-lookup"><span data-stu-id="08eac-128">Define the path of a desktop app</span></span>|
|<span data-ttu-id="08eac-129">Propriedadesdesktopapplicationid</span><span class="sxs-lookup"><span data-stu-id="08eac-129">desktopApplicationId</span></span>|<span data-ttu-id="08eac-130">String</span><span class="sxs-lookup"><span data-stu-id="08eac-130">String</span></span>|<span data-ttu-id="08eac-131">Definir o Propriedadesdesktopapplicationid do aplicativo</span><span class="sxs-lookup"><span data-stu-id="08eac-131">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="08eac-132">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="08eac-132">desktopApplicationLinkPath</span></span>|<span data-ttu-id="08eac-133">String</span><span class="sxs-lookup"><span data-stu-id="08eac-133">String</span></span>|<span data-ttu-id="08eac-134">Definir o DesktopApplicationLinkPath do aplicativo</span><span class="sxs-lookup"><span data-stu-id="08eac-134">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="08eac-135">Relações</span><span class="sxs-lookup"><span data-stu-id="08eac-135">Relationships</span></span>
<span data-ttu-id="08eac-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08eac-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08eac-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08eac-137">JSON Representation</span></span>
<span data-ttu-id="08eac-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08eac-138">Here is a JSON representation of the resource.</span></span>
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



