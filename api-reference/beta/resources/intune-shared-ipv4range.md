---
title: Tipo de recurso iPv4Range
description: Definição de intervalo IPv4.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6a732ad11980b22b08d4684a8706e244e78a08a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938864"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="f64af-103">Tipo de recurso iPv4Range</span><span class="sxs-lookup"><span data-stu-id="f64af-103">iPv4Range resource type</span></span>

> <span data-ttu-id="f64af-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f64af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f64af-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f64af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f64af-106">Definição de intervalo IPv4.</span><span class="sxs-lookup"><span data-stu-id="f64af-106">IPv4 Range definition.</span></span>


<span data-ttu-id="f64af-107">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="f64af-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f64af-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f64af-108">Properties</span></span>
|<span data-ttu-id="f64af-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f64af-109">Property</span></span>|<span data-ttu-id="f64af-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f64af-110">Type</span></span>|<span data-ttu-id="f64af-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f64af-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f64af-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="f64af-112">lowerAddress</span></span>|<span data-ttu-id="f64af-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f64af-113">String</span></span>|<span data-ttu-id="f64af-114">Endereço inferior.</span><span class="sxs-lookup"><span data-stu-id="f64af-114">Lower address.</span></span>|
|<span data-ttu-id="f64af-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="f64af-115">upperAddress</span></span>|<span data-ttu-id="f64af-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f64af-116">String</span></span>|<span data-ttu-id="f64af-117">Endereço superior.</span><span class="sxs-lookup"><span data-stu-id="f64af-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f64af-118">Relações</span><span class="sxs-lookup"><span data-stu-id="f64af-118">Relationships</span></span>
<span data-ttu-id="f64af-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f64af-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f64af-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f64af-120">JSON Representation</span></span>
<span data-ttu-id="f64af-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f64af-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```




