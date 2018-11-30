---
title: Tipo de recurso iPv4Range
description: Intervalo de IP V4
ms.openlocfilehash: 8b59101e1fcdb5ab88d9c24a0359f8abb1687818
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006268"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="0bb4a-103">Tipo de recurso iPv4Range</span><span class="sxs-lookup"><span data-stu-id="0bb4a-103">iPv4Range resource type</span></span>

> <span data-ttu-id="0bb4a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0bb4a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bb4a-105">Intervalo de IP V4</span><span class="sxs-lookup"><span data-stu-id="0bb4a-105">IP V4 range</span></span>

<span data-ttu-id="0bb4a-106">Herda de [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="0bb4a-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0bb4a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0bb4a-107">Properties</span></span>
|<span data-ttu-id="0bb4a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bb4a-108">Property</span></span>|<span data-ttu-id="0bb4a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bb4a-109">Type</span></span>|<span data-ttu-id="0bb4a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bb4a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bb4a-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="0bb4a-111">lowerAddress</span></span>|<span data-ttu-id="0bb4a-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bb4a-112">String</span></span>|<span data-ttu-id="0bb4a-113">Endereço IP de número mais baixo</span><span class="sxs-lookup"><span data-stu-id="0bb4a-113">Lower IP Address</span></span>|
|<span data-ttu-id="0bb4a-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="0bb4a-114">upperAddress</span></span>|<span data-ttu-id="0bb4a-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bb4a-115">String</span></span>|<span data-ttu-id="0bb4a-116">Endereço IP de número mais alto</span><span class="sxs-lookup"><span data-stu-id="0bb4a-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bb4a-117">Relações</span><span class="sxs-lookup"><span data-stu-id="0bb4a-117">Relationships</span></span>
<span data-ttu-id="0bb4a-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0bb4a-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0bb4a-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0bb4a-119">JSON Representation</span></span>
<span data-ttu-id="0bb4a-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0bb4a-120">Here is a JSON representation of the resource.</span></span>
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



