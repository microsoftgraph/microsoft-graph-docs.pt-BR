---
title: Tipo de recurso alertTrigger
description: Contém informações sobre as propriedades que dispararam uma detecção (existem propriedades na entidade de alerta).
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6bdee4ee550b44694a572e3611652b19c7ff574c
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129436"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="207f1-103">Tipo de recurso alertTrigger</span><span class="sxs-lookup"><span data-stu-id="207f1-103">alertTrigger resource type</span></span>

<span data-ttu-id="207f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="207f1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="207f1-105">Contém informações sobre as propriedades que dispararam uma detecção (existem propriedades na entidade de alerta).</span><span class="sxs-lookup"><span data-stu-id="207f1-105">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="207f1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="207f1-106">Properties</span></span>

| <span data-ttu-id="207f1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="207f1-107">Property</span></span>   | <span data-ttu-id="207f1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="207f1-108">Type</span></span>|<span data-ttu-id="207f1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="207f1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="207f1-110">nome</span><span class="sxs-lookup"><span data-stu-id="207f1-110">name</span></span>|<span data-ttu-id="207f1-111">String</span><span class="sxs-lookup"><span data-stu-id="207f1-111">String</span></span>|<span data-ttu-id="207f1-112">Nome da propriedade que serve como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="207f1-112">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="207f1-113">tipo</span><span class="sxs-lookup"><span data-stu-id="207f1-113">type</span></span>|<span data-ttu-id="207f1-114">String</span><span class="sxs-lookup"><span data-stu-id="207f1-114">String</span></span>|<span data-ttu-id="207f1-115">Tipo da propriedade no par key:value para interpretação.</span><span class="sxs-lookup"><span data-stu-id="207f1-115">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="207f1-116">Por exemplo, String, Boolean etc.</span><span class="sxs-lookup"><span data-stu-id="207f1-116">For example, String, Boolean etc.</span></span>|
|<span data-ttu-id="207f1-117">value</span><span class="sxs-lookup"><span data-stu-id="207f1-117">value</span></span>|<span data-ttu-id="207f1-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="207f1-118">String</span></span>|<span data-ttu-id="207f1-119">Valor da propriedade que serve como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="207f1-119">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="207f1-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="207f1-120">JSON representation</span></span>

<span data-ttu-id="207f1-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="207f1-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="207f1-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="207f1-122">Example</span></span>

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

