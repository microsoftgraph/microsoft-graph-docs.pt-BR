---
title: Tipo de recurso iPv4Range
description: Definição de intervalo IPv4.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f7fc8ef3ecc436580c14150df472971144b5197d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356447"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="4e4a4-103">Tipo de recurso iPv4Range</span><span class="sxs-lookup"><span data-stu-id="4e4a4-103">iPv4Range resource type</span></span>

> <span data-ttu-id="4e4a4-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e4a4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e4a4-105">Definição de intervalo IPv4.</span><span class="sxs-lookup"><span data-stu-id="4e4a4-105">IPv4 Range definition.</span></span>


<span data-ttu-id="4e4a4-106">Herda de [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="4e4a4-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4e4a4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e4a4-107">Properties</span></span>
|<span data-ttu-id="4e4a4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e4a4-108">Property</span></span>|<span data-ttu-id="4e4a4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e4a4-109">Type</span></span>|<span data-ttu-id="4e4a4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e4a4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e4a4-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="4e4a4-111">lowerAddress</span></span>|<span data-ttu-id="4e4a4-112">String</span><span class="sxs-lookup"><span data-stu-id="4e4a4-112">String</span></span>|<span data-ttu-id="4e4a4-113">Endereço inferior.</span><span class="sxs-lookup"><span data-stu-id="4e4a4-113">Lower address.</span></span>|
|<span data-ttu-id="4e4a4-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="4e4a4-114">upperAddress</span></span>|<span data-ttu-id="4e4a4-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e4a4-115">String</span></span>|<span data-ttu-id="4e4a4-116">Endereço superior.</span><span class="sxs-lookup"><span data-stu-id="4e4a4-116">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e4a4-117">Relações</span><span class="sxs-lookup"><span data-stu-id="4e4a4-117">Relationships</span></span>
<span data-ttu-id="4e4a4-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4e4a4-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e4a4-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e4a4-119">JSON Representation</span></span>
<span data-ttu-id="4e4a4-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e4a4-120">Here is a JSON representation of the resource.</span></span>
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




