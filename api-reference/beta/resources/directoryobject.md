---
title: Tipo de recurso directoryObject
description: Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.
localization_priority: Priority
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 19afac29a257dac404bcd8d006462aea7ba5c4b0
ms.sourcegitcommit: c4366ac71cf496242c8ff435bc8d8b3816bdc1aa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2020
ms.locfileid: "47287460"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="676bb-104">Tipo de recurso directoryObject</span><span class="sxs-lookup"><span data-stu-id="676bb-104">directoryObject resource type</span></span>

<span data-ttu-id="676bb-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="676bb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="676bb-p102">Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.</span><span class="sxs-lookup"><span data-stu-id="676bb-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="676bb-108">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="676bb-108">This resource supports:</span></span>

- <span data-ttu-id="676bb-109">Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryobject-delta.md).</span><span class="sxs-lookup"><span data-stu-id="676bb-109">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="676bb-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="676bb-110">Methods</span></span>

| <span data-ttu-id="676bb-111">Método</span><span class="sxs-lookup"><span data-stu-id="676bb-111">Method</span></span>       | <span data-ttu-id="676bb-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="676bb-112">Return Type</span></span>  |<span data-ttu-id="676bb-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="676bb-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="676bb-114">Get directoryObject</span><span class="sxs-lookup"><span data-stu-id="676bb-114">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="676bb-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="676bb-115">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="676bb-116">Leia as propriedades de um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="676bb-116">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="676bb-117">Delete</span><span class="sxs-lookup"><span data-stu-id="676bb-117">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="676bb-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="676bb-118">None</span></span> |<span data-ttu-id="676bb-119">Exclua um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="676bb-119">Delete a directory object.</span></span> |
|[<span data-ttu-id="676bb-120">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="676bb-120">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="676bb-121">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="676bb-121">String collection</span></span>|<span data-ttu-id="676bb-p103">Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="676bb-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="676bb-124">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="676bb-124">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="676bb-125">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="676bb-125">String collection</span></span>|<span data-ttu-id="676bb-p104">Retorne todos os grupos dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="676bb-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="676bb-128">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="676bb-128">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="676bb-129">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="676bb-129">String collection</span></span>| <span data-ttu-id="676bb-p105">Retorne todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="676bb-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="676bb-132">getByIds</span><span class="sxs-lookup"><span data-stu-id="676bb-132">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="676bb-133">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="676bb-133">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="676bb-134">Obtenha um conjunto de objetos de diretório com base em um conjunto de ids fornecidas.</span><span class="sxs-lookup"><span data-stu-id="676bb-134">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="676bb-135">validateProperties</span><span class="sxs-lookup"><span data-stu-id="676bb-135">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="676bb-136">Json</span><span class="sxs-lookup"><span data-stu-id="676bb-136">Json</span></span>| <span data-ttu-id="676bb-137">Validar se o nome de exibição de um grupo do Microsoft 365 ou apelido de email está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="676bb-137">Validate a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="676bb-138">delta</span><span class="sxs-lookup"><span data-stu-id="676bb-138">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="676bb-139">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="676bb-139">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="676bb-140">Obtenha alterações incrementais para objetos de diretório.</span><span class="sxs-lookup"><span data-stu-id="676bb-140">Get incremental changes for directory objects.</span></span> <span data-ttu-id="676bb-141">Oferece suporte à filtragem por tipo derivado.</span><span class="sxs-lookup"><span data-stu-id="676bb-141">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="676bb-142">Propriedades</span><span class="sxs-lookup"><span data-stu-id="676bb-142">Properties</span></span>

| <span data-ttu-id="676bb-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="676bb-143">Property</span></span>   | <span data-ttu-id="676bb-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="676bb-144">Type</span></span> |<span data-ttu-id="676bb-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="676bb-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="676bb-146">id</span><span class="sxs-lookup"><span data-stu-id="676bb-146">id</span></span>|<span data-ttu-id="676bb-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="676bb-147">String</span></span>|<span data-ttu-id="676bb-148">O identificador exclusivo para o objeto.</span><span class="sxs-lookup"><span data-stu-id="676bb-148">The unique identifier for the object.</span></span> <span data-ttu-id="676bb-149">Por exemplo, 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="676bb-149">For example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="676bb-150">O valor da propriedade **ID** é frequentemente, mas não exclusivamente, sob o formato de um GUID; O valor deve ser tratado como um identificador opaco e não confie no fato de ser um GUID.</span><span class="sxs-lookup"><span data-stu-id="676bb-150">The value of the **id** property is often but not exclusively in the form of a GUID; treat it as an opaque identifier and do not rely on it being a GUID.</span></span> <span data-ttu-id="676bb-151">Chave.</span><span class="sxs-lookup"><span data-stu-id="676bb-151">Key.</span></span> <span data-ttu-id="676bb-152">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="676bb-152">Not nullable.</span></span> <span data-ttu-id="676bb-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="676bb-153">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="676bb-154">Relações</span><span class="sxs-lookup"><span data-stu-id="676bb-154">Relationships</span></span>

<span data-ttu-id="676bb-155">Nenhum</span><span class="sxs-lookup"><span data-stu-id="676bb-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="676bb-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="676bb-156">JSON representation</span></span>

<span data-ttu-id="676bb-157">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="676bb-157">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject",
  "openType": true
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
