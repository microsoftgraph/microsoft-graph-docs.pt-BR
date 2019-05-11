---
title: Tipo de recurso windowsInformationProtectionResourceCollection
description: Coleção de recursos da Proteção de Informações do Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f5a31f85b70095975d1692e2a0aff175df12512
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940565"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="1901c-103">Tipo de recurso windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="1901c-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="1901c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1901c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1901c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1901c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1901c-106">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="1901c-106">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="1901c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1901c-107">Properties</span></span>
|<span data-ttu-id="1901c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1901c-108">Property</span></span>|<span data-ttu-id="1901c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1901c-109">Type</span></span>|<span data-ttu-id="1901c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1901c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1901c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1901c-111">displayName</span></span>|<span data-ttu-id="1901c-112">String</span><span class="sxs-lookup"><span data-stu-id="1901c-112">String</span></span>|<span data-ttu-id="1901c-113">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="1901c-113">Display name</span></span>|
|<span data-ttu-id="1901c-114">recursos</span><span class="sxs-lookup"><span data-stu-id="1901c-114">resources</span></span>|<span data-ttu-id="1901c-115">String collection</span><span class="sxs-lookup"><span data-stu-id="1901c-115">String collection</span></span>|<span data-ttu-id="1901c-116">Coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="1901c-116">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="1901c-117">Relações</span><span class="sxs-lookup"><span data-stu-id="1901c-117">Relationships</span></span>
<span data-ttu-id="1901c-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1901c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1901c-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1901c-119">JSON Representation</span></span>
<span data-ttu-id="1901c-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1901c-120">Here is a JSON representation of the resource.</span></span>
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




