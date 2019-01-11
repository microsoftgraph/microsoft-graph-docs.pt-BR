---
title: Tipo de recurso iPv6Range
description: Intervalo de IPV6
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 759f661464d2dd5cd6c12f6fbfe6b1bfcf549a70
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829656"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="7ded2-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="7ded2-103">iPv6Range resource type</span></span>

> <span data-ttu-id="7ded2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7ded2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ded2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7ded2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ded2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7ded2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ded2-107">Intervalo de IPV6</span><span class="sxs-lookup"><span data-stu-id="7ded2-107">IP V6 range</span></span>

<span data-ttu-id="7ded2-108">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="7ded2-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7ded2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ded2-109">Properties</span></span>
|<span data-ttu-id="7ded2-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ded2-110">Property</span></span>|<span data-ttu-id="7ded2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ded2-111">Type</span></span>|<span data-ttu-id="7ded2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ded2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ded2-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="7ded2-113">lowerAddress</span></span>|<span data-ttu-id="7ded2-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ded2-114">String</span></span>|<span data-ttu-id="7ded2-115">Endereço IP de número mais baixo</span><span class="sxs-lookup"><span data-stu-id="7ded2-115">Lower IP Address</span></span>|
|<span data-ttu-id="7ded2-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="7ded2-116">upperAddress</span></span>|<span data-ttu-id="7ded2-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ded2-117">String</span></span>|<span data-ttu-id="7ded2-118">Endereço IP de número mais alto</span><span class="sxs-lookup"><span data-stu-id="7ded2-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ded2-119">Relações</span><span class="sxs-lookup"><span data-stu-id="7ded2-119">Relationships</span></span>
<span data-ttu-id="7ded2-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ded2-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7ded2-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ded2-121">JSON Representation</span></span>
<span data-ttu-id="7ded2-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ded2-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



