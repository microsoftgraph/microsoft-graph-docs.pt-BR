---
title: tipo de recurso de alertTrigger
description: Contém informações sobre as propriedades que disparou uma detecção (Propriedades existirem na entidade alerta).
author: Preetikr
localization_priority: Normal
ms.openlocfilehash: 1dc8bb2b18380da50134aa67e742da89dea3c057
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894338"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="5c4d3-103">tipo de recurso de alertTrigger</span><span class="sxs-lookup"><span data-stu-id="5c4d3-103">alertTrigger resource type</span></span>

<span data-ttu-id="5c4d3-104">Contém informações sobre as propriedades que disparou uma detecção (Propriedades existirem na entidade alerta).</span><span class="sxs-lookup"><span data-stu-id="5c4d3-104">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="5c4d3-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5c4d3-105">Properties</span></span>

| <span data-ttu-id="5c4d3-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c4d3-106">Property</span></span>   | <span data-ttu-id="5c4d3-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c4d3-107">Type</span></span>|<span data-ttu-id="5c4d3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c4d3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c4d3-109">name</span><span class="sxs-lookup"><span data-stu-id="5c4d3-109">name</span></span>|<span data-ttu-id="5c4d3-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c4d3-110">String</span></span>|<span data-ttu-id="5c4d3-111">Nome da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="5c4d3-111">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="5c4d3-112">type</span><span class="sxs-lookup"><span data-stu-id="5c4d3-112">type</span></span>|<span data-ttu-id="5c4d3-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c4d3-113">String</span></span>|<span data-ttu-id="5c4d3-114">Tipo da propriedade no par de chave: valor de interpretação.</span><span class="sxs-lookup"><span data-stu-id="5c4d3-114">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="5c4d3-115">Por exemplo, String, Boolean, etc.</span><span class="sxs-lookup"><span data-stu-id="5c4d3-115">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="5c4d3-116">valor</span><span class="sxs-lookup"><span data-stu-id="5c4d3-116">value</span></span>|<span data-ttu-id="5c4d3-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c4d3-117">String</span></span>|<span data-ttu-id="5c4d3-118">Valor da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="5c4d3-118">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5c4d3-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5c4d3-119">JSON representation</span></span>

<span data-ttu-id="5c4d3-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5c4d3-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a><span data-ttu-id="5c4d3-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c4d3-121">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
