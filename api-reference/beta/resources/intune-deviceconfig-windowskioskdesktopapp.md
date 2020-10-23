---
title: tipo de recurso Complexowindowskioskdesktopapp
description: A classe base de um tipo de aplicativo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 82773d7bedc5bb4221327217195e98e12621dfde
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729536"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="56c02-103">tipo de recurso Complexowindowskioskdesktopapp</span><span class="sxs-lookup"><span data-stu-id="56c02-103">windowsKioskDesktopApp resource type</span></span>

<span data-ttu-id="56c02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56c02-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56c02-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="56c02-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56c02-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="56c02-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56c02-107">A classe base de um tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="56c02-107">The base class for a type of apps</span></span>


<span data-ttu-id="56c02-108">Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="56c02-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="56c02-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56c02-109">Properties</span></span>
|<span data-ttu-id="56c02-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56c02-110">Property</span></span>|<span data-ttu-id="56c02-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="56c02-111">Type</span></span>|<span data-ttu-id="56c02-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="56c02-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56c02-113">Propriedadesstartlayouttilesize</span><span class="sxs-lookup"><span data-stu-id="56c02-113">startLayoutTileSize</span></span>|[<span data-ttu-id="56c02-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="56c02-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="56c02-115">O tamanho do bloco do aplicativo para o layout inicial herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="56c02-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="56c02-116">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="56c02-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="56c02-117">nome</span><span class="sxs-lookup"><span data-stu-id="56c02-117">name</span></span>|<span data-ttu-id="56c02-118">String</span><span class="sxs-lookup"><span data-stu-id="56c02-118">String</span></span>|<span data-ttu-id="56c02-119">Representa o nome amigável de um aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="56c02-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="56c02-120">appType</span><span class="sxs-lookup"><span data-stu-id="56c02-120">appType</span></span>|[<span data-ttu-id="56c02-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="56c02-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="56c02-122">O tipo de aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="56c02-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="56c02-123">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="56c02-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="56c02-124">autolançamento</span><span class="sxs-lookup"><span data-stu-id="56c02-124">autoLaunch</span></span>|<span data-ttu-id="56c02-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="56c02-125">Boolean</span></span>|<span data-ttu-id="56c02-126">Permitir que o aplicativo seja iniciado automaticamente no modo de quiosque de vários aplicativos herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="56c02-126">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="56c02-127">caminho</span><span class="sxs-lookup"><span data-stu-id="56c02-127">path</span></span>|<span data-ttu-id="56c02-128">String</span><span class="sxs-lookup"><span data-stu-id="56c02-128">String</span></span>|<span data-ttu-id="56c02-129">Definir o caminho de um aplicativo de área de trabalho</span><span class="sxs-lookup"><span data-stu-id="56c02-129">Define the path of a desktop app</span></span>|
|<span data-ttu-id="56c02-130">Propriedadesdesktopapplicationid</span><span class="sxs-lookup"><span data-stu-id="56c02-130">desktopApplicationId</span></span>|<span data-ttu-id="56c02-131">String</span><span class="sxs-lookup"><span data-stu-id="56c02-131">String</span></span>|<span data-ttu-id="56c02-132">Definir o Propriedadesdesktopapplicationid do aplicativo</span><span class="sxs-lookup"><span data-stu-id="56c02-132">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="56c02-133">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="56c02-133">desktopApplicationLinkPath</span></span>|<span data-ttu-id="56c02-134">String</span><span class="sxs-lookup"><span data-stu-id="56c02-134">String</span></span>|<span data-ttu-id="56c02-135">Definir o DesktopApplicationLinkPath do aplicativo</span><span class="sxs-lookup"><span data-stu-id="56c02-135">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="56c02-136">Relações</span><span class="sxs-lookup"><span data-stu-id="56c02-136">Relationships</span></span>
<span data-ttu-id="56c02-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="56c02-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56c02-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56c02-138">JSON Representation</span></span>
<span data-ttu-id="56c02-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="56c02-139">Here is a JSON representation of the resource.</span></span>
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





