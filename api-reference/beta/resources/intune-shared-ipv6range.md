---
title: Tipo de recurso iPv6Range
description: Definição de intervalo IPv6.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 51815dffc0048ec88b81cbe6034a42e108e5b222
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803567"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="62698-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="62698-103">iPv6Range resource type</span></span>

> <span data-ttu-id="62698-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62698-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62698-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62698-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62698-106">Definição de intervalo IPv6.</span><span class="sxs-lookup"><span data-stu-id="62698-106">IPv6 Range definition.</span></span>


<span data-ttu-id="62698-107">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="62698-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="62698-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62698-108">Properties</span></span>
|<span data-ttu-id="62698-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62698-109">Property</span></span>|<span data-ttu-id="62698-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="62698-110">Type</span></span>|<span data-ttu-id="62698-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="62698-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62698-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="62698-112">lowerAddress</span></span>|<span data-ttu-id="62698-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62698-113">String</span></span>|<span data-ttu-id="62698-114">Endereço inferior.</span><span class="sxs-lookup"><span data-stu-id="62698-114">Lower address.</span></span>|
|<span data-ttu-id="62698-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="62698-115">upperAddress</span></span>|<span data-ttu-id="62698-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62698-116">String</span></span>|<span data-ttu-id="62698-117">Endereço superior.</span><span class="sxs-lookup"><span data-stu-id="62698-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62698-118">Relações</span><span class="sxs-lookup"><span data-stu-id="62698-118">Relationships</span></span>
<span data-ttu-id="62698-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="62698-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62698-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62698-120">JSON Representation</span></span>
<span data-ttu-id="62698-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62698-121">Here is a JSON representation of the resource.</span></span>
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





