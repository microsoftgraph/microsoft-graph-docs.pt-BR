---
title: Tipo de recurso windowsInformationProtectionIPRangeCollection
description: Coleção de intervalos de IP da Proteção de Informações do Windows
author: tfitzmac
ms.openlocfilehash: 12030ab0b71448c644e4e664f9095dea3e48a26c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319751"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="18764-103">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="18764-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="18764-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="18764-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18764-105">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="18764-105">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="18764-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18764-106">Properties</span></span>
|<span data-ttu-id="18764-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18764-107">Property</span></span>|<span data-ttu-id="18764-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="18764-108">Type</span></span>|<span data-ttu-id="18764-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="18764-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18764-110">displayName</span><span class="sxs-lookup"><span data-stu-id="18764-110">displayName</span></span>|<span data-ttu-id="18764-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18764-111">String</span></span>|<span data-ttu-id="18764-112">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="18764-112">Display name</span></span>|
|<span data-ttu-id="18764-113">ranges</span><span class="sxs-lookup"><span data-stu-id="18764-113">ranges</span></span>|<span data-ttu-id="18764-114">Coleção [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="18764-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="18764-115">Coleção de intervalos de IP</span><span class="sxs-lookup"><span data-stu-id="18764-115">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="18764-116">Relações</span><span class="sxs-lookup"><span data-stu-id="18764-116">Relationships</span></span>
<span data-ttu-id="18764-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18764-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="18764-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18764-118">JSON Representation</span></span>
<span data-ttu-id="18764-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18764-119">Here is a JSON representation of the resource.</span></span>
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



