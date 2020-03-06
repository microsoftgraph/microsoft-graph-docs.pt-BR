---
title: Tipo de recurso iPv6Range
description: Definição de intervalo IPv6.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e6def6fa06d9cad863dcfd8c2cc7bb03f718bab3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530197"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="e5634-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="e5634-103">iPv6Range resource type</span></span>

<span data-ttu-id="e5634-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5634-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5634-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5634-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5634-106">Definição de intervalo IPv6.</span><span class="sxs-lookup"><span data-stu-id="e5634-106">IPv6 Range definition.</span></span>


<span data-ttu-id="e5634-107">Herda de [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e5634-107">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e5634-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5634-108">Properties</span></span>
|<span data-ttu-id="e5634-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5634-109">Property</span></span>|<span data-ttu-id="e5634-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5634-110">Type</span></span>|<span data-ttu-id="e5634-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5634-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5634-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="e5634-112">lowerAddress</span></span>|<span data-ttu-id="e5634-113">String</span><span class="sxs-lookup"><span data-stu-id="e5634-113">String</span></span>|<span data-ttu-id="e5634-114">Endereço inferior</span><span class="sxs-lookup"><span data-stu-id="e5634-114">Lower address</span></span>|
|<span data-ttu-id="e5634-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="e5634-115">upperAddress</span></span>|<span data-ttu-id="e5634-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5634-116">String</span></span>|<span data-ttu-id="e5634-117">Endereço superior</span><span class="sxs-lookup"><span data-stu-id="e5634-117">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5634-118">Relações</span><span class="sxs-lookup"><span data-stu-id="e5634-118">Relationships</span></span>
<span data-ttu-id="e5634-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5634-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5634-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5634-120">JSON Representation</span></span>
<span data-ttu-id="e5634-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5634-121">Here is a JSON representation of the resource.</span></span>
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




