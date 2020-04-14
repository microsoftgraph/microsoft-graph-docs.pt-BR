---
title: Tipo de recurso iPv6Range
description: Definição de intervalo IPv6.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 77037ad6e8635a9e83da6fb727b30406e77304b4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473579"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="e1cfb-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="e1cfb-103">iPv6Range resource type</span></span>

<span data-ttu-id="e1cfb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1cfb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1cfb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1cfb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1cfb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1cfb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1cfb-107">Definição de intervalo IPv6.</span><span class="sxs-lookup"><span data-stu-id="e1cfb-107">IPv6 Range definition.</span></span>


<span data-ttu-id="e1cfb-108">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e1cfb-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e1cfb-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1cfb-109">Properties</span></span>
|<span data-ttu-id="e1cfb-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1cfb-110">Property</span></span>|<span data-ttu-id="e1cfb-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1cfb-111">Type</span></span>|<span data-ttu-id="e1cfb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1cfb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1cfb-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="e1cfb-113">lowerAddress</span></span>|<span data-ttu-id="e1cfb-114">String</span><span class="sxs-lookup"><span data-stu-id="e1cfb-114">String</span></span>|<span data-ttu-id="e1cfb-115">Endereço inferior.</span><span class="sxs-lookup"><span data-stu-id="e1cfb-115">Lower address.</span></span>|
|<span data-ttu-id="e1cfb-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="e1cfb-116">upperAddress</span></span>|<span data-ttu-id="e1cfb-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1cfb-117">String</span></span>|<span data-ttu-id="e1cfb-118">Endereço superior.</span><span class="sxs-lookup"><span data-stu-id="e1cfb-118">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1cfb-119">Relações</span><span class="sxs-lookup"><span data-stu-id="e1cfb-119">Relationships</span></span>
<span data-ttu-id="e1cfb-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1cfb-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1cfb-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1cfb-121">JSON Representation</span></span>
<span data-ttu-id="e1cfb-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1cfb-122">Here is a JSON representation of the resource.</span></span>
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



