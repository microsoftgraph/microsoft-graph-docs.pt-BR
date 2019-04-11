---
title: Tipo de recurso windowsInformationProtectionIPRangeCollection
description: Coleção de intervalos de IP da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a972ddf469723acd91e6b122cfef103ab08e24f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785689"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="8cdd0-103">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="8cdd0-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="8cdd0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8cdd0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cdd0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cdd0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cdd0-106">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="8cdd0-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="8cdd0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8cdd0-107">Properties</span></span>
|<span data-ttu-id="8cdd0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cdd0-108">Property</span></span>|<span data-ttu-id="8cdd0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cdd0-109">Type</span></span>|<span data-ttu-id="8cdd0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cdd0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cdd0-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8cdd0-111">displayName</span></span>|<span data-ttu-id="8cdd0-112">String</span><span class="sxs-lookup"><span data-stu-id="8cdd0-112">String</span></span>|<span data-ttu-id="8cdd0-113">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="8cdd0-113">Display name</span></span>|
|<span data-ttu-id="8cdd0-114">ranges</span><span class="sxs-lookup"><span data-stu-id="8cdd0-114">ranges</span></span>|<span data-ttu-id="8cdd0-115">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="8cdd0-115">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="8cdd0-116">Coleção de intervalos de IP</span><span class="sxs-lookup"><span data-stu-id="8cdd0-116">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cdd0-117">Relações</span><span class="sxs-lookup"><span data-stu-id="8cdd0-117">Relationships</span></span>
<span data-ttu-id="8cdd0-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="8cdd0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cdd0-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8cdd0-119">JSON Representation</span></span>
<span data-ttu-id="8cdd0-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8cdd0-120">Here is a JSON representation of the resource.</span></span>
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





