---
title: Tipo de recurso extension
description: Um tipo abstrato para oferecer suporte ao tipo openTypeExtension livre do OData v4.
ms.openlocfilehash: 1b3d735e0997ca128b539bff9a05c9c7c56799df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003673"
---
# <a name="extension-resource-type"></a><span data-ttu-id="ac968-103">Tipo de recurso extension</span><span class="sxs-lookup"><span data-stu-id="ac968-103">extension resource type</span></span>

<span data-ttu-id="ac968-104">Um tipo abstrato para oferecer suporte ao tipo [openTypeExtension](opentypeextension.md) livre do OData v4.</span><span class="sxs-lookup"><span data-stu-id="ac968-104">An abstract type to support the OData v4 open type [openTypeExtension](opentypeextension.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac968-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac968-105">JSON representation</span></span>

<span data-ttu-id="ac968-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ac968-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "abstract": "true",
  "baseType": "microsoft.graph.entity",
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a><span data-ttu-id="ac968-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac968-107">Properties</span></span>
| <span data-ttu-id="ac968-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac968-108">Property</span></span>     | <span data-ttu-id="ac968-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac968-109">Type</span></span>   |<span data-ttu-id="ac968-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac968-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac968-111">id</span><span class="sxs-lookup"><span data-stu-id="ac968-111">id</span></span>|<span data-ttu-id="ac968-112">String</span><span class="sxs-lookup"><span data-stu-id="ac968-112">String</span></span>| <span data-ttu-id="ac968-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac968-113">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac968-114">Relações</span><span class="sxs-lookup"><span data-stu-id="ac968-114">Relationships</span></span>
<span data-ttu-id="ac968-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac968-115">None</span></span>


## <a name="methods"></a><span data-ttu-id="ac968-116">Métodos</span><span class="sxs-lookup"><span data-stu-id="ac968-116">Methods</span></span>

<span data-ttu-id="ac968-117">Consulte os métodos do tipo derivado [openTypeExtension](opentypeextension.md) para métodos que são realmente compatíveis.</span><span class="sxs-lookup"><span data-stu-id="ac968-117">See the methods of the derived type [openTypeExtension](opentypeextension.md) for actually supported methods.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->