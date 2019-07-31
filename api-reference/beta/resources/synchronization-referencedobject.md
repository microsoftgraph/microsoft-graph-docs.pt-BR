---
title: tipo de recurso referenciouobject
description: Descreve uma referência a outro objeto definido na mesma definição de diretório.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c1c7e1554764031efbfa3a5d1c1280f4b72bc160
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007855"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="55542-103">tipo de recurso referenciouobject</span><span class="sxs-lookup"><span data-stu-id="55542-103">referencedObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55542-104">Descreve uma referência a outro objeto definido na mesma [definição de diretório](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="55542-104">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="55542-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55542-105">Properties</span></span>

| <span data-ttu-id="55542-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55542-106">Property</span></span>                   | <span data-ttu-id="55542-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="55542-107">Type</span></span>                      | <span data-ttu-id="55542-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="55542-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="55542-109">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="55542-109">referencedObjectName</span></span>        |<span data-ttu-id="55542-110">String</span><span class="sxs-lookup"><span data-stu-id="55542-110">String</span></span>                     |<span data-ttu-id="55542-111">Nome do objeto referenciado.</span><span class="sxs-lookup"><span data-stu-id="55542-111">Name of the referenced object.</span></span> <span data-ttu-id="55542-112">Deve corresponder a um dos objetos na [definição de diretório](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="55542-112">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="55542-113">referenciouproperty</span><span class="sxs-lookup"><span data-stu-id="55542-113">referencedProperty</span></span>          |<span data-ttu-id="55542-114">String</span><span class="sxs-lookup"><span data-stu-id="55542-114">String</span></span>                     |<span data-ttu-id="55542-115">**Não suportado no momento**.</span><span class="sxs-lookup"><span data-stu-id="55542-115">**Currently not supported**.</span></span> <span data-ttu-id="55542-116">Nome da propriedade no objeto referenciado, o valor para o qual é usado como a referência.</span><span class="sxs-lookup"><span data-stu-id="55542-116">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55542-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55542-117">JSON representation</span></span>

<span data-ttu-id="55542-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55542-118">The following is a JSON representation of the resource.</span></span>

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
            
