---
title: tipo de recurso numberRange
description: Definição do intervalo de números.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 711206a256e17d6e10c7c54cf8a3dda4868db031
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166784"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="7e291-103">tipo de recurso numberRange</span><span class="sxs-lookup"><span data-stu-id="7e291-103">numberRange resource type</span></span>

> <span data-ttu-id="7e291-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7e291-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e291-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7e291-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e291-106">Definição do intervalo de números.</span><span class="sxs-lookup"><span data-stu-id="7e291-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="7e291-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7e291-107">Properties</span></span>
|<span data-ttu-id="7e291-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e291-108">Property</span></span>|<span data-ttu-id="7e291-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e291-109">Type</span></span>|<span data-ttu-id="7e291-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e291-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e291-111">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="7e291-111">lowerNumber</span></span>|<span data-ttu-id="7e291-112">Int32</span><span class="sxs-lookup"><span data-stu-id="7e291-112">Int32</span></span>|<span data-ttu-id="7e291-113">Número menor.</span><span class="sxs-lookup"><span data-stu-id="7e291-113">Lower number.</span></span>|
|<span data-ttu-id="7e291-114">upperNumber</span><span class="sxs-lookup"><span data-stu-id="7e291-114">upperNumber</span></span>|<span data-ttu-id="7e291-115">Int32</span><span class="sxs-lookup"><span data-stu-id="7e291-115">Int32</span></span>|<span data-ttu-id="7e291-116">Número superior.</span><span class="sxs-lookup"><span data-stu-id="7e291-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e291-117">Relações</span><span class="sxs-lookup"><span data-stu-id="7e291-117">Relationships</span></span>
<span data-ttu-id="7e291-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7e291-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e291-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7e291-119">JSON Representation</span></span>
<span data-ttu-id="7e291-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7e291-120">Here is a JSON representation of the resource.</span></span>
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




