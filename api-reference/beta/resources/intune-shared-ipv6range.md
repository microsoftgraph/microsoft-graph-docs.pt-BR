---
title: Tipo de recurso iPv6Range
description: Definição de intervalo IPv6.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bf5dff72f8df369fa48c71ff58bf6e4925cc16e8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769161"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="315ef-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="315ef-103">iPv6Range resource type</span></span>

> <span data-ttu-id="315ef-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="315ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="315ef-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="315ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="315ef-106">Definição de intervalo IPv6.</span><span class="sxs-lookup"><span data-stu-id="315ef-106">IPv6 Range definition.</span></span>


<span data-ttu-id="315ef-107">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="315ef-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="315ef-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="315ef-108">Properties</span></span>
|<span data-ttu-id="315ef-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="315ef-109">Property</span></span>|<span data-ttu-id="315ef-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="315ef-110">Type</span></span>|<span data-ttu-id="315ef-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="315ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="315ef-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="315ef-112">lowerAddress</span></span>|<span data-ttu-id="315ef-113">String</span><span class="sxs-lookup"><span data-stu-id="315ef-113">String</span></span>|<span data-ttu-id="315ef-114">Endereço inferior.</span><span class="sxs-lookup"><span data-stu-id="315ef-114">Lower address.</span></span>|
|<span data-ttu-id="315ef-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="315ef-115">upperAddress</span></span>|<span data-ttu-id="315ef-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="315ef-116">String</span></span>|<span data-ttu-id="315ef-117">Endereço superior.</span><span class="sxs-lookup"><span data-stu-id="315ef-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="315ef-118">Relações</span><span class="sxs-lookup"><span data-stu-id="315ef-118">Relationships</span></span>
<span data-ttu-id="315ef-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="315ef-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="315ef-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="315ef-120">JSON Representation</span></span>
<span data-ttu-id="315ef-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="315ef-121">Here is a JSON representation of the resource.</span></span>
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



