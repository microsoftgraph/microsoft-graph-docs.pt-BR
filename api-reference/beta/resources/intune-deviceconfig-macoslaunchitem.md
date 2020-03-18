---
title: tipo de recurso macOSLaunchItem
description: Representa um aplicativo na lista de itens de lançamento do macOS
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 378b2e3f510d8d0db082e3843ea2588e5a5e161d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42789203"
---
# <a name="macoslaunchitem-resource-type"></a><span data-ttu-id="e5cc2-103">tipo de recurso macOSLaunchItem</span><span class="sxs-lookup"><span data-stu-id="e5cc2-103">macOSLaunchItem resource type</span></span>

> <span data-ttu-id="e5cc2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e5cc2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5cc2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5cc2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5cc2-106">Representa um aplicativo na lista de itens de lançamento do macOS</span><span class="sxs-lookup"><span data-stu-id="e5cc2-106">Represents an app in the list of macOS launch items</span></span>

## <a name="properties"></a><span data-ttu-id="e5cc2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5cc2-107">Properties</span></span>
|<span data-ttu-id="e5cc2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5cc2-108">Property</span></span>|<span data-ttu-id="e5cc2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5cc2-109">Type</span></span>|<span data-ttu-id="e5cc2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5cc2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5cc2-111">caminho</span><span class="sxs-lookup"><span data-stu-id="e5cc2-111">path</span></span>|<span data-ttu-id="e5cc2-112">String</span><span class="sxs-lookup"><span data-stu-id="e5cc2-112">String</span></span>|<span data-ttu-id="e5cc2-113">Caminho para o item de lançamento.</span><span class="sxs-lookup"><span data-stu-id="e5cc2-113">Path to the launch item.</span></span>|
|<span data-ttu-id="e5cc2-114">ocult</span><span class="sxs-lookup"><span data-stu-id="e5cc2-114">hide</span></span>|<span data-ttu-id="e5cc2-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5cc2-115">Boolean</span></span>|<span data-ttu-id="e5cc2-116">Se o item será ou não ocultado da lista usuários e grupos.</span><span class="sxs-lookup"><span data-stu-id="e5cc2-116">Whether or not to hide the item from the Users and Groups List.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5cc2-117">Relações</span><span class="sxs-lookup"><span data-stu-id="e5cc2-117">Relationships</span></span>
<span data-ttu-id="e5cc2-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5cc2-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5cc2-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5cc2-119">JSON Representation</span></span>
<span data-ttu-id="e5cc2-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5cc2-120">Here is a JSON representation of the resource.</span></span>
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



