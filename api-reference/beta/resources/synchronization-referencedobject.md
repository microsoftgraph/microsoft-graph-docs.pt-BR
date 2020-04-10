---
title: tipo de recurso referenciouobject
description: Descreve uma referência a outro objeto definido na mesma definição de diretório.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7779fb851812c00c15749877517b79273752ab58
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217588"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="99482-103">tipo de recurso referenciouobject</span><span class="sxs-lookup"><span data-stu-id="99482-103">referencedObject resource type</span></span>

<span data-ttu-id="99482-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99482-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99482-105">Descreve uma referência a outro objeto definido na mesma [definição de diretório](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="99482-105">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="99482-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99482-106">Properties</span></span>

| <span data-ttu-id="99482-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99482-107">Property</span></span>                   | <span data-ttu-id="99482-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="99482-108">Type</span></span>                      | <span data-ttu-id="99482-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="99482-109">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="99482-110">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="99482-110">referencedObjectName</span></span>        |<span data-ttu-id="99482-111">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="99482-111">String</span></span>                     |<span data-ttu-id="99482-112">Nome do objeto referenciado.</span><span class="sxs-lookup"><span data-stu-id="99482-112">Name of the referenced object.</span></span> <span data-ttu-id="99482-113">Deve corresponder a um dos objetos na [definição de diretório](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="99482-113">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="99482-114">referenciouproperty</span><span class="sxs-lookup"><span data-stu-id="99482-114">referencedProperty</span></span>          |<span data-ttu-id="99482-115">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="99482-115">String</span></span>                     |<span data-ttu-id="99482-116">**Não suportado no momento**.</span><span class="sxs-lookup"><span data-stu-id="99482-116">**Currently not supported**.</span></span> <span data-ttu-id="99482-117">Nome da propriedade no objeto referenciado, o valor para o qual é usado como a referência.</span><span class="sxs-lookup"><span data-stu-id="99482-117">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99482-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99482-118">JSON representation</span></span>

<span data-ttu-id="99482-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99482-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referencedObject"
}-->

```json
{
  "referencedObjectName": "String",
  "referencedProperty": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
            
