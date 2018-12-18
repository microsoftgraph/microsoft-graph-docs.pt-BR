---
title: Tipo de recurso iPv6Range
description: Intervalo de IPV6
author: tfitzmac
ms.openlocfilehash: b5a2ad772d45b4be5fa3a8f4da04b28bc965195d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337545"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="572b0-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="572b0-103">iPv6Range resource type</span></span>

> <span data-ttu-id="572b0-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="572b0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="572b0-105">Intervalo de IPV6</span><span class="sxs-lookup"><span data-stu-id="572b0-105">IP V6 range</span></span>

<span data-ttu-id="572b0-106">Herda de [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="572b0-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="572b0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="572b0-107">Properties</span></span>
|<span data-ttu-id="572b0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="572b0-108">Property</span></span>|<span data-ttu-id="572b0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="572b0-109">Type</span></span>|<span data-ttu-id="572b0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="572b0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="572b0-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="572b0-111">lowerAddress</span></span>|<span data-ttu-id="572b0-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="572b0-112">String</span></span>|<span data-ttu-id="572b0-113">Endereço IP de número mais baixo</span><span class="sxs-lookup"><span data-stu-id="572b0-113">Lower IP Address</span></span>|
|<span data-ttu-id="572b0-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="572b0-114">upperAddress</span></span>|<span data-ttu-id="572b0-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="572b0-115">String</span></span>|<span data-ttu-id="572b0-116">Endereço IP de número mais alto</span><span class="sxs-lookup"><span data-stu-id="572b0-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="572b0-117">Relações</span><span class="sxs-lookup"><span data-stu-id="572b0-117">Relationships</span></span>
<span data-ttu-id="572b0-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="572b0-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="572b0-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="572b0-119">JSON Representation</span></span>
<span data-ttu-id="572b0-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="572b0-120">Here is a JSON representation of the resource.</span></span>
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



