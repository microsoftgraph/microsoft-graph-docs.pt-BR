---
title: Tipo de recurso iPv6Range
description: Definição de intervalo IPv6.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b54782b1851ea800b548f02b34f60da3a3236a3
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571533"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="bdf01-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="bdf01-103">iPv6Range resource type</span></span>

> <span data-ttu-id="bdf01-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bdf01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdf01-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bdf01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdf01-106">Definição de intervalo IPv6.</span><span class="sxs-lookup"><span data-stu-id="bdf01-106">IPv6 Range definition.</span></span>


<span data-ttu-id="bdf01-107">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="bdf01-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bdf01-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bdf01-108">Properties</span></span>
|<span data-ttu-id="bdf01-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdf01-109">Property</span></span>|<span data-ttu-id="bdf01-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdf01-110">Type</span></span>|<span data-ttu-id="bdf01-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdf01-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdf01-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="bdf01-112">lowerAddress</span></span>|<span data-ttu-id="bdf01-113">String</span><span class="sxs-lookup"><span data-stu-id="bdf01-113">String</span></span>|<span data-ttu-id="bdf01-114">Endereço inferior.</span><span class="sxs-lookup"><span data-stu-id="bdf01-114">Lower address.</span></span>|
|<span data-ttu-id="bdf01-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="bdf01-115">upperAddress</span></span>|<span data-ttu-id="bdf01-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdf01-116">String</span></span>|<span data-ttu-id="bdf01-117">Endereço superior.</span><span class="sxs-lookup"><span data-stu-id="bdf01-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdf01-118">Relações</span><span class="sxs-lookup"><span data-stu-id="bdf01-118">Relationships</span></span>
<span data-ttu-id="bdf01-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bdf01-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bdf01-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bdf01-120">JSON Representation</span></span>
<span data-ttu-id="bdf01-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bdf01-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```




