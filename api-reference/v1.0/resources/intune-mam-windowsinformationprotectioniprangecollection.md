---
title: Tipo de recurso windowsInformationProtectionIPRangeCollection
description: Coleção de intervalos de IP da Proteção de Informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 131694ba3ef67f1f87a1e40cd7545ad6e78717de
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468394"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="7aa13-103">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="7aa13-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

<span data-ttu-id="7aa13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7aa13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7aa13-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7aa13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7aa13-106">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="7aa13-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="7aa13-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7aa13-107">Properties</span></span>
|<span data-ttu-id="7aa13-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7aa13-108">Property</span></span>|<span data-ttu-id="7aa13-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7aa13-109">Type</span></span>|<span data-ttu-id="7aa13-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aa13-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7aa13-111">displayName</span><span class="sxs-lookup"><span data-stu-id="7aa13-111">displayName</span></span>|<span data-ttu-id="7aa13-112">String</span><span class="sxs-lookup"><span data-stu-id="7aa13-112">String</span></span>|<span data-ttu-id="7aa13-113">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="7aa13-113">Display name</span></span>|
|<span data-ttu-id="7aa13-114">ranges</span><span class="sxs-lookup"><span data-stu-id="7aa13-114">ranges</span></span>|<span data-ttu-id="7aa13-115">Coleção [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="7aa13-115">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="7aa13-116">Conjunto de intervalos de endereços de protocolo IP</span><span class="sxs-lookup"><span data-stu-id="7aa13-116">Collection of Internet protocol address ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="7aa13-117">Relações</span><span class="sxs-lookup"><span data-stu-id="7aa13-117">Relationships</span></span>
<span data-ttu-id="7aa13-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7aa13-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7aa13-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7aa13-119">JSON Representation</span></span>
<span data-ttu-id="7aa13-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7aa13-120">Here is a JSON representation of the resource.</span></span>
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







