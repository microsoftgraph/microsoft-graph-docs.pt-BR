---
title: Tipo de recurso windowsInformationProtectionResourceCollection
description: Coleção de recursos da Proteção de Informações do Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 81b3a75533f70c57e31fe0f56770a281b66c61af
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366927"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="d991f-103">Tipo de recurso windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="d991f-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="d991f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d991f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d991f-105">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="d991f-105">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="d991f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d991f-106">Properties</span></span>
|<span data-ttu-id="d991f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d991f-107">Property</span></span>|<span data-ttu-id="d991f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d991f-108">Type</span></span>|<span data-ttu-id="d991f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d991f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d991f-110">displayName</span><span class="sxs-lookup"><span data-stu-id="d991f-110">displayName</span></span>|<span data-ttu-id="d991f-111">String</span><span class="sxs-lookup"><span data-stu-id="d991f-111">String</span></span>|<span data-ttu-id="d991f-112">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="d991f-112">Display name</span></span>|
|<span data-ttu-id="d991f-113">recursos</span><span class="sxs-lookup"><span data-stu-id="d991f-113">resources</span></span>|<span data-ttu-id="d991f-114">String collection</span><span class="sxs-lookup"><span data-stu-id="d991f-114">String collection</span></span>|<span data-ttu-id="d991f-115">Coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="d991f-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="d991f-116">Relações</span><span class="sxs-lookup"><span data-stu-id="d991f-116">Relationships</span></span>
<span data-ttu-id="d991f-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d991f-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d991f-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d991f-118">JSON Representation</span></span>
<span data-ttu-id="d991f-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d991f-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```




