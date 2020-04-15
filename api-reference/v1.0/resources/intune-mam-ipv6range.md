---
title: Tipo de recurso iPv6Range
description: Definição de intervalo IPv6.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b0e0b733ceea2585198a46e62d0f033b76748035
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439366"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="313b8-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="313b8-103">iPv6Range resource type</span></span>

<span data-ttu-id="313b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="313b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="313b8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="313b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="313b8-106">Definição de intervalo IPv6.</span><span class="sxs-lookup"><span data-stu-id="313b8-106">IPv6 Range definition.</span></span>


<span data-ttu-id="313b8-107">Herda de [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="313b8-107">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="313b8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="313b8-108">Properties</span></span>
|<span data-ttu-id="313b8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="313b8-109">Property</span></span>|<span data-ttu-id="313b8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="313b8-110">Type</span></span>|<span data-ttu-id="313b8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="313b8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="313b8-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="313b8-112">lowerAddress</span></span>|<span data-ttu-id="313b8-113">String</span><span class="sxs-lookup"><span data-stu-id="313b8-113">String</span></span>|<span data-ttu-id="313b8-114">Endereço inferior</span><span class="sxs-lookup"><span data-stu-id="313b8-114">Lower address</span></span>|
|<span data-ttu-id="313b8-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="313b8-115">upperAddress</span></span>|<span data-ttu-id="313b8-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="313b8-116">String</span></span>|<span data-ttu-id="313b8-117">Endereço superior</span><span class="sxs-lookup"><span data-stu-id="313b8-117">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="313b8-118">Relações</span><span class="sxs-lookup"><span data-stu-id="313b8-118">Relationships</span></span>
<span data-ttu-id="313b8-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="313b8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="313b8-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="313b8-120">JSON Representation</span></span>
<span data-ttu-id="313b8-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="313b8-121">Here is a JSON representation of the resource.</span></span>
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







