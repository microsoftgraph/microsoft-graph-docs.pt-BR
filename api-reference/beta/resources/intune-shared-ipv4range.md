---
title: Tipo de recurso iPv4Range
description: Intervalo de IP V4
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 57bcaabfc5155e6b6733de2dc228dd240515281b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980178"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="5bb9a-103">Tipo de recurso iPv4Range</span><span class="sxs-lookup"><span data-stu-id="5bb9a-103">iPv4Range resource type</span></span>

> <span data-ttu-id="5bb9a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5bb9a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5bb9a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5bb9a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5bb9a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5bb9a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5bb9a-107">Intervalo de IP V4</span><span class="sxs-lookup"><span data-stu-id="5bb9a-107">IP V4 range</span></span>

<span data-ttu-id="5bb9a-108">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="5bb9a-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5bb9a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5bb9a-109">Properties</span></span>
|<span data-ttu-id="5bb9a-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5bb9a-110">Property</span></span>|<span data-ttu-id="5bb9a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="5bb9a-111">Type</span></span>|<span data-ttu-id="5bb9a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bb9a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bb9a-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="5bb9a-113">lowerAddress</span></span>|<span data-ttu-id="5bb9a-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bb9a-114">String</span></span>|<span data-ttu-id="5bb9a-115">Endereço IP de número mais baixo</span><span class="sxs-lookup"><span data-stu-id="5bb9a-115">Lower IP Address</span></span>|
|<span data-ttu-id="5bb9a-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="5bb9a-116">upperAddress</span></span>|<span data-ttu-id="5bb9a-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bb9a-117">String</span></span>|<span data-ttu-id="5bb9a-118">Endereço IP de número mais alto</span><span class="sxs-lookup"><span data-stu-id="5bb9a-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="5bb9a-119">Relações</span><span class="sxs-lookup"><span data-stu-id="5bb9a-119">Relationships</span></span>
<span data-ttu-id="5bb9a-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5bb9a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5bb9a-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5bb9a-121">JSON Representation</span></span>
<span data-ttu-id="5bb9a-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5bb9a-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



