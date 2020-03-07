---
title: Tipo de recurso directoryObject
description: Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b90e81a9337cef51af4bfded50eaaf494e4ebca7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507027"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="10c9c-104">Tipo de recurso directoryObject</span><span class="sxs-lookup"><span data-stu-id="10c9c-104">directoryObject resource type</span></span>

<span data-ttu-id="10c9c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10c9c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10c9c-p102">Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.</span><span class="sxs-lookup"><span data-stu-id="10c9c-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="10c9c-108">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="10c9c-108">This resource supports:</span></span>

- <span data-ttu-id="10c9c-109">Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryobject-delta.md).</span><span class="sxs-lookup"><span data-stu-id="10c9c-109">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="10c9c-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="10c9c-110">Methods</span></span>

| <span data-ttu-id="10c9c-111">Método</span><span class="sxs-lookup"><span data-stu-id="10c9c-111">Method</span></span>       | <span data-ttu-id="10c9c-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="10c9c-112">Return Type</span></span>  |<span data-ttu-id="10c9c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="10c9c-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="10c9c-114">Get directoryObject</span><span class="sxs-lookup"><span data-stu-id="10c9c-114">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="10c9c-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="10c9c-115">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="10c9c-116">Leia as propriedades de um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="10c9c-116">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="10c9c-117">Delete</span><span class="sxs-lookup"><span data-stu-id="10c9c-117">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="10c9c-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10c9c-118">None</span></span> |<span data-ttu-id="10c9c-119">Exclua um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="10c9c-119">Delete a directory object.</span></span> |
|[<span data-ttu-id="10c9c-120">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="10c9c-120">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="10c9c-121">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="10c9c-121">String collection</span></span>|<span data-ttu-id="10c9c-p103">Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="10c9c-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="10c9c-124">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="10c9c-124">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="10c9c-125">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="10c9c-125">String collection</span></span>|<span data-ttu-id="10c9c-p104">Retorne todos os grupos dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="10c9c-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="10c9c-128">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="10c9c-128">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="10c9c-129">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="10c9c-129">String collection</span></span>| <span data-ttu-id="10c9c-p105">Retorne todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="10c9c-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="10c9c-132">getByIds</span><span class="sxs-lookup"><span data-stu-id="10c9c-132">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="10c9c-133">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="10c9c-133">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="10c9c-134">Obtenha um conjunto de objetos de diretório com base em um conjunto de ids fornecidas.</span><span class="sxs-lookup"><span data-stu-id="10c9c-134">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="10c9c-135">validateProperties</span><span class="sxs-lookup"><span data-stu-id="10c9c-135">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="10c9c-136">Json</span><span class="sxs-lookup"><span data-stu-id="10c9c-136">Json</span></span>| <span data-ttu-id="10c9c-137">Validar um nome de exibição ou um apelido de email do grupo do Office 365 em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="10c9c-137">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="10c9c-138">delta</span><span class="sxs-lookup"><span data-stu-id="10c9c-138">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="10c9c-139">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="10c9c-139">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="10c9c-140">Obtenha alterações incrementais para objetos de diretório.</span><span class="sxs-lookup"><span data-stu-id="10c9c-140">Get incremental changes for directory objects.</span></span> <span data-ttu-id="10c9c-141">Oferece suporte à filtragem por tipo derivado.</span><span class="sxs-lookup"><span data-stu-id="10c9c-141">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="10c9c-142">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10c9c-142">Properties</span></span>

| <span data-ttu-id="10c9c-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10c9c-143">Property</span></span>   | <span data-ttu-id="10c9c-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="10c9c-144">Type</span></span> |<span data-ttu-id="10c9c-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="10c9c-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10c9c-146">id</span><span class="sxs-lookup"><span data-stu-id="10c9c-146">id</span></span>|<span data-ttu-id="10c9c-147">String</span><span class="sxs-lookup"><span data-stu-id="10c9c-147">String</span></span>|<span data-ttu-id="10c9c-148">Um Guid que é o identificador exclusivo do objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde12.</span><span class="sxs-lookup"><span data-stu-id="10c9c-148">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde12.</span></span> <span data-ttu-id="10c9c-149">Chave.</span><span class="sxs-lookup"><span data-stu-id="10c9c-149">Key.</span></span> <span data-ttu-id="10c9c-150">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="10c9c-150">Not nullable.</span></span> <span data-ttu-id="10c9c-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="10c9c-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10c9c-152">Relações</span><span class="sxs-lookup"><span data-stu-id="10c9c-152">Relationships</span></span>

<span data-ttu-id="10c9c-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10c9c-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10c9c-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10c9c-154">JSON representation</span></span>

<span data-ttu-id="10c9c-155">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="10c9c-155">Here is a JSON representation of the resource</span></span>

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
