---
title: tipo de recurso alertTrigger
description: Contém informações sobre as propriedades que acionaram uma detecção (as propriedades existem na entidade de alerta).
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 3a2f6818bad0c5600e4b2a2a2682707643d1900c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569463"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="7ae90-103">tipo de recurso alertTrigger</span><span class="sxs-lookup"><span data-stu-id="7ae90-103">alertTrigger resource type</span></span>

<span data-ttu-id="7ae90-104">Contém informações sobre as propriedades que acionaram uma detecção (as propriedades existem na entidade de alerta).</span><span class="sxs-lookup"><span data-stu-id="7ae90-104">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="7ae90-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ae90-105">Properties</span></span>

| <span data-ttu-id="7ae90-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ae90-106">Property</span></span>   | <span data-ttu-id="7ae90-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ae90-107">Type</span></span>|<span data-ttu-id="7ae90-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ae90-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ae90-109">name</span><span class="sxs-lookup"><span data-stu-id="7ae90-109">name</span></span>|<span data-ttu-id="7ae90-110">String</span><span class="sxs-lookup"><span data-stu-id="7ae90-110">String</span></span>|<span data-ttu-id="7ae90-111">Nome da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="7ae90-111">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="7ae90-112">type</span><span class="sxs-lookup"><span data-stu-id="7ae90-112">type</span></span>|<span data-ttu-id="7ae90-113">String</span><span class="sxs-lookup"><span data-stu-id="7ae90-113">String</span></span>|<span data-ttu-id="7ae90-114">Tipo da propriedade no par chave: valor para interpretação.</span><span class="sxs-lookup"><span data-stu-id="7ae90-114">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="7ae90-115">Por exemplo, String, Boolean, etc.</span><span class="sxs-lookup"><span data-stu-id="7ae90-115">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="7ae90-116">value</span><span class="sxs-lookup"><span data-stu-id="7ae90-116">value</span></span>|<span data-ttu-id="7ae90-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ae90-117">String</span></span>|<span data-ttu-id="7ae90-118">O valor da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="7ae90-118">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ae90-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ae90-119">JSON representation</span></span>

<span data-ttu-id="7ae90-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ae90-120">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="7ae90-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ae90-121">Example</span></span>

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
