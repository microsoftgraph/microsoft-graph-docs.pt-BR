---
title: tipo de recurso oneNoteIdentitySet
description: '**Suporte em breve**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 49aadd4609e214937e02dd21238110addb9ed2ea
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341780"
---
# <a name="onenoteidentityset-resource-type"></a><span data-ttu-id="47184-103">tipo de recurso oneNoteIdentitySet</span><span class="sxs-lookup"><span data-stu-id="47184-103">oneNoteIdentitySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47184-104">**Suporte em breve**</span><span class="sxs-lookup"><span data-stu-id="47184-104">**Support coming soon**</span></span>

<span data-ttu-id="47184-105">O tipo OneNoteIdentitySet é uma coleção com chave de objetos [OneNoteIdentity](onenoteidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="47184-105">The OneNoteIdentitySet type is a keyed collection of [OneNoteIdentity](onenoteidentity.md) objects.</span></span>
<span data-ttu-id="47184-106">É usado para representar um conjunto de identidades associadas a vários eventos para um _bloco de anotações_, uma _seção_ ou uma _página_, como _criado por_ ou _modificado pela última vez por_.</span><span class="sxs-lookup"><span data-stu-id="47184-106">It is used to represent a set of identities associated with various events for a _Notebook_, _Section_ or _Page_, such as _created by_ or _last modified by_.</span></span> 
 
<span data-ttu-id="47184-107">Atualmente, ele contém uma única chave, _**User**_.</span><span class="sxs-lookup"><span data-stu-id="47184-107">Currently it contains a single key, _**user**_.</span></span>  <span data-ttu-id="47184-108">No futuro, chaves como o dispositivo ou aplicativo para alterar o item podem ser adicionadas.</span><span class="sxs-lookup"><span data-stu-id="47184-108">In future, keys such as the device or application to change the item may be added.</span></span>

<span data-ttu-id="47184-109">No futuro, esse tipo será mesclado com [identityset](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="47184-109">In future, this type will be merged with [IdentitySet](identityset.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="47184-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47184-110">JSON representation</span></span>

<span data-ttu-id="47184-111">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47184-111">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteIdentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.onenoteIdentity"}
}

```
## <a name="properties"></a><span data-ttu-id="47184-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47184-112">Properties</span></span>
| <span data-ttu-id="47184-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47184-113">Property</span></span>     | <span data-ttu-id="47184-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="47184-114">Type</span></span>   |<span data-ttu-id="47184-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="47184-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47184-116">user</span><span class="sxs-lookup"><span data-stu-id="47184-116">user</span></span>|[<span data-ttu-id="47184-117">oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="47184-117">oneNoteIdentity</span></span>](onenoteidentity.md)|<span data-ttu-id="47184-118">Um recurso OneNoteIdentity que representa um usuário.</span><span class="sxs-lookup"><span data-stu-id="47184-118">A OneNoteIdentity resource that represents a user.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
