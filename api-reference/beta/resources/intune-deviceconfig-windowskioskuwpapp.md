---
title: tipo de recurso windowsKioskUWPApp
description: A classe base de um tipo de aplicativo
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9340006ee74e640e21dc6bef99cc1f0e297999b9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943771"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="3b6ed-103">tipo de recurso windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="3b6ed-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="3b6ed-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b6ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b6ed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b6ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b6ed-106">A classe base de um tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b6ed-106">The base class for a type of apps</span></span>


<span data-ttu-id="3b6ed-107">Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="3b6ed-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3b6ed-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b6ed-108">Properties</span></span>
|<span data-ttu-id="3b6ed-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b6ed-109">Property</span></span>|<span data-ttu-id="3b6ed-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b6ed-110">Type</span></span>|<span data-ttu-id="3b6ed-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b6ed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b6ed-112">Propriedadesstartlayouttilesize</span><span class="sxs-lookup"><span data-stu-id="3b6ed-112">startLayoutTileSize</span></span>|[<span data-ttu-id="3b6ed-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="3b6ed-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="3b6ed-114">O tamanho do bloco do aplicativo para o layout inicial herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="3b6ed-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="3b6ed-115">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="3b6ed-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="3b6ed-116">nome</span><span class="sxs-lookup"><span data-stu-id="3b6ed-116">name</span></span>|<span data-ttu-id="3b6ed-117">String</span><span class="sxs-lookup"><span data-stu-id="3b6ed-117">String</span></span>|<span data-ttu-id="3b6ed-118">Representa o nome amigável de um aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="3b6ed-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="3b6ed-119">appType</span><span class="sxs-lookup"><span data-stu-id="3b6ed-119">appType</span></span>|[<span data-ttu-id="3b6ed-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="3b6ed-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="3b6ed-121">O tipo de aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="3b6ed-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="3b6ed-122">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="3b6ed-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="3b6ed-123">autolançamento</span><span class="sxs-lookup"><span data-stu-id="3b6ed-123">autoLaunch</span></span>|<span data-ttu-id="3b6ed-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b6ed-124">Boolean</span></span>|<span data-ttu-id="3b6ed-125">Permitir que o aplicativo seja iniciado automaticamente no modo de quiosque de vários aplicativos herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="3b6ed-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="3b6ed-126">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="3b6ed-126">appUserModelId</span></span>|<span data-ttu-id="3b6ed-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b6ed-127">String</span></span>|<span data-ttu-id="3b6ed-128">Esta é a única ID de modelo de usuário do aplicativo (AUMID) que estará disponível para iniciar o uso enquanto estiver no modo quiosque</span><span class="sxs-lookup"><span data-stu-id="3b6ed-128">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="3b6ed-129">appId</span><span class="sxs-lookup"><span data-stu-id="3b6ed-129">appId</span></span>|<span data-ttu-id="3b6ed-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b6ed-130">String</span></span>|<span data-ttu-id="3b6ed-131">Isso faz referência a um aplicativo do Intune que será direcionado para as mesmas atribuições como configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="3b6ed-131">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="3b6ed-132">containedAppId</span><span class="sxs-lookup"><span data-stu-id="3b6ed-132">containedAppId</span></span>|<span data-ttu-id="3b6ed-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b6ed-133">String</span></span>|<span data-ttu-id="3b6ed-134">Isso faz referência a um aplicativo contido de um aplicativo do Intune</span><span class="sxs-lookup"><span data-stu-id="3b6ed-134">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b6ed-135">Relações</span><span class="sxs-lookup"><span data-stu-id="3b6ed-135">Relationships</span></span>
<span data-ttu-id="3b6ed-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3b6ed-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b6ed-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b6ed-137">JSON Representation</span></span>
<span data-ttu-id="3b6ed-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3b6ed-138">Here is a JSON representation of the resource.</span></span>
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




