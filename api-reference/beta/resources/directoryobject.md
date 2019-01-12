---
title: Tipo de recurso directoryObject
description: Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7f02687a8fc3b5b50f4e1e956da4bdc632ea389e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952934"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="ec59a-104">Tipo de recurso directoryObject</span><span class="sxs-lookup"><span data-stu-id="ec59a-104">directoryObject resource type</span></span>

> <span data-ttu-id="ec59a-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ec59a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec59a-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ec59a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec59a-p103">Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.</span><span class="sxs-lookup"><span data-stu-id="ec59a-p103">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="ec59a-109">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="ec59a-109">This resource supports:</span></span>

- <span data-ttu-id="ec59a-110">Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryobject-delta.md).</span><span class="sxs-lookup"><span data-stu-id="ec59a-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="ec59a-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="ec59a-111">Methods</span></span>

| <span data-ttu-id="ec59a-112">Método</span><span class="sxs-lookup"><span data-stu-id="ec59a-112">Method</span></span>       | <span data-ttu-id="ec59a-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ec59a-113">Return Type</span></span>  |<span data-ttu-id="ec59a-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec59a-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ec59a-115">Get directoryObject</span><span class="sxs-lookup"><span data-stu-id="ec59a-115">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="ec59a-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="ec59a-116">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="ec59a-117">Leia as propriedades de um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="ec59a-117">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="ec59a-118">Delete</span><span class="sxs-lookup"><span data-stu-id="ec59a-118">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="ec59a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec59a-119">None</span></span> |<span data-ttu-id="ec59a-120">Exclua um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="ec59a-120">Delete a directory object.</span></span> |
|[<span data-ttu-id="ec59a-121">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="ec59a-121">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="ec59a-122">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec59a-122">String collection</span></span>|<span data-ttu-id="ec59a-p104">Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="ec59a-p104">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="ec59a-125">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="ec59a-125">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="ec59a-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec59a-126">String collection</span></span>|<span data-ttu-id="ec59a-p105">Retorne todos os grupos dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="ec59a-p105">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="ec59a-129">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="ec59a-129">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="ec59a-130">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec59a-130">String collection</span></span>| <span data-ttu-id="ec59a-p106">Retorne todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="ec59a-p106">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="ec59a-133">getByIds</span><span class="sxs-lookup"><span data-stu-id="ec59a-133">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="ec59a-134">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ec59a-134">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="ec59a-135">Obtenha um conjunto de objetos de diretório com base em um conjunto de ids fornecidas.</span><span class="sxs-lookup"><span data-stu-id="ec59a-135">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="ec59a-136">validateProperties</span><span class="sxs-lookup"><span data-stu-id="ec59a-136">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="ec59a-137">JSON</span><span class="sxs-lookup"><span data-stu-id="ec59a-137">JSON</span></span>| <span data-ttu-id="ec59a-138">Validar o nome de exibição de um grupo Office 365 ou apelido de email está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="ec59a-138">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="ec59a-139">delta</span><span class="sxs-lookup"><span data-stu-id="ec59a-139">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="ec59a-140">Coleção directoryObject</span><span class="sxs-lookup"><span data-stu-id="ec59a-140">directoryObject collection</span></span>| <span data-ttu-id="ec59a-141">Obtenha as alterações incrementais para objetos de diretório.</span><span class="sxs-lookup"><span data-stu-id="ec59a-141">Get incremental changes for directory objects.</span></span> <span data-ttu-id="ec59a-142">Oferece suporte à filtragem por tipo de derrived.</span><span class="sxs-lookup"><span data-stu-id="ec59a-142">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="ec59a-143">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec59a-143">Properties</span></span>

| <span data-ttu-id="ec59a-144">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec59a-144">Property</span></span>   | <span data-ttu-id="ec59a-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec59a-145">Type</span></span> |<span data-ttu-id="ec59a-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec59a-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec59a-147">id</span><span class="sxs-lookup"><span data-stu-id="ec59a-147">id</span></span>|<span data-ttu-id="ec59a-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec59a-148">String</span></span>|<span data-ttu-id="ec59a-149">Um Guid que é o identificador exclusivo para o objeto; Por exemplo, 12345678-9abc-def0-1234-56789abcde12.</span><span class="sxs-lookup"><span data-stu-id="ec59a-149">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde12.</span></span> <span data-ttu-id="ec59a-150">Chave.</span><span class="sxs-lookup"><span data-stu-id="ec59a-150">Key.</span></span> <span data-ttu-id="ec59a-151">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ec59a-151">Not nullable.</span></span> <span data-ttu-id="ec59a-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ec59a-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec59a-153">Relações</span><span class="sxs-lookup"><span data-stu-id="ec59a-153">Relationships</span></span>

<span data-ttu-id="ec59a-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec59a-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec59a-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec59a-155">JSON representation</span></span>

<span data-ttu-id="ec59a-156">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ec59a-156">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject"
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
