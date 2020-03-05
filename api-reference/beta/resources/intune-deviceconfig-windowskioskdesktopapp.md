---
title: tipo de recurso Complexowindowskioskdesktopapp
description: A classe base de um tipo de aplicativo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7df38deba11cae5199a781a38dda6cd4b5abb698
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529031"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="934fd-103">tipo de recurso Complexowindowskioskdesktopapp</span><span class="sxs-lookup"><span data-stu-id="934fd-103">windowsKioskDesktopApp resource type</span></span>

<span data-ttu-id="934fd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="934fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="934fd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="934fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="934fd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="934fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="934fd-107">A classe base de um tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="934fd-107">The base class for a type of apps</span></span>


<span data-ttu-id="934fd-108">Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="934fd-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="934fd-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="934fd-109">Properties</span></span>
|<span data-ttu-id="934fd-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="934fd-110">Property</span></span>|<span data-ttu-id="934fd-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="934fd-111">Type</span></span>|<span data-ttu-id="934fd-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="934fd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="934fd-113">Propriedadesstartlayouttilesize</span><span class="sxs-lookup"><span data-stu-id="934fd-113">startLayoutTileSize</span></span>|[<span data-ttu-id="934fd-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="934fd-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="934fd-115">O tamanho do bloco do aplicativo para o layout inicial herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="934fd-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="934fd-116">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="934fd-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="934fd-117">nome</span><span class="sxs-lookup"><span data-stu-id="934fd-117">name</span></span>|<span data-ttu-id="934fd-118">String</span><span class="sxs-lookup"><span data-stu-id="934fd-118">String</span></span>|<span data-ttu-id="934fd-119">Representa o nome amigável de um aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="934fd-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="934fd-120">appType</span><span class="sxs-lookup"><span data-stu-id="934fd-120">appType</span></span>|[<span data-ttu-id="934fd-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="934fd-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="934fd-122">O tipo de aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="934fd-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="934fd-123">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="934fd-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="934fd-124">autolançamento</span><span class="sxs-lookup"><span data-stu-id="934fd-124">autoLaunch</span></span>|<span data-ttu-id="934fd-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="934fd-125">Boolean</span></span>|<span data-ttu-id="934fd-126">Permitir que o aplicativo seja iniciado automaticamente no modo de quiosque de vários aplicativos herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="934fd-126">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="934fd-127">caminho</span><span class="sxs-lookup"><span data-stu-id="934fd-127">path</span></span>|<span data-ttu-id="934fd-128">String</span><span class="sxs-lookup"><span data-stu-id="934fd-128">String</span></span>|<span data-ttu-id="934fd-129">Definir o caminho de um aplicativo de área de trabalho</span><span class="sxs-lookup"><span data-stu-id="934fd-129">Define the path of a desktop app</span></span>|
|<span data-ttu-id="934fd-130">Propriedadesdesktopapplicationid</span><span class="sxs-lookup"><span data-stu-id="934fd-130">desktopApplicationId</span></span>|<span data-ttu-id="934fd-131">String</span><span class="sxs-lookup"><span data-stu-id="934fd-131">String</span></span>|<span data-ttu-id="934fd-132">Definir o Propriedadesdesktopapplicationid do aplicativo</span><span class="sxs-lookup"><span data-stu-id="934fd-132">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="934fd-133">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="934fd-133">desktopApplicationLinkPath</span></span>|<span data-ttu-id="934fd-134">String</span><span class="sxs-lookup"><span data-stu-id="934fd-134">String</span></span>|<span data-ttu-id="934fd-135">Definir o DesktopApplicationLinkPath do aplicativo</span><span class="sxs-lookup"><span data-stu-id="934fd-135">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="934fd-136">Relações</span><span class="sxs-lookup"><span data-stu-id="934fd-136">Relationships</span></span>
<span data-ttu-id="934fd-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="934fd-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="934fd-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="934fd-138">JSON Representation</span></span>
<span data-ttu-id="934fd-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="934fd-139">Here is a JSON representation of the resource.</span></span>
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



