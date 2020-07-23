---
title: Tipo de recurso directoryObject
description: Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.
localization_priority: Priority
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4e690598a9e93dbbbc7527bbfcd8864e0b800bc5
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2020
ms.locfileid: "45225099"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="e9344-104">Tipo de recurso directoryObject</span><span class="sxs-lookup"><span data-stu-id="e9344-104">directoryObject resource type</span></span>

<span data-ttu-id="e9344-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9344-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e9344-p102">Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.</span><span class="sxs-lookup"><span data-stu-id="e9344-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="e9344-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="e9344-108">Methods</span></span>

| <span data-ttu-id="e9344-109">Método</span><span class="sxs-lookup"><span data-stu-id="e9344-109">Method</span></span>       | <span data-ttu-id="e9344-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e9344-110">Return Type</span></span>  |<span data-ttu-id="e9344-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9344-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e9344-112">Get directoryObject</span><span class="sxs-lookup"><span data-stu-id="e9344-112">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="e9344-113">directoryObject</span><span class="sxs-lookup"><span data-stu-id="e9344-113">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="e9344-114">Leia as propriedades de um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="e9344-114">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="e9344-115">Delete directoryObject</span><span class="sxs-lookup"><span data-stu-id="e9344-115">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="e9344-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e9344-116">None</span></span> |<span data-ttu-id="e9344-117">Exclua um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="e9344-117">Delete a directory object.</span></span> |
|[<span data-ttu-id="e9344-118">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="e9344-118">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="e9344-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9344-119">String collection</span></span>|<span data-ttu-id="e9344-p103">Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="e9344-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="e9344-122">Obtenha as propriedades de extensão disponíveis</span><span class="sxs-lookup"><span data-stu-id="e9344-122">Get available extension properties</span></span>](../api/directoryobject-getavailableextensionproperties.md)|<span data-ttu-id="e9344-123">Coleção [extensionProperty](../resources/extensionproperty.md)</span><span class="sxs-lookup"><span data-stu-id="e9344-123">[extensionProperty](../resources/extensionproperty.md) collection</span></span>|<span data-ttu-id="e9344-124">Obtenha todas as listas ou uma lista filtrada das propriedades de extensão do diretório que foram registradas em um diretório.</span><span class="sxs-lookup"><span data-stu-id="e9344-124">Get all or a filtered list of the directory extension properties that have been registered in a directory.</span></span>|
|[<span data-ttu-id="e9344-125">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="e9344-125">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="e9344-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9344-126">String collection</span></span>|<span data-ttu-id="e9344-p104">Retorne todos os grupos dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="e9344-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="e9344-129">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="e9344-129">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="e9344-130">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9344-130">String collection</span></span>| <span data-ttu-id="e9344-p105">Retorne todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="e9344-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="e9344-133">getByIds</span><span class="sxs-lookup"><span data-stu-id="e9344-133">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="e9344-134">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e9344-134">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="e9344-135">Obtenha um conjunto de objetos de diretório com base em um conjunto de ids fornecidas.</span><span class="sxs-lookup"><span data-stu-id="e9344-135">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="e9344-136">validateProperties</span><span class="sxs-lookup"><span data-stu-id="e9344-136">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="e9344-137">Json</span><span class="sxs-lookup"><span data-stu-id="e9344-137">Json</span></span>| <span data-ttu-id="e9344-138">Valide se o nome de exibição ou apelido de email de um grupo da Microsoft 365 está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="e9344-138">Validate that a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span> |

## <a name="properties"></a><span data-ttu-id="e9344-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e9344-139">Properties</span></span>

| <span data-ttu-id="e9344-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9344-140">Property</span></span>   | <span data-ttu-id="e9344-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9344-141">Type</span></span> |<span data-ttu-id="e9344-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9344-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9344-143">id</span><span class="sxs-lookup"><span data-stu-id="e9344-143">id</span></span>|<span data-ttu-id="e9344-144">String</span><span class="sxs-lookup"><span data-stu-id="e9344-144">String</span></span>|<span data-ttu-id="e9344-p106">Um GUID que é o identificador exclusivo do objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde. Chave. Não anulável. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e9344-p106">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9344-149">Relações</span><span class="sxs-lookup"><span data-stu-id="e9344-149">Relationships</span></span>

<span data-ttu-id="e9344-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e9344-150">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e9344-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e9344-151">JSON representation</span></span>

<span data-ttu-id="e9344-152">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e9344-152">Here is a JSON representation of the resource</span></span>

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
