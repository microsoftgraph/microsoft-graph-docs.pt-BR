---
title: Tipo de recurso iPv6Range
description: Definição de intervalo IPv6.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f171a8ebb28d15e78a30bf542c37a163f0d097f0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258986"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="37f99-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="37f99-103">iPv6Range resource type</span></span>

> <span data-ttu-id="37f99-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37f99-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37f99-105">Definição de intervalo IPv6.</span><span class="sxs-lookup"><span data-stu-id="37f99-105">IPv6 Range definition.</span></span>


<span data-ttu-id="37f99-106">Herda de [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="37f99-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="37f99-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37f99-107">Properties</span></span>
|<span data-ttu-id="37f99-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37f99-108">Property</span></span>|<span data-ttu-id="37f99-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="37f99-109">Type</span></span>|<span data-ttu-id="37f99-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="37f99-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37f99-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="37f99-111">lowerAddress</span></span>|<span data-ttu-id="37f99-112">String</span><span class="sxs-lookup"><span data-stu-id="37f99-112">String</span></span>|<span data-ttu-id="37f99-113">Endereço inferior</span><span class="sxs-lookup"><span data-stu-id="37f99-113">Lower address</span></span>|
|<span data-ttu-id="37f99-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="37f99-114">upperAddress</span></span>|<span data-ttu-id="37f99-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37f99-115">String</span></span>|<span data-ttu-id="37f99-116">Endereço superior</span><span class="sxs-lookup"><span data-stu-id="37f99-116">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="37f99-117">Relações</span><span class="sxs-lookup"><span data-stu-id="37f99-117">Relationships</span></span>
<span data-ttu-id="37f99-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37f99-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37f99-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37f99-119">JSON Representation</span></span>
<span data-ttu-id="37f99-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37f99-120">Here is a JSON representation of the resource.</span></span>
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



