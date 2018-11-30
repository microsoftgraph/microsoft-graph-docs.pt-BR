---
title: Tipo de recurso extension
description: Um tipo abstrato para oferecer suporte ao tipo openTypeExtension livre do OData v4.
ms.openlocfilehash: b67c347e44c875ca550465be46eecdff3f845eef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034183"
---
# <a name="extension-resource-type"></a><span data-ttu-id="87958-103">Tipo de recurso extension</span><span class="sxs-lookup"><span data-stu-id="87958-103">extension resource type</span></span>

> <span data-ttu-id="87958-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="87958-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87958-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="87958-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87958-106">Um tipo abstrato para oferecer suporte ao tipo [openTypeExtension](opentypeextension.md) livre do OData v4.</span><span class="sxs-lookup"><span data-stu-id="87958-106">An abstract type to support the OData v4 open type [openTypeExtension](opentypeextension.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="87958-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87958-107">JSON representation</span></span>

<span data-ttu-id="87958-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="87958-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a><span data-ttu-id="87958-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87958-109">Properties</span></span>
| <span data-ttu-id="87958-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87958-110">Property</span></span>     | <span data-ttu-id="87958-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="87958-111">Type</span></span>   |<span data-ttu-id="87958-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="87958-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87958-113">id</span><span class="sxs-lookup"><span data-stu-id="87958-113">id</span></span>|<span data-ttu-id="87958-114">String</span><span class="sxs-lookup"><span data-stu-id="87958-114">String</span></span>| <span data-ttu-id="87958-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87958-115">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87958-116">Relações</span><span class="sxs-lookup"><span data-stu-id="87958-116">Relationships</span></span>
<span data-ttu-id="87958-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="87958-117">None</span></span>


## <a name="methods"></a><span data-ttu-id="87958-118">Métodos</span><span class="sxs-lookup"><span data-stu-id="87958-118">Methods</span></span>

<span data-ttu-id="87958-119">Consulte os métodos do tipo derivado [openTypeExtension](opentypeextension.md) para métodos que são realmente compatíveis.</span><span class="sxs-lookup"><span data-stu-id="87958-119">See the methods of the derived type [openTypeExtension](opentypeextension.md) for actually supported methods.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->