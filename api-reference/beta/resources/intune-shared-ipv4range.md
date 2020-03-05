---
title: Tipo de recurso iPv4Range
description: Definição de intervalo IPv4.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a4583b84f3bc2859763c0672f1ea833efeda9378
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523643"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="fa75e-103">Tipo de recurso iPv4Range</span><span class="sxs-lookup"><span data-stu-id="fa75e-103">iPv4Range resource type</span></span>

<span data-ttu-id="fa75e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fa75e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa75e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fa75e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa75e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fa75e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa75e-107">Definição de intervalo IPv4.</span><span class="sxs-lookup"><span data-stu-id="fa75e-107">IPv4 Range definition.</span></span>


<span data-ttu-id="fa75e-108">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="fa75e-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fa75e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa75e-109">Properties</span></span>
|<span data-ttu-id="fa75e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa75e-110">Property</span></span>|<span data-ttu-id="fa75e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa75e-111">Type</span></span>|<span data-ttu-id="fa75e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa75e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa75e-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="fa75e-113">lowerAddress</span></span>|<span data-ttu-id="fa75e-114">String</span><span class="sxs-lookup"><span data-stu-id="fa75e-114">String</span></span>|<span data-ttu-id="fa75e-115">Endereço inferior.</span><span class="sxs-lookup"><span data-stu-id="fa75e-115">Lower address.</span></span>|
|<span data-ttu-id="fa75e-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="fa75e-116">upperAddress</span></span>|<span data-ttu-id="fa75e-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa75e-117">String</span></span>|<span data-ttu-id="fa75e-118">Endereço superior.</span><span class="sxs-lookup"><span data-stu-id="fa75e-118">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa75e-119">Relações</span><span class="sxs-lookup"><span data-stu-id="fa75e-119">Relationships</span></span>
<span data-ttu-id="fa75e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fa75e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa75e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa75e-121">JSON Representation</span></span>
<span data-ttu-id="fa75e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa75e-122">Here is a JSON representation of the resource.</span></span>
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



