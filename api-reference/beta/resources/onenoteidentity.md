---
title: tipo de recurso de oneNoteIdentity
description: '**Suporte em breve**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: f1b03ad907a0b8f6f3cf2674d74f1ee8722357ea
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513939"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="8ba55-103">tipo de recurso de oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="8ba55-103">oneNoteIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ba55-104">**Suporte em breve**</span><span class="sxs-lookup"><span data-stu-id="8ba55-104">**Support coming soon**</span></span>

<span data-ttu-id="8ba55-105">O tipo de OneNoteIdentity representa uma identidade de um _usuário_.</span><span class="sxs-lookup"><span data-stu-id="8ba55-105">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="8ba55-106">No futuro, esse tipo de será mesclado com [identidade](identity.md)</span><span class="sxs-lookup"><span data-stu-id="8ba55-106">In future, this type will be merged with [Identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="8ba55-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ba55-107">JSON representation</span></span>

<span data-ttu-id="8ba55-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ba55-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a><span data-ttu-id="8ba55-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ba55-109">Properties</span></span>
| <span data-ttu-id="8ba55-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ba55-110">Property</span></span>     | <span data-ttu-id="8ba55-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ba55-111">Type</span></span>   |<span data-ttu-id="8ba55-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ba55-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ba55-113">displayName</span><span class="sxs-lookup"><span data-stu-id="8ba55-113">displayName</span></span>|<span data-ttu-id="8ba55-114">string</span><span class="sxs-lookup"><span data-stu-id="8ba55-114">string</span></span>|<span data-ttu-id="8ba55-115">Nome para exibição da identidade.</span><span class="sxs-lookup"><span data-stu-id="8ba55-115">The identity's display name.</span></span>|
|<span data-ttu-id="8ba55-116">id</span><span class="sxs-lookup"><span data-stu-id="8ba55-116">id</span></span>|<span data-ttu-id="8ba55-117">string</span><span class="sxs-lookup"><span data-stu-id="8ba55-117">string</span></span>|<span data-ttu-id="8ba55-118">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="8ba55-118">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteidentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
