---
title: Tipo de recurso iPv6Range
description: Intervalo de IPV6
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 84d925cc7885dab4b3e87dbd62060894e741f52c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845742"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="466e5-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="466e5-103">iPv6Range resource type</span></span>

> <span data-ttu-id="466e5-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="466e5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="466e5-105">Intervalo de IPV6</span><span class="sxs-lookup"><span data-stu-id="466e5-105">IP V6 range</span></span>

<span data-ttu-id="466e5-106">Herda de [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="466e5-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="466e5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="466e5-107">Properties</span></span>
|<span data-ttu-id="466e5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="466e5-108">Property</span></span>|<span data-ttu-id="466e5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="466e5-109">Type</span></span>|<span data-ttu-id="466e5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="466e5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="466e5-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="466e5-111">lowerAddress</span></span>|<span data-ttu-id="466e5-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="466e5-112">String</span></span>|<span data-ttu-id="466e5-113">Endereço IP de número mais baixo</span><span class="sxs-lookup"><span data-stu-id="466e5-113">Lower IP Address</span></span>|
|<span data-ttu-id="466e5-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="466e5-114">upperAddress</span></span>|<span data-ttu-id="466e5-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="466e5-115">String</span></span>|<span data-ttu-id="466e5-116">Endereço IP de número mais alto</span><span class="sxs-lookup"><span data-stu-id="466e5-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="466e5-117">Relações</span><span class="sxs-lookup"><span data-stu-id="466e5-117">Relationships</span></span>
<span data-ttu-id="466e5-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="466e5-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="466e5-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="466e5-119">JSON Representation</span></span>
<span data-ttu-id="466e5-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="466e5-120">Here is a JSON representation of the resource.</span></span>
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



