---
title: Tipo de recurso windowsInformationProtectionIPRangeCollection
description: Coleção de intervalos de IP da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a972ddf469723acd91e6b122cfef103ab08e24f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522087"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="38edd-103">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="38edd-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="38edd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="38edd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38edd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="38edd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38edd-106">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="38edd-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="38edd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38edd-107">Properties</span></span>
|<span data-ttu-id="38edd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38edd-108">Property</span></span>|<span data-ttu-id="38edd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="38edd-109">Type</span></span>|<span data-ttu-id="38edd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="38edd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38edd-111">displayName</span><span class="sxs-lookup"><span data-stu-id="38edd-111">displayName</span></span>|<span data-ttu-id="38edd-112">String</span><span class="sxs-lookup"><span data-stu-id="38edd-112">String</span></span>|<span data-ttu-id="38edd-113">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="38edd-113">Display name</span></span>|
|<span data-ttu-id="38edd-114">ranges</span><span class="sxs-lookup"><span data-stu-id="38edd-114">ranges</span></span>|<span data-ttu-id="38edd-115">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="38edd-115">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="38edd-116">Coleção de intervalos de IP</span><span class="sxs-lookup"><span data-stu-id="38edd-116">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="38edd-117">Relações</span><span class="sxs-lookup"><span data-stu-id="38edd-117">Relationships</span></span>
<span data-ttu-id="38edd-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="38edd-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38edd-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38edd-119">JSON Representation</span></span>
<span data-ttu-id="38edd-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38edd-120">Here is a JSON representation of the resource.</span></span>
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





