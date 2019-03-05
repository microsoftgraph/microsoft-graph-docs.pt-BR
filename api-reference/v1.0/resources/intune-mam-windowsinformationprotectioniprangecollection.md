---
title: Tipo de recurso windowsInformationProtectionIPRangeCollection
description: Coleção de intervalos de IP da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6a2f52613eae9d8e06751672c95230dfc3b00c4
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253894"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="80650-103">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="80650-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="80650-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80650-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80650-105">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="80650-105">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="80650-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80650-106">Properties</span></span>
|<span data-ttu-id="80650-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80650-107">Property</span></span>|<span data-ttu-id="80650-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="80650-108">Type</span></span>|<span data-ttu-id="80650-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="80650-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80650-110">displayName</span><span class="sxs-lookup"><span data-stu-id="80650-110">displayName</span></span>|<span data-ttu-id="80650-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80650-111">String</span></span>|<span data-ttu-id="80650-112">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="80650-112">Display name</span></span>|
|<span data-ttu-id="80650-113">ranges</span><span class="sxs-lookup"><span data-stu-id="80650-113">ranges</span></span>|<span data-ttu-id="80650-114">Coleção [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="80650-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="80650-115">Conjunto de intervalos de endereços de protocolo IP</span><span class="sxs-lookup"><span data-stu-id="80650-115">Collection of Internet protocol address ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="80650-116">Relações</span><span class="sxs-lookup"><span data-stu-id="80650-116">Relationships</span></span>
<span data-ttu-id="80650-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80650-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80650-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80650-118">JSON Representation</span></span>
<span data-ttu-id="80650-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80650-119">Here is a JSON representation of the resource.</span></span>
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



