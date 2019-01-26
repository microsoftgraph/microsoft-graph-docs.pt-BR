---
title: tipo de recurso de oneNoteIdentitySet
description: '**Suporte em breve**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: dc8256cb2459ae23fcdae9e2e658394df899a134
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577288"
---
# <a name="onenoteidentityset-resource-type"></a><span data-ttu-id="68e98-103">tipo de recurso de oneNoteIdentitySet</span><span class="sxs-lookup"><span data-stu-id="68e98-103">oneNoteIdentitySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68e98-104">**Suporte em breve**</span><span class="sxs-lookup"><span data-stu-id="68e98-104">**Support coming soon**</span></span>

<span data-ttu-id="68e98-105">O tipo de OneNoteIdentitySet é uma coleção com chave de objetos [OneNoteIdentity](onenoteidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="68e98-105">The OneNoteIdentitySet type is a keyed collection of [OneNoteIdentity](onenoteidentity.md) objects.</span></span>
<span data-ttu-id="68e98-106">Ele é usado para representar um conjunto de identidades associado a vários eventos para um _Bloco de anotações_, _seção_ ou da _página_, como _criado por_ ou _modificado pela última vez_.</span><span class="sxs-lookup"><span data-stu-id="68e98-106">It is used to represent a set of identities associated with various events for a _Notebook_, _Section_ or _Page_, such as _created by_ or _last modified by_.</span></span> 
 
<span data-ttu-id="68e98-107">Atualmente, ele contém um único _**usuário**_ de chave.</span><span class="sxs-lookup"><span data-stu-id="68e98-107">Currently it contains a single key, _**user**_.</span></span>  <span data-ttu-id="68e98-108">No futuro, chaves, como o dispositivo ou aplicativo para alterar o item podem ser adicionadas.</span><span class="sxs-lookup"><span data-stu-id="68e98-108">In future, keys such as the device or application to change the item may be added.</span></span>

<span data-ttu-id="68e98-109">No futuro, esse tipo de será mesclado com [IdentitySet](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="68e98-109">In future, this type will be merged with [IdentitySet](identityset.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="68e98-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68e98-110">JSON representation</span></span>

<span data-ttu-id="68e98-111">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68e98-111">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oneNoteIdentitySet"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.oneNoteIdentity"}
}

```
## <a name="properties"></a><span data-ttu-id="68e98-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68e98-112">Properties</span></span>
| <span data-ttu-id="68e98-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68e98-113">Property</span></span>     | <span data-ttu-id="68e98-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="68e98-114">Type</span></span>   |<span data-ttu-id="68e98-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="68e98-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68e98-116">user</span><span class="sxs-lookup"><span data-stu-id="68e98-116">user</span></span>|[<span data-ttu-id="68e98-117">oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="68e98-117">oneNoteIdentity</span></span>](onenoteidentity.md)|<span data-ttu-id="68e98-118">Um recurso de OneNoteIdentity que representa um usuário.</span><span class="sxs-lookup"><span data-stu-id="68e98-118">A OneNoteIdentity resource that represents a user.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteidentityset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
