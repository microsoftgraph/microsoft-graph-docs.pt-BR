---
title: Tipo de recurso directoryObject
description: Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.
localization_priority: Priority
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7ae5c016bcc6ccb317a56b1d248c8450703d5d34
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013838"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="7a8d2-104">Tipo de recurso directoryObject</span><span class="sxs-lookup"><span data-stu-id="7a8d2-104">directoryObject resource type</span></span>

<span data-ttu-id="7a8d2-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a8d2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a8d2-p102">Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.</span><span class="sxs-lookup"><span data-stu-id="7a8d2-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="7a8d2-108">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="7a8d2-108">This resource supports:</span></span>

- <span data-ttu-id="7a8d2-109">Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryobject-delta.md).</span><span class="sxs-lookup"><span data-stu-id="7a8d2-109">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="7a8d2-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="7a8d2-110">Methods</span></span>

| <span data-ttu-id="7a8d2-111">Método</span><span class="sxs-lookup"><span data-stu-id="7a8d2-111">Method</span></span>       | <span data-ttu-id="7a8d2-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7a8d2-112">Return Type</span></span>  |<span data-ttu-id="7a8d2-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a8d2-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7a8d2-114">Get directoryObject</span><span class="sxs-lookup"><span data-stu-id="7a8d2-114">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="7a8d2-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="7a8d2-115">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="7a8d2-116">Leia as propriedades de um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="7a8d2-116">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="7a8d2-117">Delete</span><span class="sxs-lookup"><span data-stu-id="7a8d2-117">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="7a8d2-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7a8d2-118">None</span></span> |<span data-ttu-id="7a8d2-119">Exclua um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="7a8d2-119">Delete a directory object.</span></span> |
|[<span data-ttu-id="7a8d2-120">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="7a8d2-120">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="7a8d2-121">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a8d2-121">String collection</span></span>|<span data-ttu-id="7a8d2-p103">Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="7a8d2-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="7a8d2-124">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="7a8d2-124">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="7a8d2-125">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a8d2-125">String collection</span></span>|<span data-ttu-id="7a8d2-p104">Retorne todos os grupos dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="7a8d2-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="7a8d2-128">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="7a8d2-128">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="7a8d2-129">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a8d2-129">String collection</span></span>| <span data-ttu-id="7a8d2-p105">Retorne todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="7a8d2-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="7a8d2-132">getByIds</span><span class="sxs-lookup"><span data-stu-id="7a8d2-132">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="7a8d2-133">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="7a8d2-133">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="7a8d2-134">Obtenha um conjunto de objetos de diretório com base em um conjunto de ids fornecidas.</span><span class="sxs-lookup"><span data-stu-id="7a8d2-134">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="7a8d2-135">validateProperties</span><span class="sxs-lookup"><span data-stu-id="7a8d2-135">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="7a8d2-136">Json</span><span class="sxs-lookup"><span data-stu-id="7a8d2-136">Json</span></span>| <span data-ttu-id="7a8d2-137">Validar se o nome de exibição de um grupo do Microsoft 365 ou apelido de email está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="7a8d2-137">Validate a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="7a8d2-138">delta</span><span class="sxs-lookup"><span data-stu-id="7a8d2-138">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="7a8d2-139">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="7a8d2-139">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="7a8d2-140">Obtenha alterações incrementais para objetos de diretório.</span><span class="sxs-lookup"><span data-stu-id="7a8d2-140">Get incremental changes for directory objects.</span></span> <span data-ttu-id="7a8d2-141">Oferece suporte à filtragem por tipo derivado.</span><span class="sxs-lookup"><span data-stu-id="7a8d2-141">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="7a8d2-142">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a8d2-142">Properties</span></span>

| <span data-ttu-id="7a8d2-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a8d2-143">Property</span></span>   | <span data-ttu-id="7a8d2-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a8d2-144">Type</span></span> |<span data-ttu-id="7a8d2-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a8d2-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a8d2-146">id</span><span class="sxs-lookup"><span data-stu-id="7a8d2-146">id</span></span>|<span data-ttu-id="7a8d2-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a8d2-147">String</span></span>|<span data-ttu-id="7a8d2-148">O identificador exclusivo para o objeto.</span><span class="sxs-lookup"><span data-stu-id="7a8d2-148">The unique identifier for the object.</span></span> <span data-ttu-id="7a8d2-149">Por exemplo, 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="7a8d2-149">For example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="7a8d2-150">O valor da propriedade **ID** é frequentemente, mas não exclusivamente, sob o formato de um GUID; O valor deve ser tratado como um identificador opaco e não confie no fato de ser um GUID.</span><span class="sxs-lookup"><span data-stu-id="7a8d2-150">The value of the **id** property is often but not exclusively in the form of a GUID; treat it as an opaque identifier and do not rely on it being a GUID.</span></span> <span data-ttu-id="7a8d2-151">Chave.</span><span class="sxs-lookup"><span data-stu-id="7a8d2-151">Key.</span></span> <span data-ttu-id="7a8d2-152">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="7a8d2-152">Not nullable.</span></span> <span data-ttu-id="7a8d2-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7a8d2-153">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a8d2-154">Relações</span><span class="sxs-lookup"><span data-stu-id="7a8d2-154">Relationships</span></span>

<span data-ttu-id="7a8d2-155">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7a8d2-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a8d2-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a8d2-156">JSON representation</span></span>

<span data-ttu-id="7a8d2-157">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7a8d2-157">Here is a JSON representation of the resource</span></span>

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


