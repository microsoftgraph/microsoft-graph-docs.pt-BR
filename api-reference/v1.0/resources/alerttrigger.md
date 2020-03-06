---
title: tipo de recurso alertTrigger
description: Contém informações sobre as propriedades que acionaram uma detecção (as propriedades existem na entidade de alerta).
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 75663b351004d31884f58c53a1ce91e035b0414c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532150"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="939a2-103">tipo de recurso alertTrigger</span><span class="sxs-lookup"><span data-stu-id="939a2-103">alertTrigger resource type</span></span>

<span data-ttu-id="939a2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="939a2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="939a2-105">Contém informações sobre as propriedades que acionaram uma detecção (as propriedades existem na entidade de alerta).</span><span class="sxs-lookup"><span data-stu-id="939a2-105">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="939a2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="939a2-106">Properties</span></span>

| <span data-ttu-id="939a2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="939a2-107">Property</span></span>   | <span data-ttu-id="939a2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="939a2-108">Type</span></span>|<span data-ttu-id="939a2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="939a2-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="939a2-110">nome</span><span class="sxs-lookup"><span data-stu-id="939a2-110">name</span></span>|<span data-ttu-id="939a2-111">String</span><span class="sxs-lookup"><span data-stu-id="939a2-111">String</span></span>|<span data-ttu-id="939a2-112">Nome da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="939a2-112">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="939a2-113">type</span><span class="sxs-lookup"><span data-stu-id="939a2-113">type</span></span>|<span data-ttu-id="939a2-114">String</span><span class="sxs-lookup"><span data-stu-id="939a2-114">String</span></span>|<span data-ttu-id="939a2-115">Tipo da propriedade no par chave: valor para interpretação.</span><span class="sxs-lookup"><span data-stu-id="939a2-115">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="939a2-116">Por exemplo, String, Boolean, etc.</span><span class="sxs-lookup"><span data-stu-id="939a2-116">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="939a2-117">value</span><span class="sxs-lookup"><span data-stu-id="939a2-117">value</span></span>|<span data-ttu-id="939a2-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="939a2-118">String</span></span>|<span data-ttu-id="939a2-119">O valor da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="939a2-119">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="939a2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="939a2-120">JSON representation</span></span>

<span data-ttu-id="939a2-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="939a2-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="939a2-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="939a2-122">Example</span></span>

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
