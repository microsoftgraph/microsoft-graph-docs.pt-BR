---
title: Tipo de recurso iPv6Range
description: Definição de intervalo IPv6.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 04183f443d767236a1a7c0afb1d1ed9b92c37889
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038136"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="efbe0-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="efbe0-103">iPv6Range resource type</span></span>

> <span data-ttu-id="efbe0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="efbe0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efbe0-105">Definição de intervalo IPv6.</span><span class="sxs-lookup"><span data-stu-id="efbe0-105">IPv6 Range definition.</span></span>


<span data-ttu-id="efbe0-106">Herda de [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="efbe0-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="efbe0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="efbe0-107">Properties</span></span>
|<span data-ttu-id="efbe0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efbe0-108">Property</span></span>|<span data-ttu-id="efbe0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="efbe0-109">Type</span></span>|<span data-ttu-id="efbe0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="efbe0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efbe0-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="efbe0-111">lowerAddress</span></span>|<span data-ttu-id="efbe0-112">String</span><span class="sxs-lookup"><span data-stu-id="efbe0-112">String</span></span>|<span data-ttu-id="efbe0-113">Endereço inferior</span><span class="sxs-lookup"><span data-stu-id="efbe0-113">Lower address</span></span>|
|<span data-ttu-id="efbe0-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="efbe0-114">upperAddress</span></span>|<span data-ttu-id="efbe0-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efbe0-115">String</span></span>|<span data-ttu-id="efbe0-116">Endereço superior</span><span class="sxs-lookup"><span data-stu-id="efbe0-116">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="efbe0-117">Relações</span><span class="sxs-lookup"><span data-stu-id="efbe0-117">Relationships</span></span>
<span data-ttu-id="efbe0-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="efbe0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="efbe0-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="efbe0-119">JSON Representation</span></span>
<span data-ttu-id="efbe0-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="efbe0-120">Here is a JSON representation of the resource.</span></span>
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



