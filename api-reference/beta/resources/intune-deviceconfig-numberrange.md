---
title: tipo de recurso numberRange
description: Definição do intervalo de números.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4e47252b42fe7be886a1d6ce7c0d71b6c2dc1b21
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460958"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="95bb7-103">tipo de recurso numberRange</span><span class="sxs-lookup"><span data-stu-id="95bb7-103">numberRange resource type</span></span>

<span data-ttu-id="95bb7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95bb7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95bb7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="95bb7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95bb7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="95bb7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95bb7-107">Definição do intervalo de números.</span><span class="sxs-lookup"><span data-stu-id="95bb7-107">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="95bb7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95bb7-108">Properties</span></span>
|<span data-ttu-id="95bb7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95bb7-109">Property</span></span>|<span data-ttu-id="95bb7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="95bb7-110">Type</span></span>|<span data-ttu-id="95bb7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="95bb7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95bb7-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="95bb7-112">lowerNumber</span></span>|<span data-ttu-id="95bb7-113">Int32</span><span class="sxs-lookup"><span data-stu-id="95bb7-113">Int32</span></span>|<span data-ttu-id="95bb7-114">Número menor.</span><span class="sxs-lookup"><span data-stu-id="95bb7-114">Lower number.</span></span>|
|<span data-ttu-id="95bb7-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="95bb7-115">upperNumber</span></span>|<span data-ttu-id="95bb7-116">Int32</span><span class="sxs-lookup"><span data-stu-id="95bb7-116">Int32</span></span>|<span data-ttu-id="95bb7-117">Número superior.</span><span class="sxs-lookup"><span data-stu-id="95bb7-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95bb7-118">Relações</span><span class="sxs-lookup"><span data-stu-id="95bb7-118">Relationships</span></span>
<span data-ttu-id="95bb7-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="95bb7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95bb7-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95bb7-120">JSON Representation</span></span>
<span data-ttu-id="95bb7-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="95bb7-121">Here is a JSON representation of the resource.</span></span>
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



