---
title: tipo de recurso de windowsKioskDesktopApp
description: A classe base para um tipo de aplicativos
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a9b808bfd67e1b14e0b11fe84da48b77b4d965ba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947327"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="e68a6-103">tipo de recurso de windowsKioskDesktopApp</span><span class="sxs-lookup"><span data-stu-id="e68a6-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="e68a6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e68a6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e68a6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e68a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e68a6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e68a6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e68a6-107">A classe base para um tipo de aplicativos</span><span class="sxs-lookup"><span data-stu-id="e68a6-107">The base class for a type of apps</span></span>

<span data-ttu-id="e68a6-108">Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="e68a6-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e68a6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e68a6-109">Properties</span></span>
|<span data-ttu-id="e68a6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e68a6-110">Property</span></span>|<span data-ttu-id="e68a6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e68a6-111">Type</span></span>|<span data-ttu-id="e68a6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e68a6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e68a6-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="e68a6-113">startLayoutTileSize</span></span>|[<span data-ttu-id="e68a6-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="e68a6-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="e68a6-115">O tamanho de blocos de aplicativo para o layout de iniciar Inherited de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="e68a6-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="e68a6-116">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="e68a6-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="e68a6-117">name</span><span class="sxs-lookup"><span data-stu-id="e68a6-117">name</span></span>|<span data-ttu-id="e68a6-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e68a6-118">String</span></span>|<span data-ttu-id="e68a6-119">Representa o nome amigável de um aplicativo Inherited de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="e68a6-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="e68a6-120">caminho</span><span class="sxs-lookup"><span data-stu-id="e68a6-120">path</span></span>|<span data-ttu-id="e68a6-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e68a6-121">String</span></span>|<span data-ttu-id="e68a6-122">Definir o caminho de um aplicativo de área de trabalho</span><span class="sxs-lookup"><span data-stu-id="e68a6-122">Define the path of a desktop app</span></span>|
|<span data-ttu-id="e68a6-123">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="e68a6-123">desktopApplicationId</span></span>|<span data-ttu-id="e68a6-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e68a6-124">String</span></span>|<span data-ttu-id="e68a6-125">Definir o DesktopApplicationID do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e68a6-125">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="e68a6-126">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="e68a6-126">desktopApplicationLinkPath</span></span>|<span data-ttu-id="e68a6-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e68a6-127">String</span></span>|<span data-ttu-id="e68a6-128">Definir o DesktopApplicationLinkPath do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e68a6-128">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="e68a6-129">Relações</span><span class="sxs-lookup"><span data-stu-id="e68a6-129">Relationships</span></span>
<span data-ttu-id="e68a6-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e68a6-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e68a6-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e68a6-131">JSON Representation</span></span>
<span data-ttu-id="e68a6-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e68a6-132">Here is a JSON representation of the resource.</span></span>
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
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```





