---
title: Tipo de recurso windowsInformationProtectionIPRangeCollection
description: Coleção de intervalos de IP da Proteção de Informações do Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b894318bb0b56bb2e5fc86e47a677dd9709e1092
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524248"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="c8755-103">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="c8755-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

<span data-ttu-id="c8755-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c8755-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8755-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c8755-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8755-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8755-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8755-107">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="c8755-107">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="c8755-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8755-108">Properties</span></span>
|<span data-ttu-id="c8755-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8755-109">Property</span></span>|<span data-ttu-id="c8755-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8755-110">Type</span></span>|<span data-ttu-id="c8755-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8755-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8755-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c8755-112">displayName</span></span>|<span data-ttu-id="c8755-113">String</span><span class="sxs-lookup"><span data-stu-id="c8755-113">String</span></span>|<span data-ttu-id="c8755-114">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="c8755-114">Display name</span></span>|
|<span data-ttu-id="c8755-115">ranges</span><span class="sxs-lookup"><span data-stu-id="c8755-115">ranges</span></span>|<span data-ttu-id="c8755-116">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="c8755-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="c8755-117">Coleção de intervalos de IP</span><span class="sxs-lookup"><span data-stu-id="c8755-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8755-118">Relações</span><span class="sxs-lookup"><span data-stu-id="c8755-118">Relationships</span></span>
<span data-ttu-id="c8755-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8755-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8755-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8755-120">JSON Representation</span></span>
<span data-ttu-id="c8755-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8755-121">Here is a JSON representation of the resource.</span></span>
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



