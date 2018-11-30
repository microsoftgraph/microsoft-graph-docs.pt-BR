---
title: tipo de recurso de oneNoteIdentitySet
description: '**Suporte em breve**'
ms.openlocfilehash: bbfd49c1ea4c0af7812ec67f40490ed8627a65a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034330"
---
# <a name="onenoteidentityset-resource-type"></a><span data-ttu-id="5d188-103">tipo de recurso de oneNoteIdentitySet</span><span class="sxs-lookup"><span data-stu-id="5d188-103">oneNoteIdentitySet resource type</span></span>

> <span data-ttu-id="5d188-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5d188-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d188-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5d188-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5d188-106">**Suporte em breve**</span><span class="sxs-lookup"><span data-stu-id="5d188-106">**Support coming soon**</span></span>

<span data-ttu-id="5d188-107">O tipo de OneNoteIdentitySet é uma coleção com chave de objetos [OneNoteIdentity](onenoteidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="5d188-107">The OneNoteIdentitySet type is a keyed collection of [OneNoteIdentity](onenoteidentity.md) objects.</span></span>
<span data-ttu-id="5d188-108">Ele é usado para representar um conjunto de identidades associado a vários eventos para um _Bloco de anotações_, _seção_ ou da _página_, como _criado por_ ou _modificado pela última vez_.</span><span class="sxs-lookup"><span data-stu-id="5d188-108">It is used to represent a set of identities associated with various events for a _Notebook_, _Section_ or _Page_, such as _created by_ or _last modified by_.</span></span> 
 
<span data-ttu-id="5d188-109">Atualmente, ele contém um único _**usuário**_ de chave.</span><span class="sxs-lookup"><span data-stu-id="5d188-109">Currently it contains a single key, _**user**_.</span></span>  <span data-ttu-id="5d188-110">No futuro, chaves, como o dispositivo ou aplicativo para alterar o item podem ser adicionadas.</span><span class="sxs-lookup"><span data-stu-id="5d188-110">In future, keys such as the device or application to change the item may be added.</span></span>

<span data-ttu-id="5d188-111">No futuro, esse tipo de será mesclado com [IdentitySet](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="5d188-111">In future, this type will be merged with [IdentitySet](identityset.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d188-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5d188-112">JSON representation</span></span>

<span data-ttu-id="5d188-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5d188-113">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.oneNoteIdentity"}
}

```
## <a name="properties"></a><span data-ttu-id="5d188-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5d188-114">Properties</span></span>
| <span data-ttu-id="5d188-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d188-115">Property</span></span>     | <span data-ttu-id="5d188-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d188-116">Type</span></span>   |<span data-ttu-id="5d188-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d188-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d188-118">user</span><span class="sxs-lookup"><span data-stu-id="5d188-118">user</span></span>|[<span data-ttu-id="5d188-119">oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="5d188-119">oneNoteIdentity</span></span>](onenoteidentity.md)|<span data-ttu-id="5d188-120">Um recurso de OneNoteIdentity que representa um usuário.</span><span class="sxs-lookup"><span data-stu-id="5d188-120">A OneNoteIdentity resource that represents a user.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
