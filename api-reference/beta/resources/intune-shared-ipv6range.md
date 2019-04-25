---
title: Tipo de recurso iPv6Range
description: Definição de intervalo IPv6.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 51815dffc0048ec88b81cbe6034a42e108e5b222
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550578"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="c5803-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="c5803-103">iPv6Range resource type</span></span>

> <span data-ttu-id="c5803-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c5803-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5803-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5803-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5803-106">Definição de intervalo IPv6.</span><span class="sxs-lookup"><span data-stu-id="c5803-106">IPv6 Range definition.</span></span>


<span data-ttu-id="c5803-107">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="c5803-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c5803-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5803-108">Properties</span></span>
|<span data-ttu-id="c5803-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5803-109">Property</span></span>|<span data-ttu-id="c5803-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5803-110">Type</span></span>|<span data-ttu-id="c5803-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5803-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5803-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="c5803-112">lowerAddress</span></span>|<span data-ttu-id="c5803-113">String</span><span class="sxs-lookup"><span data-stu-id="c5803-113">String</span></span>|<span data-ttu-id="c5803-114">Endereço inferior.</span><span class="sxs-lookup"><span data-stu-id="c5803-114">Lower address.</span></span>|
|<span data-ttu-id="c5803-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="c5803-115">upperAddress</span></span>|<span data-ttu-id="c5803-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5803-116">String</span></span>|<span data-ttu-id="c5803-117">Endereço superior.</span><span class="sxs-lookup"><span data-stu-id="c5803-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5803-118">Relações</span><span class="sxs-lookup"><span data-stu-id="c5803-118">Relationships</span></span>
<span data-ttu-id="c5803-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c5803-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5803-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5803-120">JSON Representation</span></span>
<span data-ttu-id="c5803-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5803-121">Here is a JSON representation of the resource.</span></span>
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





