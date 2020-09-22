---
title: Tipo de recurso windowsInformationProtectionIPRangeCollection
description: Coleção de intervalos de IP da Proteção de Informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b243f8923ac44b516a93608fd5c7d82c9cb1296f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074892"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="f311a-103">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="f311a-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

<span data-ttu-id="f311a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f311a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f311a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f311a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f311a-106">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="f311a-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="f311a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f311a-107">Properties</span></span>
|<span data-ttu-id="f311a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f311a-108">Property</span></span>|<span data-ttu-id="f311a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f311a-109">Type</span></span>|<span data-ttu-id="f311a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f311a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f311a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f311a-111">displayName</span></span>|<span data-ttu-id="f311a-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f311a-112">String</span></span>|<span data-ttu-id="f311a-113">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="f311a-113">Display name</span></span>|
|<span data-ttu-id="f311a-114">ranges</span><span class="sxs-lookup"><span data-stu-id="f311a-114">ranges</span></span>|<span data-ttu-id="f311a-115">Coleção [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="f311a-115">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="f311a-116">Conjunto de intervalos de endereços de protocolo IP</span><span class="sxs-lookup"><span data-stu-id="f311a-116">Collection of Internet protocol address ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="f311a-117">Relações</span><span class="sxs-lookup"><span data-stu-id="f311a-117">Relationships</span></span>
<span data-ttu-id="f311a-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f311a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f311a-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f311a-119">JSON Representation</span></span>
<span data-ttu-id="f311a-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f311a-120">Here is a JSON representation of the resource.</span></span>
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









