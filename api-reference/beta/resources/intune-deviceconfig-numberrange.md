---
title: tipo de recurso numberRange
description: Definição do intervalo de números.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2e3073de15fc84f5a8cb755d6aad32caaf1ee29f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788489"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="3b2d6-103">tipo de recurso numberRange</span><span class="sxs-lookup"><span data-stu-id="3b2d6-103">numberRange resource type</span></span>

> <span data-ttu-id="3b2d6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b2d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b2d6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b2d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b2d6-106">Definição do intervalo de números.</span><span class="sxs-lookup"><span data-stu-id="3b2d6-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="3b2d6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b2d6-107">Properties</span></span>
|<span data-ttu-id="3b2d6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b2d6-108">Property</span></span>|<span data-ttu-id="3b2d6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b2d6-109">Type</span></span>|<span data-ttu-id="3b2d6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b2d6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b2d6-111">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="3b2d6-111">lowerNumber</span></span>|<span data-ttu-id="3b2d6-112">Int32</span><span class="sxs-lookup"><span data-stu-id="3b2d6-112">Int32</span></span>|<span data-ttu-id="3b2d6-113">Número menor.</span><span class="sxs-lookup"><span data-stu-id="3b2d6-113">Lower number.</span></span>|
|<span data-ttu-id="3b2d6-114">upperNumber</span><span class="sxs-lookup"><span data-stu-id="3b2d6-114">upperNumber</span></span>|<span data-ttu-id="3b2d6-115">Int32</span><span class="sxs-lookup"><span data-stu-id="3b2d6-115">Int32</span></span>|<span data-ttu-id="3b2d6-116">Número superior.</span><span class="sxs-lookup"><span data-stu-id="3b2d6-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b2d6-117">Relações</span><span class="sxs-lookup"><span data-stu-id="3b2d6-117">Relationships</span></span>
<span data-ttu-id="3b2d6-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3b2d6-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b2d6-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b2d6-119">JSON Representation</span></span>
<span data-ttu-id="3b2d6-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3b2d6-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```



