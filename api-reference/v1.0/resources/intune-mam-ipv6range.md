---
title: Tipo de recurso iPv6Range
description: Intervalo de IPV6
ms.openlocfilehash: c2f17529b589fc2d7837f6a8f539ff64d5d82dd9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007453"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="a1278-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="a1278-103">iPv6Range resource type</span></span>

> <span data-ttu-id="a1278-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a1278-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1278-105">Intervalo de IPV6</span><span class="sxs-lookup"><span data-stu-id="a1278-105">IP V6 range</span></span>

<span data-ttu-id="a1278-106">Herda de [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="a1278-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a1278-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a1278-107">Properties</span></span>
|<span data-ttu-id="a1278-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1278-108">Property</span></span>|<span data-ttu-id="a1278-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1278-109">Type</span></span>|<span data-ttu-id="a1278-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1278-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1278-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="a1278-111">lowerAddress</span></span>|<span data-ttu-id="a1278-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1278-112">String</span></span>|<span data-ttu-id="a1278-113">Endereço IP de número mais baixo</span><span class="sxs-lookup"><span data-stu-id="a1278-113">Lower IP Address</span></span>|
|<span data-ttu-id="a1278-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="a1278-114">upperAddress</span></span>|<span data-ttu-id="a1278-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1278-115">String</span></span>|<span data-ttu-id="a1278-116">Endereço IP de número mais alto</span><span class="sxs-lookup"><span data-stu-id="a1278-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1278-117">Relações</span><span class="sxs-lookup"><span data-stu-id="a1278-117">Relationships</span></span>
<span data-ttu-id="a1278-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a1278-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a1278-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a1278-119">JSON Representation</span></span>
<span data-ttu-id="a1278-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a1278-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



