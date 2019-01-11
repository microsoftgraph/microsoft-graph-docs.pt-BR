---
title: Tipo de recurso iPv4Range
description: Intervalo de IP V4
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a1f76fcd99663fe7ddd34263c8304b5597e6941c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888288"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="7bb98-103">Tipo de recurso iPv4Range</span><span class="sxs-lookup"><span data-stu-id="7bb98-103">iPv4Range resource type</span></span>

> <span data-ttu-id="7bb98-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7bb98-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7bb98-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7bb98-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7bb98-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7bb98-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7bb98-107">Intervalo de IP V4</span><span class="sxs-lookup"><span data-stu-id="7bb98-107">IP V4 range</span></span>

<span data-ttu-id="7bb98-108">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="7bb98-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7bb98-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7bb98-109">Properties</span></span>
|<span data-ttu-id="7bb98-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bb98-110">Property</span></span>|<span data-ttu-id="7bb98-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bb98-111">Type</span></span>|<span data-ttu-id="7bb98-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bb98-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bb98-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="7bb98-113">lowerAddress</span></span>|<span data-ttu-id="7bb98-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bb98-114">String</span></span>|<span data-ttu-id="7bb98-115">Endereço IP de número mais baixo</span><span class="sxs-lookup"><span data-stu-id="7bb98-115">Lower IP Address</span></span>|
|<span data-ttu-id="7bb98-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="7bb98-116">upperAddress</span></span>|<span data-ttu-id="7bb98-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bb98-117">String</span></span>|<span data-ttu-id="7bb98-118">Endereço IP de número mais alto</span><span class="sxs-lookup"><span data-stu-id="7bb98-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bb98-119">Relações</span><span class="sxs-lookup"><span data-stu-id="7bb98-119">Relationships</span></span>
<span data-ttu-id="7bb98-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7bb98-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bb98-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7bb98-121">JSON Representation</span></span>
<span data-ttu-id="7bb98-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7bb98-122">Here is a JSON representation of the resource.</span></span>
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



