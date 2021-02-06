---
title: Tipo de recurso referencedObject
description: Descreve uma referência a outro objeto definido na mesma definição de diretório.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: c6e273474c70919bab3c30335a26477509eca8cc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132515"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="ad601-103">Tipo de recurso referencedObject</span><span class="sxs-lookup"><span data-stu-id="ad601-103">referencedObject resource type</span></span>

<span data-ttu-id="ad601-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad601-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad601-105">Descreve uma referência a outro objeto definido na mesma definição [de diretório.](synchronization-directorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad601-105">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ad601-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad601-106">Properties</span></span>

| <span data-ttu-id="ad601-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad601-107">Property</span></span>                   | <span data-ttu-id="ad601-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad601-108">Type</span></span>                      | <span data-ttu-id="ad601-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad601-109">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="ad601-110">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="ad601-110">referencedObjectName</span></span>        |<span data-ttu-id="ad601-111">String</span><span class="sxs-lookup"><span data-stu-id="ad601-111">String</span></span>                     |<span data-ttu-id="ad601-112">Nome do objeto referenciado.</span><span class="sxs-lookup"><span data-stu-id="ad601-112">Name of the referenced object.</span></span> <span data-ttu-id="ad601-113">Deve corresponder a um dos objetos na definição [de diretório.](synchronization-directorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad601-113">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="ad601-114">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="ad601-114">referencedProperty</span></span>          |<span data-ttu-id="ad601-115">String</span><span class="sxs-lookup"><span data-stu-id="ad601-115">String</span></span>                     |<span data-ttu-id="ad601-116">**Não há suporte no momento.**</span><span class="sxs-lookup"><span data-stu-id="ad601-116">**Currently not supported**.</span></span> <span data-ttu-id="ad601-117">Nome da propriedade no objeto referenciado, o valor para o qual é usado como referência.</span><span class="sxs-lookup"><span data-stu-id="ad601-117">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad601-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad601-118">JSON representation</span></span>

<span data-ttu-id="ad601-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ad601-119">The following is a JSON representation of the resource.</span></span>

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
            


