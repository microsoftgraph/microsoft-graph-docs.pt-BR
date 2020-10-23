---
title: Tipo de recurso windowsInformationProtectionIPRangeCollection
description: Coleção de intervalos de IP da Proteção de Informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 464680aeb1badc90b04a0940b63a890b2fa34693
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726329"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="1bb8a-103">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="1bb8a-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

<span data-ttu-id="1bb8a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bb8a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bb8a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1bb8a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bb8a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1bb8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bb8a-107">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="1bb8a-107">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="1bb8a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1bb8a-108">Properties</span></span>
|<span data-ttu-id="1bb8a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bb8a-109">Property</span></span>|<span data-ttu-id="1bb8a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bb8a-110">Type</span></span>|<span data-ttu-id="1bb8a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bb8a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bb8a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1bb8a-112">displayName</span></span>|<span data-ttu-id="1bb8a-113">String</span><span class="sxs-lookup"><span data-stu-id="1bb8a-113">String</span></span>|<span data-ttu-id="1bb8a-114">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="1bb8a-114">Display name</span></span>|
|<span data-ttu-id="1bb8a-115">ranges</span><span class="sxs-lookup"><span data-stu-id="1bb8a-115">ranges</span></span>|<span data-ttu-id="1bb8a-116">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="1bb8a-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="1bb8a-117">Coleção de intervalos de IP</span><span class="sxs-lookup"><span data-stu-id="1bb8a-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="1bb8a-118">Relações</span><span class="sxs-lookup"><span data-stu-id="1bb8a-118">Relationships</span></span>
<span data-ttu-id="1bb8a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1bb8a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1bb8a-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1bb8a-120">JSON Representation</span></span>
<span data-ttu-id="1bb8a-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1bb8a-121">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.ipRange"
    }
  ]
}
```





