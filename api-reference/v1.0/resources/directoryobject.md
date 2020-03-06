---
title: Tipo de recurso directoryObject
description: Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 01548a3f1be4725fad1814f4a509a13a987858e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531649"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="700b2-104">Tipo de recurso directoryObject</span><span class="sxs-lookup"><span data-stu-id="700b2-104">directoryObject resource type</span></span>

<span data-ttu-id="700b2-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="700b2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="700b2-p102">Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.</span><span class="sxs-lookup"><span data-stu-id="700b2-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="700b2-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="700b2-108">Methods</span></span>

| <span data-ttu-id="700b2-109">Método</span><span class="sxs-lookup"><span data-stu-id="700b2-109">Method</span></span>       | <span data-ttu-id="700b2-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="700b2-110">Return Type</span></span>  |<span data-ttu-id="700b2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="700b2-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="700b2-112">Get directoryObject</span><span class="sxs-lookup"><span data-stu-id="700b2-112">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="700b2-113">directoryObject</span><span class="sxs-lookup"><span data-stu-id="700b2-113">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="700b2-114">Leia as propriedades de um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="700b2-114">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="700b2-115">Delete directoryObject</span><span class="sxs-lookup"><span data-stu-id="700b2-115">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="700b2-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="700b2-116">None</span></span> |<span data-ttu-id="700b2-117">Exclua um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="700b2-117">Delete a directory object.</span></span> |
|[<span data-ttu-id="700b2-118">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="700b2-118">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="700b2-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="700b2-119">String collection</span></span>|<span data-ttu-id="700b2-p103">Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="700b2-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="700b2-122">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="700b2-122">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="700b2-123">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="700b2-123">String collection</span></span>|<span data-ttu-id="700b2-p104">Retorne todos os grupos dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="700b2-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="700b2-126">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="700b2-126">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="700b2-127">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="700b2-127">String collection</span></span>| <span data-ttu-id="700b2-p105">Retorne todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="700b2-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="700b2-130">getByIds</span><span class="sxs-lookup"><span data-stu-id="700b2-130">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="700b2-131">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="700b2-131">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="700b2-132">Obtenha um conjunto de objetos de diretório com base em um conjunto de ids fornecidas.</span><span class="sxs-lookup"><span data-stu-id="700b2-132">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="700b2-133">validateProperties</span><span class="sxs-lookup"><span data-stu-id="700b2-133">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="700b2-134">Json</span><span class="sxs-lookup"><span data-stu-id="700b2-134">Json</span></span>| <span data-ttu-id="700b2-135">Valide se o nome de exibição do grupo do Office 365 ou apelido de email está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="700b2-135">Validate that an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |

## <a name="properties"></a><span data-ttu-id="700b2-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="700b2-136">Properties</span></span>

| <span data-ttu-id="700b2-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="700b2-137">Property</span></span>   | <span data-ttu-id="700b2-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="700b2-138">Type</span></span> |<span data-ttu-id="700b2-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="700b2-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="700b2-140">id</span><span class="sxs-lookup"><span data-stu-id="700b2-140">id</span></span>|<span data-ttu-id="700b2-141">String</span><span class="sxs-lookup"><span data-stu-id="700b2-141">String</span></span>|<span data-ttu-id="700b2-p106">Um GUID que é o identificador exclusivo do objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde. Chave. Não anulável. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="700b2-p106">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="700b2-146">Relações</span><span class="sxs-lookup"><span data-stu-id="700b2-146">Relationships</span></span>

<span data-ttu-id="700b2-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="700b2-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="700b2-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="700b2-148">JSON representation</span></span>

<span data-ttu-id="700b2-149">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="700b2-149">Here is a JSON representation of the resource</span></span>

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
