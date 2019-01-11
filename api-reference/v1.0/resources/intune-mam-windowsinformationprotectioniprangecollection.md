---
title: Tipo de recurso windowsInformationProtectionIPRangeCollection
description: Coleção de intervalos de IP da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2ba01b8a4385b5c06cc1e6a95441e9b7946a116d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839743"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="412dc-103">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="412dc-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="412dc-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="412dc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="412dc-105">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="412dc-105">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="412dc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="412dc-106">Properties</span></span>
|<span data-ttu-id="412dc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="412dc-107">Property</span></span>|<span data-ttu-id="412dc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="412dc-108">Type</span></span>|<span data-ttu-id="412dc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="412dc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="412dc-110">displayName</span><span class="sxs-lookup"><span data-stu-id="412dc-110">displayName</span></span>|<span data-ttu-id="412dc-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="412dc-111">String</span></span>|<span data-ttu-id="412dc-112">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="412dc-112">Display name</span></span>|
|<span data-ttu-id="412dc-113">ranges</span><span class="sxs-lookup"><span data-stu-id="412dc-113">ranges</span></span>|<span data-ttu-id="412dc-114">Coleção [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="412dc-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="412dc-115">Coleção de intervalos de IP</span><span class="sxs-lookup"><span data-stu-id="412dc-115">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="412dc-116">Relações</span><span class="sxs-lookup"><span data-stu-id="412dc-116">Relationships</span></span>
<span data-ttu-id="412dc-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="412dc-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="412dc-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="412dc-118">JSON Representation</span></span>
<span data-ttu-id="412dc-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="412dc-119">Here is a JSON representation of the resource.</span></span>
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



