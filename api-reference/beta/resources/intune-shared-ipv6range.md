---
title: Tipo de recurso iPv6Range
description: Definição de intervalo IPv6.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24ee76f226e54e2f04da2f3cf4ebf47e6e4fa537
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995977"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="1461d-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="1461d-103">iPv6Range resource type</span></span>

> <span data-ttu-id="1461d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1461d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1461d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1461d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1461d-106">Definição de intervalo IPv6.</span><span class="sxs-lookup"><span data-stu-id="1461d-106">IPv6 Range definition.</span></span>


<span data-ttu-id="1461d-107">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="1461d-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1461d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1461d-108">Properties</span></span>
|<span data-ttu-id="1461d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1461d-109">Property</span></span>|<span data-ttu-id="1461d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1461d-110">Type</span></span>|<span data-ttu-id="1461d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1461d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1461d-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="1461d-112">lowerAddress</span></span>|<span data-ttu-id="1461d-113">String</span><span class="sxs-lookup"><span data-stu-id="1461d-113">String</span></span>|<span data-ttu-id="1461d-114">Endereço inferior.</span><span class="sxs-lookup"><span data-stu-id="1461d-114">Lower address.</span></span>|
|<span data-ttu-id="1461d-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="1461d-115">upperAddress</span></span>|<span data-ttu-id="1461d-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1461d-116">String</span></span>|<span data-ttu-id="1461d-117">Endereço superior.</span><span class="sxs-lookup"><span data-stu-id="1461d-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1461d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="1461d-118">Relationships</span></span>
<span data-ttu-id="1461d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1461d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1461d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1461d-120">JSON Representation</span></span>
<span data-ttu-id="1461d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1461d-121">Here is a JSON representation of the resource.</span></span>
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





