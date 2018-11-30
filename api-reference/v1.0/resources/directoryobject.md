---
title: Tipo de recurso directoryObject
description: Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.
ms.openlocfilehash: 0981584bb86b71d06e29de4efc379c84bacac51d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007140"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="79930-104">Tipo de recurso directoryObject</span><span class="sxs-lookup"><span data-stu-id="79930-104">directoryObject resource type</span></span>

<span data-ttu-id="79930-p102">Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.</span><span class="sxs-lookup"><span data-stu-id="79930-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="79930-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="79930-107">Methods</span></span>

| <span data-ttu-id="79930-108">Método</span><span class="sxs-lookup"><span data-stu-id="79930-108">Method</span></span>       | <span data-ttu-id="79930-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="79930-109">Return Type</span></span>  |<span data-ttu-id="79930-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="79930-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="79930-111">Get directoryObject</span><span class="sxs-lookup"><span data-stu-id="79930-111">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="79930-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="79930-112">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="79930-113">Leia as propriedades de um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="79930-113">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="79930-114">Delete directoryObject</span><span class="sxs-lookup"><span data-stu-id="79930-114">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="79930-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79930-115">None</span></span> |<span data-ttu-id="79930-116">Exclua um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="79930-116">Delete a directory object.</span></span> |
|[<span data-ttu-id="79930-117">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="79930-117">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="79930-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="79930-118">String collection</span></span>|<span data-ttu-id="79930-p103">Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="79930-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="79930-121">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="79930-121">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="79930-122">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="79930-122">String collection</span></span>|<span data-ttu-id="79930-p104">Retorne todos os grupos dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="79930-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="79930-125">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="79930-125">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="79930-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="79930-126">String collection</span></span>| <span data-ttu-id="79930-p105">Retorne todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="79930-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="79930-129">getByIds</span><span class="sxs-lookup"><span data-stu-id="79930-129">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="79930-130">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="79930-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="79930-131">Obtenha um conjunto de objetos de diretório com base em um conjunto de ids fornecidas.</span><span class="sxs-lookup"><span data-stu-id="79930-131">Get a set of directory objects based on a set of supplied ids.</span></span> |

## <a name="properties"></a><span data-ttu-id="79930-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79930-132">Properties</span></span>

| <span data-ttu-id="79930-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79930-133">Property</span></span>   | <span data-ttu-id="79930-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="79930-134">Type</span></span> |<span data-ttu-id="79930-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="79930-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79930-136">id</span><span class="sxs-lookup"><span data-stu-id="79930-136">id</span></span>|<span data-ttu-id="79930-137">String</span><span class="sxs-lookup"><span data-stu-id="79930-137">String</span></span>|<span data-ttu-id="79930-p106">Um GUID que é o identificador exclusivo do objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde. Chave. Não anulável. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="79930-p106">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79930-142">Relações</span><span class="sxs-lookup"><span data-stu-id="79930-142">Relationships</span></span>

<span data-ttu-id="79930-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79930-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="79930-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79930-144">JSON representation</span></span>

<span data-ttu-id="79930-145">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="79930-145">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directoryObject",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
