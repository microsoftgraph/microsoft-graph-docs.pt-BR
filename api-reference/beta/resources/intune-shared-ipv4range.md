---
title: Tipo de recurso iPv4Range
description: Definição de intervalo IPv4.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1bed3b43af7203a6c1ee081156708679337e94e0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769280"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="80277-103">Tipo de recurso iPv4Range</span><span class="sxs-lookup"><span data-stu-id="80277-103">iPv4Range resource type</span></span>

> <span data-ttu-id="80277-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="80277-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80277-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80277-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80277-106">Definição de intervalo IPv4.</span><span class="sxs-lookup"><span data-stu-id="80277-106">IPv4 Range definition.</span></span>


<span data-ttu-id="80277-107">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="80277-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="80277-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80277-108">Properties</span></span>
|<span data-ttu-id="80277-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80277-109">Property</span></span>|<span data-ttu-id="80277-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="80277-110">Type</span></span>|<span data-ttu-id="80277-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="80277-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80277-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="80277-112">lowerAddress</span></span>|<span data-ttu-id="80277-113">String</span><span class="sxs-lookup"><span data-stu-id="80277-113">String</span></span>|<span data-ttu-id="80277-114">Endereço inferior.</span><span class="sxs-lookup"><span data-stu-id="80277-114">Lower address.</span></span>|
|<span data-ttu-id="80277-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="80277-115">upperAddress</span></span>|<span data-ttu-id="80277-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80277-116">String</span></span>|<span data-ttu-id="80277-117">Endereço superior.</span><span class="sxs-lookup"><span data-stu-id="80277-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80277-118">Relações</span><span class="sxs-lookup"><span data-stu-id="80277-118">Relationships</span></span>
<span data-ttu-id="80277-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80277-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80277-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80277-120">JSON Representation</span></span>
<span data-ttu-id="80277-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80277-121">Here is a JSON representation of the resource.</span></span>
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



