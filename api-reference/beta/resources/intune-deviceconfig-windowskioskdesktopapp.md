---
title: tipo de recurso de windowsKioskDesktopApp
description: A classe base para um tipo de aplicativos
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 831ed86da24791cde549687ecaff42cabc29a99e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415303"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="1ac93-103">tipo de recurso de windowsKioskDesktopApp</span><span class="sxs-lookup"><span data-stu-id="1ac93-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="1ac93-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="1ac93-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1ac93-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1ac93-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ac93-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="1ac93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ac93-107">A classe base para um tipo de aplicativos</span><span class="sxs-lookup"><span data-stu-id="1ac93-107">The base class for a type of apps</span></span>


<span data-ttu-id="1ac93-108">Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="1ac93-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1ac93-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ac93-109">Properties</span></span>
|<span data-ttu-id="1ac93-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ac93-110">Property</span></span>|<span data-ttu-id="1ac93-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ac93-111">Type</span></span>|<span data-ttu-id="1ac93-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ac93-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ac93-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="1ac93-113">startLayoutTileSize</span></span>|[<span data-ttu-id="1ac93-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="1ac93-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="1ac93-115">O tamanho de blocos de aplicativo para o layout de iniciar Inherited de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="1ac93-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="1ac93-116">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="1ac93-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="1ac93-117">name</span><span class="sxs-lookup"><span data-stu-id="1ac93-117">name</span></span>|<span data-ttu-id="1ac93-118">String</span><span class="sxs-lookup"><span data-stu-id="1ac93-118">String</span></span>|<span data-ttu-id="1ac93-119">Representa o nome amigável de um aplicativo Inherited de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="1ac93-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="1ac93-120">tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ac93-120">appType</span></span>|[<span data-ttu-id="1ac93-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="1ac93-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="1ac93-122">O tipo de app Inherited da [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="1ac93-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="1ac93-123">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="1ac93-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="1ac93-124">caminho</span><span class="sxs-lookup"><span data-stu-id="1ac93-124">path</span></span>|<span data-ttu-id="1ac93-125">String</span><span class="sxs-lookup"><span data-stu-id="1ac93-125">String</span></span>|<span data-ttu-id="1ac93-126">Definir o caminho de um aplicativo de área de trabalho</span><span class="sxs-lookup"><span data-stu-id="1ac93-126">Define the path of a desktop app</span></span>|
|<span data-ttu-id="1ac93-127">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="1ac93-127">desktopApplicationId</span></span>|<span data-ttu-id="1ac93-128">String</span><span class="sxs-lookup"><span data-stu-id="1ac93-128">String</span></span>|<span data-ttu-id="1ac93-129">Definir o DesktopApplicationID do aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ac93-129">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="1ac93-130">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="1ac93-130">desktopApplicationLinkPath</span></span>|<span data-ttu-id="1ac93-131">String</span><span class="sxs-lookup"><span data-stu-id="1ac93-131">String</span></span>|<span data-ttu-id="1ac93-132">Definir o DesktopApplicationLinkPath do aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ac93-132">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ac93-133">Relações</span><span class="sxs-lookup"><span data-stu-id="1ac93-133">Relationships</span></span>
<span data-ttu-id="1ac93-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ac93-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ac93-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ac93-135">JSON Representation</span></span>
<span data-ttu-id="1ac93-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ac93-136">Here is a JSON representation of the resource.</span></span>
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
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```




