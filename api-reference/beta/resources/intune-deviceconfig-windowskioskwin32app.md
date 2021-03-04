---
title: Tipo de recurso windowsKioskWin32App
description: Suporte a aplicativos do KioskModeApp v4 para Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d7b0dd1a5afb5dcad27bd0b2656f29336be3332d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445692"
---
# <a name="windowskioskwin32app-resource-type"></a><span data-ttu-id="ff010-103">Tipo de recurso windowsKioskWin32App</span><span class="sxs-lookup"><span data-stu-id="ff010-103">windowsKioskWin32App resource type</span></span>

<span data-ttu-id="ff010-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff010-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff010-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ff010-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff010-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff010-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff010-107">Suporte a aplicativos do KioskModeApp v4 para Win32</span><span class="sxs-lookup"><span data-stu-id="ff010-107">KioskModeApp v4 for Win32 app support</span></span>


<span data-ttu-id="ff010-108">Herda do [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="ff010-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ff010-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff010-109">Properties</span></span>
|<span data-ttu-id="ff010-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff010-110">Property</span></span>|<span data-ttu-id="ff010-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff010-111">Type</span></span>|<span data-ttu-id="ff010-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff010-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff010-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="ff010-113">startLayoutTileSize</span></span>|[<span data-ttu-id="ff010-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="ff010-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="ff010-115">O tamanho do azulejo do aplicativo para o layout inicial Herdado do [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="ff010-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="ff010-116">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="ff010-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="ff010-117">nome</span><span class="sxs-lookup"><span data-stu-id="ff010-117">name</span></span>|<span data-ttu-id="ff010-118">String</span><span class="sxs-lookup"><span data-stu-id="ff010-118">String</span></span>|<span data-ttu-id="ff010-119">Representa o nome amigável de um aplicativo Herdado do [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="ff010-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="ff010-120">appType</span><span class="sxs-lookup"><span data-stu-id="ff010-120">appType</span></span>|[<span data-ttu-id="ff010-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="ff010-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="ff010-122">O tipo de aplicativo Herdado do [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="ff010-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="ff010-123">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="ff010-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="ff010-124">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="ff010-124">autoLaunch</span></span>|<span data-ttu-id="ff010-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="ff010-125">Boolean</span></span>|<span data-ttu-id="ff010-126">Permitir que o aplicativo seja lançado automaticamente no modo de quiosque de vários aplicativos Herdado do [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="ff010-126">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="ff010-127">classicAppPath</span><span class="sxs-lookup"><span data-stu-id="ff010-127">classicAppPath</span></span>|<span data-ttu-id="ff010-128">String</span><span class="sxs-lookup"><span data-stu-id="ff010-128">String</span></span>|<span data-ttu-id="ff010-129">Este é o classicapppath a ser usado pelo aplicativo v4 Win32 enquanto estiver no modo Quiosque</span><span class="sxs-lookup"><span data-stu-id="ff010-129">This is the classicapppath to be used by v4 Win32 app while in Kiosk Mode</span></span>|
|<span data-ttu-id="ff010-130">edgeNoFirstRun</span><span class="sxs-lookup"><span data-stu-id="ff010-130">edgeNoFirstRun</span></span>|<span data-ttu-id="ff010-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="ff010-131">Boolean</span></span>|<span data-ttu-id="ff010-132">Sinalizador de primeira corrida de borda para o modo de quiosque de borda</span><span class="sxs-lookup"><span data-stu-id="ff010-132">Edge first run flag for Edge kiosk mode</span></span>|
|<span data-ttu-id="ff010-133">edgeKioskIdleTimeoutMinutes</span><span class="sxs-lookup"><span data-stu-id="ff010-133">edgeKioskIdleTimeoutMinutes</span></span>|<span data-ttu-id="ff010-134">Int32</span><span class="sxs-lookup"><span data-stu-id="ff010-134">Int32</span></span>|<span data-ttu-id="ff010-135">Tempo limite ocioso do quiosque de borda em minutos para o modo quiosque de Borda.</span><span class="sxs-lookup"><span data-stu-id="ff010-135">Edge kiosk idle timeout in minutes for Edge kiosk mode.</span></span> <span data-ttu-id="ff010-136">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="ff010-136">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="ff010-137">edgeKioskType</span><span class="sxs-lookup"><span data-stu-id="ff010-137">edgeKioskType</span></span>|[<span data-ttu-id="ff010-138">windowsEdgeKioskType</span><span class="sxs-lookup"><span data-stu-id="ff010-138">windowsEdgeKioskType</span></span>](../resources/intune-deviceconfig-windowsedgekiosktype.md)|<span data-ttu-id="ff010-139">Tipo de quiosque de borda para modo quiosque de borda.</span><span class="sxs-lookup"><span data-stu-id="ff010-139">Edge kiosk type for Edge kiosk mode.</span></span> <span data-ttu-id="ff010-140">Os valores possíveis são: `publicBrowsing` e `fullScreen`.</span><span class="sxs-lookup"><span data-stu-id="ff010-140">Possible values are: `publicBrowsing`, `fullScreen`.</span></span>|
|<span data-ttu-id="ff010-141">edgeKiosk</span><span class="sxs-lookup"><span data-stu-id="ff010-141">edgeKiosk</span></span>|<span data-ttu-id="ff010-142">String</span><span class="sxs-lookup"><span data-stu-id="ff010-142">String</span></span>|<span data-ttu-id="ff010-143">Quiosque de borda (url) para o modo de quiosque de borda</span><span class="sxs-lookup"><span data-stu-id="ff010-143">Edge kiosk (url) for Edge kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff010-144">Relações</span><span class="sxs-lookup"><span data-stu-id="ff010-144">Relationships</span></span>
<span data-ttu-id="ff010-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff010-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff010-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff010-146">JSON Representation</span></span>
<span data-ttu-id="ff010-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff010-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskWin32App"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskWin32App",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "classicAppPath": "String",
  "edgeNoFirstRun": true,
  "edgeKioskIdleTimeoutMinutes": 1024,
  "edgeKioskType": "String",
  "edgeKiosk": "String"
}
```




