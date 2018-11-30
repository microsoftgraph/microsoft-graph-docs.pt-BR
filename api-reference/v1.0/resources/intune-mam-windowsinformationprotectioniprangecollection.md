---
title: Tipo de recurso windowsInformationProtectionIPRangeCollection
description: Coleção de intervalos de IP da Proteção de Informações do Windows
ms.openlocfilehash: 41558014ec3d48af06788e15fc40786fe7f9aea4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004522"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="efc02-103">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="efc02-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="efc02-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="efc02-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="efc02-105">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="efc02-105">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="efc02-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="efc02-106">Properties</span></span>
|<span data-ttu-id="efc02-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efc02-107">Property</span></span>|<span data-ttu-id="efc02-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="efc02-108">Type</span></span>|<span data-ttu-id="efc02-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="efc02-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efc02-110">displayName</span><span class="sxs-lookup"><span data-stu-id="efc02-110">displayName</span></span>|<span data-ttu-id="efc02-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efc02-111">String</span></span>|<span data-ttu-id="efc02-112">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="efc02-112">Display name</span></span>|
|<span data-ttu-id="efc02-113">ranges</span><span class="sxs-lookup"><span data-stu-id="efc02-113">ranges</span></span>|<span data-ttu-id="efc02-114">Coleção [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="efc02-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="efc02-115">Coleção de intervalos de IP</span><span class="sxs-lookup"><span data-stu-id="efc02-115">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="efc02-116">Relações</span><span class="sxs-lookup"><span data-stu-id="efc02-116">Relationships</span></span>
<span data-ttu-id="efc02-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="efc02-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="efc02-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="efc02-118">JSON Representation</span></span>
<span data-ttu-id="efc02-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="efc02-119">Here is a JSON representation of the resource.</span></span>
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



