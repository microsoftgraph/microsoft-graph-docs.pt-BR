---
title: tipo de recurso macOSLaunchItem
description: Representa um aplicativo na lista de itens de lançamento do macOS
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1317f2d42c21d0d11d45290696f183c679b049e1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809145"
---
# <a name="macoslaunchitem-resource-type"></a><span data-ttu-id="ebc02-103">tipo de recurso macOSLaunchItem</span><span class="sxs-lookup"><span data-stu-id="ebc02-103">macOSLaunchItem resource type</span></span>

> <span data-ttu-id="ebc02-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ebc02-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebc02-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ebc02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebc02-106">Representa um aplicativo na lista de itens de lançamento do macOS</span><span class="sxs-lookup"><span data-stu-id="ebc02-106">Represents an app in the list of macOS launch items</span></span>

## <a name="properties"></a><span data-ttu-id="ebc02-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ebc02-107">Properties</span></span>
|<span data-ttu-id="ebc02-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebc02-108">Property</span></span>|<span data-ttu-id="ebc02-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebc02-109">Type</span></span>|<span data-ttu-id="ebc02-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebc02-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebc02-111">caminho</span><span class="sxs-lookup"><span data-stu-id="ebc02-111">path</span></span>|<span data-ttu-id="ebc02-112">String</span><span class="sxs-lookup"><span data-stu-id="ebc02-112">String</span></span>|<span data-ttu-id="ebc02-113">Caminho para o item de lançamento.</span><span class="sxs-lookup"><span data-stu-id="ebc02-113">Path to the launch item.</span></span>|
|<span data-ttu-id="ebc02-114">ocult</span><span class="sxs-lookup"><span data-stu-id="ebc02-114">hide</span></span>|<span data-ttu-id="ebc02-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="ebc02-115">Boolean</span></span>|<span data-ttu-id="ebc02-116">Se o item será ou não ocultado da lista usuários e grupos.</span><span class="sxs-lookup"><span data-stu-id="ebc02-116">Whether or not to hide the item from the Users and Groups List.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebc02-117">Relações</span><span class="sxs-lookup"><span data-stu-id="ebc02-117">Relationships</span></span>
<span data-ttu-id="ebc02-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ebc02-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebc02-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ebc02-119">JSON Representation</span></span>
<span data-ttu-id="ebc02-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ebc02-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLaunchItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLaunchItem",
  "path": "String",
  "hide": true
}
```





