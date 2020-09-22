---
title: tipo de recurso Complexowindowskioskdesktopapp
description: A classe base de um tipo de aplicativo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 145cc54d3d04a3a703ad65f5ee91a71df7bb63ab
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039780"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="d7f60-103">tipo de recurso Complexowindowskioskdesktopapp</span><span class="sxs-lookup"><span data-stu-id="d7f60-103">windowsKioskDesktopApp resource type</span></span>

<span data-ttu-id="d7f60-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7f60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7f60-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d7f60-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7f60-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d7f60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7f60-107">A classe base de um tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7f60-107">The base class for a type of apps</span></span>


<span data-ttu-id="d7f60-108">Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="d7f60-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d7f60-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7f60-109">Properties</span></span>
|<span data-ttu-id="d7f60-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7f60-110">Property</span></span>|<span data-ttu-id="d7f60-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7f60-111">Type</span></span>|<span data-ttu-id="d7f60-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7f60-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7f60-113">Propriedadesstartlayouttilesize</span><span class="sxs-lookup"><span data-stu-id="d7f60-113">startLayoutTileSize</span></span>|[<span data-ttu-id="d7f60-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="d7f60-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="d7f60-115">O tamanho do bloco do aplicativo para o layout inicial herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="d7f60-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="d7f60-116">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="d7f60-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="d7f60-117">nome</span><span class="sxs-lookup"><span data-stu-id="d7f60-117">name</span></span>|<span data-ttu-id="d7f60-118">String</span><span class="sxs-lookup"><span data-stu-id="d7f60-118">String</span></span>|<span data-ttu-id="d7f60-119">Representa o nome amigável de um aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="d7f60-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="d7f60-120">appType</span><span class="sxs-lookup"><span data-stu-id="d7f60-120">appType</span></span>|[<span data-ttu-id="d7f60-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="d7f60-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="d7f60-122">O tipo de aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="d7f60-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="d7f60-123">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="d7f60-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="d7f60-124">autolançamento</span><span class="sxs-lookup"><span data-stu-id="d7f60-124">autoLaunch</span></span>|<span data-ttu-id="d7f60-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="d7f60-125">Boolean</span></span>|<span data-ttu-id="d7f60-126">Permitir que o aplicativo seja iniciado automaticamente no modo de quiosque de vários aplicativos herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="d7f60-126">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="d7f60-127">caminho</span><span class="sxs-lookup"><span data-stu-id="d7f60-127">path</span></span>|<span data-ttu-id="d7f60-128">String</span><span class="sxs-lookup"><span data-stu-id="d7f60-128">String</span></span>|<span data-ttu-id="d7f60-129">Definir o caminho de um aplicativo de área de trabalho</span><span class="sxs-lookup"><span data-stu-id="d7f60-129">Define the path of a desktop app</span></span>|
|<span data-ttu-id="d7f60-130">Propriedadesdesktopapplicationid</span><span class="sxs-lookup"><span data-stu-id="d7f60-130">desktopApplicationId</span></span>|<span data-ttu-id="d7f60-131">String</span><span class="sxs-lookup"><span data-stu-id="d7f60-131">String</span></span>|<span data-ttu-id="d7f60-132">Definir o Propriedadesdesktopapplicationid do aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7f60-132">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="d7f60-133">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="d7f60-133">desktopApplicationLinkPath</span></span>|<span data-ttu-id="d7f60-134">String</span><span class="sxs-lookup"><span data-stu-id="d7f60-134">String</span></span>|<span data-ttu-id="d7f60-135">Definir o DesktopApplicationLinkPath do aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7f60-135">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7f60-136">Relações</span><span class="sxs-lookup"><span data-stu-id="d7f60-136">Relationships</span></span>
<span data-ttu-id="d7f60-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d7f60-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7f60-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7f60-138">JSON Representation</span></span>
<span data-ttu-id="d7f60-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d7f60-139">Here is a JSON representation of the resource.</span></span>
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






