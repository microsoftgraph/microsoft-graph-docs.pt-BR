---
title: tipo de recurso windowsKioskAppBase
description: A classe base de um tipo de aplicativo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 58e1339d25f615946add4ff4b9a4fe25d72dd5e4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011173"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="9c4e1-103">tipo de recurso windowsKioskAppBase</span><span class="sxs-lookup"><span data-stu-id="9c4e1-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="9c4e1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9c4e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c4e1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9c4e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c4e1-106">A classe base de um tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c4e1-106">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="9c4e1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c4e1-107">Properties</span></span>
|<span data-ttu-id="9c4e1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c4e1-108">Property</span></span>|<span data-ttu-id="9c4e1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c4e1-109">Type</span></span>|<span data-ttu-id="9c4e1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c4e1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c4e1-111">Propriedadesstartlayouttilesize</span><span class="sxs-lookup"><span data-stu-id="9c4e1-111">startLayoutTileSize</span></span>|[<span data-ttu-id="9c4e1-112">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="9c4e1-112">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="9c4e1-113">O tamanho do bloco do aplicativo para o layout inicial.</span><span class="sxs-lookup"><span data-stu-id="9c4e1-113">The app tile size for the start layout.</span></span> <span data-ttu-id="9c4e1-114">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="9c4e1-114">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="9c4e1-115">name</span><span class="sxs-lookup"><span data-stu-id="9c4e1-115">name</span></span>|<span data-ttu-id="9c4e1-116">String</span><span class="sxs-lookup"><span data-stu-id="9c4e1-116">String</span></span>|<span data-ttu-id="9c4e1-117">Representa o nome amigável de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c4e1-117">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="9c4e1-118">appType</span><span class="sxs-lookup"><span data-stu-id="9c4e1-118">appType</span></span>|[<span data-ttu-id="9c4e1-119">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="9c4e1-119">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="9c4e1-120">O tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9c4e1-120">The app type.</span></span> <span data-ttu-id="9c4e1-121">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="9c4e1-121">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="9c4e1-122">autolançamento</span><span class="sxs-lookup"><span data-stu-id="9c4e1-122">autoLaunch</span></span>|<span data-ttu-id="9c4e1-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="9c4e1-123">Boolean</span></span>|<span data-ttu-id="9c4e1-124">Permitir que o aplicativo seja iniciado automaticamente no modo de quiosque de vários aplicativos</span><span class="sxs-lookup"><span data-stu-id="9c4e1-124">Allow the app to be auto-launched in multi-app kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c4e1-125">Relações</span><span class="sxs-lookup"><span data-stu-id="9c4e1-125">Relationships</span></span>
<span data-ttu-id="9c4e1-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c4e1-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c4e1-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c4e1-127">JSON Representation</span></span>
<span data-ttu-id="9c4e1-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c4e1-128">Here is a JSON representation of the resource.</span></span>
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





