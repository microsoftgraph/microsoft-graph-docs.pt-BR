---
title: Tipo de recurso windowsInformationProtectionIPRangeCollection
description: Coleção de intervalos de IP da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e9d23f8a6d771b116b35058c249866c70c7460d8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952654"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="e604a-103">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="e604a-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="e604a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e604a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e604a-105">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="e604a-105">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="e604a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e604a-106">Properties</span></span>
|<span data-ttu-id="e604a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e604a-107">Property</span></span>|<span data-ttu-id="e604a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e604a-108">Type</span></span>|<span data-ttu-id="e604a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e604a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e604a-110">displayName</span><span class="sxs-lookup"><span data-stu-id="e604a-110">displayName</span></span>|<span data-ttu-id="e604a-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e604a-111">String</span></span>|<span data-ttu-id="e604a-112">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="e604a-112">Display name</span></span>|
|<span data-ttu-id="e604a-113">ranges</span><span class="sxs-lookup"><span data-stu-id="e604a-113">ranges</span></span>|<span data-ttu-id="e604a-114">Coleção [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e604a-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="e604a-115">Coleção de intervalos de IP</span><span class="sxs-lookup"><span data-stu-id="e604a-115">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="e604a-116">Relações</span><span class="sxs-lookup"><span data-stu-id="e604a-116">Relationships</span></span>
<span data-ttu-id="e604a-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e604a-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e604a-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e604a-118">JSON Representation</span></span>
<span data-ttu-id="e604a-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e604a-119">Here is a JSON representation of the resource.</span></span>
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



