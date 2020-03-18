---
title: tipo de recurso windowsKioskAppBase
description: A classe base de um tipo de aplicativo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d3ba4a27f1107b35264d1671530b5314ea28026c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786443"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="447c9-103">tipo de recurso windowsKioskAppBase</span><span class="sxs-lookup"><span data-stu-id="447c9-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="447c9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="447c9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="447c9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="447c9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="447c9-106">A classe base de um tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="447c9-106">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="447c9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="447c9-107">Properties</span></span>
|<span data-ttu-id="447c9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="447c9-108">Property</span></span>|<span data-ttu-id="447c9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="447c9-109">Type</span></span>|<span data-ttu-id="447c9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="447c9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="447c9-111">Propriedadesstartlayouttilesize</span><span class="sxs-lookup"><span data-stu-id="447c9-111">startLayoutTileSize</span></span>|[<span data-ttu-id="447c9-112">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="447c9-112">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="447c9-113">O tamanho do bloco do aplicativo para o layout inicial.</span><span class="sxs-lookup"><span data-stu-id="447c9-113">The app tile size for the start layout.</span></span> <span data-ttu-id="447c9-114">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="447c9-114">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="447c9-115">nome</span><span class="sxs-lookup"><span data-stu-id="447c9-115">name</span></span>|<span data-ttu-id="447c9-116">String</span><span class="sxs-lookup"><span data-stu-id="447c9-116">String</span></span>|<span data-ttu-id="447c9-117">Representa o nome amigável de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="447c9-117">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="447c9-118">appType</span><span class="sxs-lookup"><span data-stu-id="447c9-118">appType</span></span>|[<span data-ttu-id="447c9-119">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="447c9-119">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="447c9-120">O tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="447c9-120">The app type.</span></span> <span data-ttu-id="447c9-121">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="447c9-121">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="447c9-122">autolançamento</span><span class="sxs-lookup"><span data-stu-id="447c9-122">autoLaunch</span></span>|<span data-ttu-id="447c9-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="447c9-123">Boolean</span></span>|<span data-ttu-id="447c9-124">Permitir que o aplicativo seja iniciado automaticamente no modo de quiosque de vários aplicativos</span><span class="sxs-lookup"><span data-stu-id="447c9-124">Allow the app to be auto-launched in multi-app kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="447c9-125">Relações</span><span class="sxs-lookup"><span data-stu-id="447c9-125">Relationships</span></span>
<span data-ttu-id="447c9-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="447c9-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="447c9-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="447c9-127">JSON Representation</span></span>
<span data-ttu-id="447c9-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="447c9-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAppBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAppBase",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true
}
```



