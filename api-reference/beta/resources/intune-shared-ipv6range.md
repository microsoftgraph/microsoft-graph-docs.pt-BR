---
title: Tipo de recurso iPv6Range
description: Definição de intervalo IPv6.
author: rolyon
localization_priority: Normal
doc_type: resourcePageType
ms.prod: Intune
ms.openlocfilehash: 1f2b46cea71d097955ca9e78cc74f6f0cddd1002
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967366"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="2b721-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="2b721-103">iPv6Range resource type</span></span>

> <span data-ttu-id="2b721-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2b721-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b721-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b721-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b721-106">Definição de intervalo IPv6.</span><span class="sxs-lookup"><span data-stu-id="2b721-106">IPv6 Range definition.</span></span>


<span data-ttu-id="2b721-107">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="2b721-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2b721-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b721-108">Properties</span></span>
|<span data-ttu-id="2b721-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b721-109">Property</span></span>|<span data-ttu-id="2b721-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b721-110">Type</span></span>|<span data-ttu-id="2b721-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b721-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b721-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="2b721-112">lowerAddress</span></span>|<span data-ttu-id="2b721-113">String</span><span class="sxs-lookup"><span data-stu-id="2b721-113">String</span></span>|<span data-ttu-id="2b721-114">Endereço inferior.</span><span class="sxs-lookup"><span data-stu-id="2b721-114">Lower address.</span></span>|
|<span data-ttu-id="2b721-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="2b721-115">upperAddress</span></span>|<span data-ttu-id="2b721-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b721-116">String</span></span>|<span data-ttu-id="2b721-117">Endereço superior.</span><span class="sxs-lookup"><span data-stu-id="2b721-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b721-118">Relações</span><span class="sxs-lookup"><span data-stu-id="2b721-118">Relationships</span></span>
<span data-ttu-id="2b721-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b721-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b721-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b721-120">JSON Representation</span></span>
<span data-ttu-id="2b721-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b721-121">Here is a JSON representation of the resource.</span></span>
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





