---
title: tipo de recurso oneNoteIdentitySet
description: '**Suporte em breve**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: c0d2f0b4ed65ac83a59036c362136b7af772d21c
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290578"
---
# <a name="onenoteidentityset-resource-type"></a><span data-ttu-id="b694c-103">tipo de recurso oneNoteIdentitySet</span><span class="sxs-lookup"><span data-stu-id="b694c-103">oneNoteIdentitySet resource type</span></span>

<span data-ttu-id="b694c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b694c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b694c-105">**Suporte em breve**</span><span class="sxs-lookup"><span data-stu-id="b694c-105">**Support coming soon**</span></span>

<span data-ttu-id="b694c-106">O tipo OneNoteIdentitySet é uma coleção com chave de objetos [OneNoteIdentity](onenoteidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="b694c-106">The OneNoteIdentitySet type is a keyed collection of [OneNoteIdentity](onenoteidentity.md) objects.</span></span>
<span data-ttu-id="b694c-107">É usado para representar um conjunto de identidades associadas a vários eventos para um _bloco de anotações_, uma _seção_ ou uma _página_, como _criado por_ ou _modificado pela última vez por_.</span><span class="sxs-lookup"><span data-stu-id="b694c-107">It is used to represent a set of identities associated with various events for a _Notebook_, _Section_ or _Page_, such as _created by_ or _last modified by_.</span></span> 
 
<span data-ttu-id="b694c-108">Atualmente, ele contém uma única chave, _**User**_.</span><span class="sxs-lookup"><span data-stu-id="b694c-108">Currently it contains a single key, _**user**_.</span></span>  <span data-ttu-id="b694c-109">No futuro, chaves como o dispositivo ou aplicativo para alterar o item podem ser adicionadas.</span><span class="sxs-lookup"><span data-stu-id="b694c-109">In future, keys such as the device or application to change the item may be added.</span></span>

<span data-ttu-id="b694c-110">No futuro, esse tipo será mesclado com [identityset](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="b694c-110">In future, this type will be merged with [IdentitySet](identityset.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="b694c-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b694c-111">JSON representation</span></span>

<span data-ttu-id="b694c-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b694c-112">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="b694c-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b694c-113">Properties</span></span>
| <span data-ttu-id="b694c-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b694c-114">Property</span></span>     | <span data-ttu-id="b694c-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="b694c-115">Type</span></span>   |<span data-ttu-id="b694c-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="b694c-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b694c-117">user</span><span class="sxs-lookup"><span data-stu-id="b694c-117">user</span></span>|[<span data-ttu-id="b694c-118">onenoteIdentity</span><span class="sxs-lookup"><span data-stu-id="b694c-118">onenoteIdentity</span></span>](onenoteidentity.md)|<span data-ttu-id="b694c-119">Um recurso OneNoteIdentity que representa um usuário.</span><span class="sxs-lookup"><span data-stu-id="b694c-119">A OneNoteIdentity resource that represents a user.</span></span>|

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
