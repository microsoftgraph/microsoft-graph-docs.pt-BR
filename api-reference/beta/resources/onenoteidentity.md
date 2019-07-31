---
title: tipo de recurso oneNoteIdentity
description: '**Suporte em breve**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 0a7df80dd3dcd4f4b93edb4e708e65de3f74d775
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966444"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="892db-103">tipo de recurso oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="892db-103">oneNoteIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="892db-104">**Suporte em breve**</span><span class="sxs-lookup"><span data-stu-id="892db-104">**Support coming soon**</span></span>

<span data-ttu-id="892db-105">O tipo OneNoteIdentity representa uma identidade de um _usuário_.</span><span class="sxs-lookup"><span data-stu-id="892db-105">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="892db-106">No futuro, este tipo será mesclado com a [identidade](identity.md)</span><span class="sxs-lookup"><span data-stu-id="892db-106">In future, this type will be merged with [identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="892db-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="892db-107">JSON representation</span></span>

<span data-ttu-id="892db-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="892db-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a><span data-ttu-id="892db-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="892db-109">Properties</span></span>
| <span data-ttu-id="892db-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="892db-110">Property</span></span>     | <span data-ttu-id="892db-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="892db-111">Type</span></span>   |<span data-ttu-id="892db-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="892db-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="892db-113">displayName</span><span class="sxs-lookup"><span data-stu-id="892db-113">displayName</span></span>|<span data-ttu-id="892db-114">string</span><span class="sxs-lookup"><span data-stu-id="892db-114">string</span></span>|<span data-ttu-id="892db-115">Nome de exibição da identidade.</span><span class="sxs-lookup"><span data-stu-id="892db-115">The identity's display name.</span></span>|
|<span data-ttu-id="892db-116">id</span><span class="sxs-lookup"><span data-stu-id="892db-116">id</span></span>|<span data-ttu-id="892db-117">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="892db-117">string</span></span>|<span data-ttu-id="892db-118">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="892db-118">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
