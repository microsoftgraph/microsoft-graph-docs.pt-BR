---
title: Tipo de recurso iPv4Range
description: Intervalo de IP V4
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 593fc2287e888b38eadd3c588aaeeb51b31ea78f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816258"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="82146-103">Tipo de recurso iPv4Range</span><span class="sxs-lookup"><span data-stu-id="82146-103">iPv4Range resource type</span></span>

> <span data-ttu-id="82146-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="82146-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82146-105">Intervalo de IP V4</span><span class="sxs-lookup"><span data-stu-id="82146-105">IP V4 range</span></span>

<span data-ttu-id="82146-106">Herda de [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="82146-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="82146-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82146-107">Properties</span></span>
|<span data-ttu-id="82146-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82146-108">Property</span></span>|<span data-ttu-id="82146-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="82146-109">Type</span></span>|<span data-ttu-id="82146-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="82146-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82146-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="82146-111">lowerAddress</span></span>|<span data-ttu-id="82146-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82146-112">String</span></span>|<span data-ttu-id="82146-113">Endereço IP de número mais baixo</span><span class="sxs-lookup"><span data-stu-id="82146-113">Lower IP Address</span></span>|
|<span data-ttu-id="82146-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="82146-114">upperAddress</span></span>|<span data-ttu-id="82146-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82146-115">String</span></span>|<span data-ttu-id="82146-116">Endereço IP de número mais alto</span><span class="sxs-lookup"><span data-stu-id="82146-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="82146-117">Relações</span><span class="sxs-lookup"><span data-stu-id="82146-117">Relationships</span></span>
<span data-ttu-id="82146-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="82146-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="82146-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82146-119">JSON Representation</span></span>
<span data-ttu-id="82146-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="82146-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



