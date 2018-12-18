---
title: Tipo de recurso iPv4Range
description: Intervalo de IP V4
author: tfitzmac
ms.openlocfilehash: 3dd5479776cf5f497ab6f26e893a78c73fa6ad86
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316664"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="8ab34-103">Tipo de recurso iPv4Range</span><span class="sxs-lookup"><span data-stu-id="8ab34-103">iPv4Range resource type</span></span>

> <span data-ttu-id="8ab34-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8ab34-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ab34-105">Intervalo de IP V4</span><span class="sxs-lookup"><span data-stu-id="8ab34-105">IP V4 range</span></span>

<span data-ttu-id="8ab34-106">Herda de [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="8ab34-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8ab34-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ab34-107">Properties</span></span>
|<span data-ttu-id="8ab34-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ab34-108">Property</span></span>|<span data-ttu-id="8ab34-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ab34-109">Type</span></span>|<span data-ttu-id="8ab34-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ab34-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ab34-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="8ab34-111">lowerAddress</span></span>|<span data-ttu-id="8ab34-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ab34-112">String</span></span>|<span data-ttu-id="8ab34-113">Endereço IP de número mais baixo</span><span class="sxs-lookup"><span data-stu-id="8ab34-113">Lower IP Address</span></span>|
|<span data-ttu-id="8ab34-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="8ab34-114">upperAddress</span></span>|<span data-ttu-id="8ab34-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ab34-115">String</span></span>|<span data-ttu-id="8ab34-116">Endereço IP de número mais alto</span><span class="sxs-lookup"><span data-stu-id="8ab34-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ab34-117">Relações</span><span class="sxs-lookup"><span data-stu-id="8ab34-117">Relationships</span></span>
<span data-ttu-id="8ab34-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ab34-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8ab34-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ab34-119">JSON Representation</span></span>
<span data-ttu-id="8ab34-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ab34-120">Here is a JSON representation of the resource.</span></span>
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



