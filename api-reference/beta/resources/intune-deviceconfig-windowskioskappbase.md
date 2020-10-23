---
title: tipo de recurso windowsKioskAppBase
description: A classe base de um tipo de aplicativo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4212dfd0362ed6253c10a2b2796241c74678dda2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736209"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="b08aa-103">tipo de recurso windowsKioskAppBase</span><span class="sxs-lookup"><span data-stu-id="b08aa-103">windowsKioskAppBase resource type</span></span>

<span data-ttu-id="b08aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b08aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b08aa-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b08aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b08aa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b08aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b08aa-107">A classe base de um tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="b08aa-107">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="b08aa-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b08aa-108">Properties</span></span>
|<span data-ttu-id="b08aa-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b08aa-109">Property</span></span>|<span data-ttu-id="b08aa-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b08aa-110">Type</span></span>|<span data-ttu-id="b08aa-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b08aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b08aa-112">Propriedadesstartlayouttilesize</span><span class="sxs-lookup"><span data-stu-id="b08aa-112">startLayoutTileSize</span></span>|[<span data-ttu-id="b08aa-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="b08aa-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="b08aa-114">O tamanho do bloco do aplicativo para o layout inicial.</span><span class="sxs-lookup"><span data-stu-id="b08aa-114">The app tile size for the start layout.</span></span> <span data-ttu-id="b08aa-115">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="b08aa-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="b08aa-116">nome</span><span class="sxs-lookup"><span data-stu-id="b08aa-116">name</span></span>|<span data-ttu-id="b08aa-117">String</span><span class="sxs-lookup"><span data-stu-id="b08aa-117">String</span></span>|<span data-ttu-id="b08aa-118">Representa o nome amigável de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="b08aa-118">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="b08aa-119">appType</span><span class="sxs-lookup"><span data-stu-id="b08aa-119">appType</span></span>|[<span data-ttu-id="b08aa-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="b08aa-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="b08aa-121">O tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b08aa-121">The app type.</span></span> <span data-ttu-id="b08aa-122">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="b08aa-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="b08aa-123">autolançamento</span><span class="sxs-lookup"><span data-stu-id="b08aa-123">autoLaunch</span></span>|<span data-ttu-id="b08aa-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="b08aa-124">Boolean</span></span>|<span data-ttu-id="b08aa-125">Permitir que o aplicativo seja iniciado automaticamente no modo de quiosque de vários aplicativos</span><span class="sxs-lookup"><span data-stu-id="b08aa-125">Allow the app to be auto-launched in multi-app kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="b08aa-126">Relações</span><span class="sxs-lookup"><span data-stu-id="b08aa-126">Relationships</span></span>
<span data-ttu-id="b08aa-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b08aa-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b08aa-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b08aa-128">JSON Representation</span></span>
<span data-ttu-id="b08aa-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b08aa-129">Here is a JSON representation of the resource.</span></span>
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





