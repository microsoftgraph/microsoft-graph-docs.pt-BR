---
title: tipo de recurso numberRange
description: Definição do intervalo de números.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8f637cb10e36ba1f2d7c45e391adc64c6e9eb00b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722996"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="ed048-103">tipo de recurso numberRange</span><span class="sxs-lookup"><span data-stu-id="ed048-103">numberRange resource type</span></span>

<span data-ttu-id="ed048-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed048-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed048-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ed048-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed048-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed048-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed048-107">Definição do intervalo de números.</span><span class="sxs-lookup"><span data-stu-id="ed048-107">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="ed048-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed048-108">Properties</span></span>
|<span data-ttu-id="ed048-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed048-109">Property</span></span>|<span data-ttu-id="ed048-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed048-110">Type</span></span>|<span data-ttu-id="ed048-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed048-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed048-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="ed048-112">lowerNumber</span></span>|<span data-ttu-id="ed048-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ed048-113">Int32</span></span>|<span data-ttu-id="ed048-114">Número menor.</span><span class="sxs-lookup"><span data-stu-id="ed048-114">Lower number.</span></span>|
|<span data-ttu-id="ed048-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="ed048-115">upperNumber</span></span>|<span data-ttu-id="ed048-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ed048-116">Int32</span></span>|<span data-ttu-id="ed048-117">Número superior.</span><span class="sxs-lookup"><span data-stu-id="ed048-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed048-118">Relações</span><span class="sxs-lookup"><span data-stu-id="ed048-118">Relationships</span></span>
<span data-ttu-id="ed048-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed048-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed048-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed048-120">JSON Representation</span></span>
<span data-ttu-id="ed048-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed048-121">Here is a JSON representation of the resource.</span></span>
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





