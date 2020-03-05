---
title: tipo de recurso windowsKioskAppBase
description: A classe base de um tipo de aplicativo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 712c23e008e6c0b1434143383e4e8cd924ace509
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525527"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="15702-103">tipo de recurso windowsKioskAppBase</span><span class="sxs-lookup"><span data-stu-id="15702-103">windowsKioskAppBase resource type</span></span>

<span data-ttu-id="15702-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="15702-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15702-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="15702-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15702-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15702-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15702-107">A classe base de um tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="15702-107">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="15702-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="15702-108">Properties</span></span>
|<span data-ttu-id="15702-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15702-109">Property</span></span>|<span data-ttu-id="15702-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="15702-110">Type</span></span>|<span data-ttu-id="15702-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="15702-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15702-112">Propriedadesstartlayouttilesize</span><span class="sxs-lookup"><span data-stu-id="15702-112">startLayoutTileSize</span></span>|[<span data-ttu-id="15702-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="15702-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="15702-114">O tamanho do bloco do aplicativo para o layout inicial.</span><span class="sxs-lookup"><span data-stu-id="15702-114">The app tile size for the start layout.</span></span> <span data-ttu-id="15702-115">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="15702-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="15702-116">nome</span><span class="sxs-lookup"><span data-stu-id="15702-116">name</span></span>|<span data-ttu-id="15702-117">String</span><span class="sxs-lookup"><span data-stu-id="15702-117">String</span></span>|<span data-ttu-id="15702-118">Representa o nome amigável de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="15702-118">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="15702-119">appType</span><span class="sxs-lookup"><span data-stu-id="15702-119">appType</span></span>|[<span data-ttu-id="15702-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="15702-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="15702-121">O tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15702-121">The app type.</span></span> <span data-ttu-id="15702-122">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="15702-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="15702-123">autolançamento</span><span class="sxs-lookup"><span data-stu-id="15702-123">autoLaunch</span></span>|<span data-ttu-id="15702-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="15702-124">Boolean</span></span>|<span data-ttu-id="15702-125">Permitir que o aplicativo seja iniciado automaticamente no modo de quiosque de vários aplicativos</span><span class="sxs-lookup"><span data-stu-id="15702-125">Allow the app to be auto-launched in multi-app kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="15702-126">Relações</span><span class="sxs-lookup"><span data-stu-id="15702-126">Relationships</span></span>
<span data-ttu-id="15702-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="15702-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15702-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="15702-128">JSON Representation</span></span>
<span data-ttu-id="15702-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="15702-129">Here is a JSON representation of the resource.</span></span>
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



