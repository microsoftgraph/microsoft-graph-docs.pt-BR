---
title: Tipo de recurso windowsInformationProtectionIPRangeCollection
description: Coleção de intervalos de IP da Proteção de Informações do Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1774a52b6dd5535443bb24dea5e786fc2c8cff34
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360640"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="100d6-103">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="100d6-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="100d6-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="100d6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="100d6-105">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="100d6-105">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="100d6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="100d6-106">Properties</span></span>
|<span data-ttu-id="100d6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="100d6-107">Property</span></span>|<span data-ttu-id="100d6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="100d6-108">Type</span></span>|<span data-ttu-id="100d6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="100d6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="100d6-110">displayName</span><span class="sxs-lookup"><span data-stu-id="100d6-110">displayName</span></span>|<span data-ttu-id="100d6-111">String</span><span class="sxs-lookup"><span data-stu-id="100d6-111">String</span></span>|<span data-ttu-id="100d6-112">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="100d6-112">Display name</span></span>|
|<span data-ttu-id="100d6-113">ranges</span><span class="sxs-lookup"><span data-stu-id="100d6-113">ranges</span></span>|<span data-ttu-id="100d6-114">Coleção [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="100d6-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="100d6-115">Conjunto de intervalos de endereços de protocolo IP</span><span class="sxs-lookup"><span data-stu-id="100d6-115">Collection of Internet protocol address ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="100d6-116">Relações</span><span class="sxs-lookup"><span data-stu-id="100d6-116">Relationships</span></span>
<span data-ttu-id="100d6-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="100d6-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="100d6-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="100d6-118">JSON Representation</span></span>
<span data-ttu-id="100d6-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="100d6-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.ipRange",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```




