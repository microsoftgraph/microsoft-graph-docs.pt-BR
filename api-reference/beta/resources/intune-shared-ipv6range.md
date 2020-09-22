---
title: Tipo de recurso iPv6Range
description: Definição de intervalo IPv6.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 64db37b136f8077f5134e8848521b98b7a9b8f15
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095118"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="0ae80-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="0ae80-103">iPv6Range resource type</span></span>

<span data-ttu-id="0ae80-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ae80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ae80-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0ae80-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ae80-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0ae80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ae80-107">Definição de intervalo IPv6.</span><span class="sxs-lookup"><span data-stu-id="0ae80-107">IPv6 Range definition.</span></span>


<span data-ttu-id="0ae80-108">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="0ae80-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0ae80-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ae80-109">Properties</span></span>
|<span data-ttu-id="0ae80-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ae80-110">Property</span></span>|<span data-ttu-id="0ae80-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ae80-111">Type</span></span>|<span data-ttu-id="0ae80-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ae80-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ae80-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="0ae80-113">lowerAddress</span></span>|<span data-ttu-id="0ae80-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ae80-114">String</span></span>|<span data-ttu-id="0ae80-115">Endereço inferior.</span><span class="sxs-lookup"><span data-stu-id="0ae80-115">Lower address.</span></span>|
|<span data-ttu-id="0ae80-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="0ae80-116">upperAddress</span></span>|<span data-ttu-id="0ae80-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ae80-117">String</span></span>|<span data-ttu-id="0ae80-118">Endereço superior.</span><span class="sxs-lookup"><span data-stu-id="0ae80-118">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ae80-119">Relações</span><span class="sxs-lookup"><span data-stu-id="0ae80-119">Relationships</span></span>
<span data-ttu-id="0ae80-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0ae80-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ae80-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ae80-121">JSON Representation</span></span>
<span data-ttu-id="0ae80-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ae80-122">Here is a JSON representation of the resource.</span></span>
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






