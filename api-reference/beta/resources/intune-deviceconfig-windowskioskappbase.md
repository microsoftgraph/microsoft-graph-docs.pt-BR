---
title: tipo de recurso de windowsKioskAppBase
description: A classe base para um tipo de aplicativos
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8ca86969eb32a1a1d129fb5ba4cd48bbb04ffd78
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407141"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="ee165-103">tipo de recurso de windowsKioskAppBase</span><span class="sxs-lookup"><span data-stu-id="ee165-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="ee165-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ee165-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ee165-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ee165-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee165-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ee165-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee165-107">A classe base para um tipo de aplicativos</span><span class="sxs-lookup"><span data-stu-id="ee165-107">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="ee165-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee165-108">Properties</span></span>
|<span data-ttu-id="ee165-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee165-109">Property</span></span>|<span data-ttu-id="ee165-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee165-110">Type</span></span>|<span data-ttu-id="ee165-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee165-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee165-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="ee165-112">startLayoutTileSize</span></span>|[<span data-ttu-id="ee165-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="ee165-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="ee165-114">O tamanho de blocos de aplicativo para o layout de iniciar.</span><span class="sxs-lookup"><span data-stu-id="ee165-114">The app tile size for the start layout.</span></span> <span data-ttu-id="ee165-115">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="ee165-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="ee165-116">name</span><span class="sxs-lookup"><span data-stu-id="ee165-116">name</span></span>|<span data-ttu-id="ee165-117">String</span><span class="sxs-lookup"><span data-stu-id="ee165-117">String</span></span>|<span data-ttu-id="ee165-118">Representa o nome amigável de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee165-118">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="ee165-119">tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee165-119">appType</span></span>|[<span data-ttu-id="ee165-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="ee165-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="ee165-121">O tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ee165-121">The app type.</span></span> <span data-ttu-id="ee165-122">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="ee165-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee165-123">Relações</span><span class="sxs-lookup"><span data-stu-id="ee165-123">Relationships</span></span>
<span data-ttu-id="ee165-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee165-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee165-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee165-125">JSON Representation</span></span>
<span data-ttu-id="ee165-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee165-126">Here is a JSON representation of the resource.</span></span>
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
  "appType": "String"
}
```




