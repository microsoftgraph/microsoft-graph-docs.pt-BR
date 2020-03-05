---
title: tipo de recurso windowsKioskUWPApp
description: A classe base de um tipo de aplicativo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 840332c2873f1a42adc5a6f1ef501f411842aa32
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529015"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="497bd-103">tipo de recurso windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="497bd-103">windowsKioskUWPApp resource type</span></span>

<span data-ttu-id="497bd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="497bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="497bd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="497bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="497bd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="497bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="497bd-107">A classe base de um tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="497bd-107">The base class for a type of apps</span></span>


<span data-ttu-id="497bd-108">Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="497bd-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="497bd-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="497bd-109">Properties</span></span>
|<span data-ttu-id="497bd-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="497bd-110">Property</span></span>|<span data-ttu-id="497bd-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="497bd-111">Type</span></span>|<span data-ttu-id="497bd-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="497bd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="497bd-113">Propriedadesstartlayouttilesize</span><span class="sxs-lookup"><span data-stu-id="497bd-113">startLayoutTileSize</span></span>|[<span data-ttu-id="497bd-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="497bd-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="497bd-115">O tamanho do bloco do aplicativo para o layout inicial herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="497bd-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="497bd-116">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="497bd-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="497bd-117">nome</span><span class="sxs-lookup"><span data-stu-id="497bd-117">name</span></span>|<span data-ttu-id="497bd-118">String</span><span class="sxs-lookup"><span data-stu-id="497bd-118">String</span></span>|<span data-ttu-id="497bd-119">Representa o nome amigável de um aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="497bd-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="497bd-120">appType</span><span class="sxs-lookup"><span data-stu-id="497bd-120">appType</span></span>|[<span data-ttu-id="497bd-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="497bd-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="497bd-122">O tipo de aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="497bd-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="497bd-123">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="497bd-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="497bd-124">autolançamento</span><span class="sxs-lookup"><span data-stu-id="497bd-124">autoLaunch</span></span>|<span data-ttu-id="497bd-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="497bd-125">Boolean</span></span>|<span data-ttu-id="497bd-126">Permitir que o aplicativo seja iniciado automaticamente no modo de quiosque de vários aplicativos herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="497bd-126">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="497bd-127">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="497bd-127">appUserModelId</span></span>|<span data-ttu-id="497bd-128">String</span><span class="sxs-lookup"><span data-stu-id="497bd-128">String</span></span>|<span data-ttu-id="497bd-129">Esta é a única ID de modelo de usuário do aplicativo (AUMID) que estará disponível para iniciar o uso enquanto estiver no modo quiosque</span><span class="sxs-lookup"><span data-stu-id="497bd-129">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="497bd-130">appId</span><span class="sxs-lookup"><span data-stu-id="497bd-130">appId</span></span>|<span data-ttu-id="497bd-131">String</span><span class="sxs-lookup"><span data-stu-id="497bd-131">String</span></span>|<span data-ttu-id="497bd-132">Isso faz referência a um aplicativo do Intune que será direcionado para as mesmas atribuições como configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="497bd-132">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="497bd-133">containedAppId</span><span class="sxs-lookup"><span data-stu-id="497bd-133">containedAppId</span></span>|<span data-ttu-id="497bd-134">String</span><span class="sxs-lookup"><span data-stu-id="497bd-134">String</span></span>|<span data-ttu-id="497bd-135">Isso faz referência a um aplicativo contido de um aplicativo do Intune</span><span class="sxs-lookup"><span data-stu-id="497bd-135">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="497bd-136">Relações</span><span class="sxs-lookup"><span data-stu-id="497bd-136">Relationships</span></span>
<span data-ttu-id="497bd-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="497bd-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="497bd-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="497bd-138">JSON Representation</span></span>
<span data-ttu-id="497bd-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="497bd-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskUWPApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```



