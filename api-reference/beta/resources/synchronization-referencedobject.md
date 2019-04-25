---
title: tipo de recurso referenciouobject
description: Descreve uma referência a outro objeto definido na mesma definição de diretório.
localization_priority: Normal
ms.openlocfilehash: dcec232335fdf3d447097ea1ae87fbc9ea676cfe
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523234"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="cb704-103">tipo de recurso referenciouobject</span><span class="sxs-lookup"><span data-stu-id="cb704-103">referencedObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb704-104">Descreve uma referência a outro objeto definido na mesma [definição de diretório](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cb704-104">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cb704-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb704-105">Properties</span></span>

| <span data-ttu-id="cb704-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb704-106">Property</span></span>                   | <span data-ttu-id="cb704-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb704-107">Type</span></span>                      | <span data-ttu-id="cb704-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb704-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="cb704-109">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="cb704-109">referencedObjectName</span></span>        |<span data-ttu-id="cb704-110">String</span><span class="sxs-lookup"><span data-stu-id="cb704-110">String</span></span>                     |<span data-ttu-id="cb704-111">Nome do objeto referenciado.</span><span class="sxs-lookup"><span data-stu-id="cb704-111">Name of the referenced object.</span></span> <span data-ttu-id="cb704-112">Deve corresponder a um dos objetos na [definição de diretório](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cb704-112">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="cb704-113">referenciouproperty</span><span class="sxs-lookup"><span data-stu-id="cb704-113">referencedProperty</span></span>          |<span data-ttu-id="cb704-114">String</span><span class="sxs-lookup"><span data-stu-id="cb704-114">String</span></span>                     |<span data-ttu-id="cb704-115">**Não suportado no momento**.</span><span class="sxs-lookup"><span data-stu-id="cb704-115">**Currently not supported**.</span></span> <span data-ttu-id="cb704-116">Nome da propriedade no objeto referenciado, o valor para o qual é usado como a referência.</span><span class="sxs-lookup"><span data-stu-id="cb704-116">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb704-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb704-117">JSON representation</span></span>

<span data-ttu-id="cb704-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb704-118">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-referencedobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
            
