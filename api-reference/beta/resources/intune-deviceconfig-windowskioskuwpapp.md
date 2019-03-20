---
title: tipo de recurso windowsKioskUWPApp
description: A classe base de um tipo de aplicativo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a247c3f02dc64657ec9cd297d8fff5d8591549cd
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572534"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="afab7-103">tipo de recurso windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="afab7-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="afab7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="afab7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afab7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="afab7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afab7-106">A classe base de um tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="afab7-106">The base class for a type of apps</span></span>


<span data-ttu-id="afab7-107">Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="afab7-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="afab7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="afab7-108">Properties</span></span>
|<span data-ttu-id="afab7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="afab7-109">Property</span></span>|<span data-ttu-id="afab7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="afab7-110">Type</span></span>|<span data-ttu-id="afab7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="afab7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afab7-112">Propriedadesstartlayouttilesize</span><span class="sxs-lookup"><span data-stu-id="afab7-112">startLayoutTileSize</span></span>|[<span data-ttu-id="afab7-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="afab7-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="afab7-114">O tamanho do bloco do aplicativo para o layout inicial herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="afab7-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="afab7-115">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="afab7-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="afab7-116">nome</span><span class="sxs-lookup"><span data-stu-id="afab7-116">name</span></span>|<span data-ttu-id="afab7-117">String</span><span class="sxs-lookup"><span data-stu-id="afab7-117">String</span></span>|<span data-ttu-id="afab7-118">Representa o nome amigável de um aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="afab7-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="afab7-119">appType</span><span class="sxs-lookup"><span data-stu-id="afab7-119">appType</span></span>|[<span data-ttu-id="afab7-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="afab7-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="afab7-121">O tipo de aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="afab7-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="afab7-122">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="afab7-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="afab7-123">autoLançamento</span><span class="sxs-lookup"><span data-stu-id="afab7-123">autoLaunch</span></span>|<span data-ttu-id="afab7-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="afab7-124">Boolean</span></span>|<span data-ttu-id="afab7-125">Permitir que o aplicativo seja iniciado automaticamente no modo de quiosque de vários aplicativos herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="afab7-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="afab7-126">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="afab7-126">appUserModelId</span></span>|<span data-ttu-id="afab7-127">String</span><span class="sxs-lookup"><span data-stu-id="afab7-127">String</span></span>|<span data-ttu-id="afab7-128">Esta é a única ID de modelo de usuário do aplicativo (AUMID) que estará disponível para iniciar o uso enquanto estiver no modo quiosque</span><span class="sxs-lookup"><span data-stu-id="afab7-128">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="afab7-129">appId</span><span class="sxs-lookup"><span data-stu-id="afab7-129">appId</span></span>|<span data-ttu-id="afab7-130">String</span><span class="sxs-lookup"><span data-stu-id="afab7-130">String</span></span>|<span data-ttu-id="afab7-131">Isso faz referência a um aplicativo do Intune que será direcionado para as mesmas atribuições como configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="afab7-131">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="afab7-132">containedAppId</span><span class="sxs-lookup"><span data-stu-id="afab7-132">containedAppId</span></span>|<span data-ttu-id="afab7-133">String</span><span class="sxs-lookup"><span data-stu-id="afab7-133">String</span></span>|<span data-ttu-id="afab7-134">Isso faz referência a um aplicativo contido de um aplicativo do Intune</span><span class="sxs-lookup"><span data-stu-id="afab7-134">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="afab7-135">Relações</span><span class="sxs-lookup"><span data-stu-id="afab7-135">Relationships</span></span>
<span data-ttu-id="afab7-136">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="afab7-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="afab7-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="afab7-137">JSON Representation</span></span>
<span data-ttu-id="afab7-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="afab7-138">Here is a JSON representation of the resource.</span></span>
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




