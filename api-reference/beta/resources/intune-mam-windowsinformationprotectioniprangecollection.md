---
title: Tipo de recurso windowsInformationProtectionIPRangeCollection
description: Coleção de intervalos de IP da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cecc1b6bb2fae45da75123000b890654c7c52c2d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160687"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="ab4ee-103">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="ab4ee-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="ab4ee-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ab4ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab4ee-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ab4ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab4ee-106">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="ab4ee-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="ab4ee-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab4ee-107">Properties</span></span>
|<span data-ttu-id="ab4ee-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab4ee-108">Property</span></span>|<span data-ttu-id="ab4ee-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab4ee-109">Type</span></span>|<span data-ttu-id="ab4ee-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab4ee-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab4ee-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ab4ee-111">displayName</span></span>|<span data-ttu-id="ab4ee-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab4ee-112">String</span></span>|<span data-ttu-id="ab4ee-113">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="ab4ee-113">Display name</span></span>|
|<span data-ttu-id="ab4ee-114">ranges</span><span class="sxs-lookup"><span data-stu-id="ab4ee-114">ranges</span></span>|<span data-ttu-id="ab4ee-115">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="ab4ee-115">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="ab4ee-116">Coleção de intervalos de IP</span><span class="sxs-lookup"><span data-stu-id="ab4ee-116">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab4ee-117">Relações</span><span class="sxs-lookup"><span data-stu-id="ab4ee-117">Relationships</span></span>
<span data-ttu-id="ab4ee-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ab4ee-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab4ee-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab4ee-119">JSON Representation</span></span>
<span data-ttu-id="ab4ee-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab4ee-120">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```




