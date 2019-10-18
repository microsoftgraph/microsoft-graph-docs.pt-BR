---
title: Tipo de recurso directoryObject
description: Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c1b462b001c9ccecfb792b705506a5b43f8b0254
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032736"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="a8b21-104">Tipo de recurso directoryObject</span><span class="sxs-lookup"><span data-stu-id="a8b21-104">directoryObject resource type</span></span>

<span data-ttu-id="a8b21-p102">Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.</span><span class="sxs-lookup"><span data-stu-id="a8b21-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="a8b21-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a8b21-107">Methods</span></span>

| <span data-ttu-id="a8b21-108">Método</span><span class="sxs-lookup"><span data-stu-id="a8b21-108">Method</span></span>       | <span data-ttu-id="a8b21-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a8b21-109">Return Type</span></span>  |<span data-ttu-id="a8b21-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8b21-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a8b21-111">Get directoryObject</span><span class="sxs-lookup"><span data-stu-id="a8b21-111">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="a8b21-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="a8b21-112">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="a8b21-113">Leia as propriedades de um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="a8b21-113">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="a8b21-114">Delete directoryObject</span><span class="sxs-lookup"><span data-stu-id="a8b21-114">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="a8b21-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8b21-115">None</span></span> |<span data-ttu-id="a8b21-116">Exclua um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="a8b21-116">Delete a directory object.</span></span> |
|[<span data-ttu-id="a8b21-117">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="a8b21-117">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="a8b21-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8b21-118">String collection</span></span>|<span data-ttu-id="a8b21-p103">Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="a8b21-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="a8b21-121">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="a8b21-121">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="a8b21-122">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8b21-122">String collection</span></span>|<span data-ttu-id="a8b21-p104">Retorne todos os grupos dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="a8b21-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="a8b21-125">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="a8b21-125">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="a8b21-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8b21-126">String collection</span></span>| <span data-ttu-id="a8b21-p105">Retorne todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="a8b21-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="a8b21-129">getByIds</span><span class="sxs-lookup"><span data-stu-id="a8b21-129">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="a8b21-130">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a8b21-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="a8b21-131">Obtenha um conjunto de objetos de diretório com base em um conjunto de ids fornecidas.</span><span class="sxs-lookup"><span data-stu-id="a8b21-131">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="a8b21-132">validateProperties</span><span class="sxs-lookup"><span data-stu-id="a8b21-132">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="a8b21-133">Json</span><span class="sxs-lookup"><span data-stu-id="a8b21-133">Json</span></span>| <span data-ttu-id="a8b21-134">Valide se o nome de exibição do grupo do Office 365 ou apelido de email está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="a8b21-134">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |

## <a name="properties"></a><span data-ttu-id="a8b21-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8b21-135">Properties</span></span>

| <span data-ttu-id="a8b21-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8b21-136">Property</span></span>   | <span data-ttu-id="a8b21-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8b21-137">Type</span></span> |<span data-ttu-id="a8b21-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8b21-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8b21-139">id</span><span class="sxs-lookup"><span data-stu-id="a8b21-139">id</span></span>|<span data-ttu-id="a8b21-140">String</span><span class="sxs-lookup"><span data-stu-id="a8b21-140">String</span></span>|<span data-ttu-id="a8b21-p106">Um GUID que é o identificador exclusivo do objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde. Chave. Não anulável. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a8b21-p106">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8b21-145">Relações</span><span class="sxs-lookup"><span data-stu-id="a8b21-145">Relationships</span></span>

<span data-ttu-id="a8b21-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8b21-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a8b21-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8b21-147">JSON representation</span></span>

<span data-ttu-id="a8b21-148">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a8b21-148">Here is a JSON representation of the resource</span></span>

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
