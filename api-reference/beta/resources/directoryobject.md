---
title: Tipo de recurso directoryObject
description: Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5ba2454a5eda90ec50dbd6a0c152383bb42a437d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573953"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="3bbb1-104">Tipo de recurso directoryObject</span><span class="sxs-lookup"><span data-stu-id="3bbb1-104">directoryObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bbb1-p102">Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.</span><span class="sxs-lookup"><span data-stu-id="3bbb1-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="3bbb1-107">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="3bbb1-107">This resource supports:</span></span>

- <span data-ttu-id="3bbb1-108">Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryobject-delta.md).</span><span class="sxs-lookup"><span data-stu-id="3bbb1-108">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="3bbb1-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="3bbb1-109">Methods</span></span>

| <span data-ttu-id="3bbb1-110">Método</span><span class="sxs-lookup"><span data-stu-id="3bbb1-110">Method</span></span>       | <span data-ttu-id="3bbb1-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3bbb1-111">Return Type</span></span>  |<span data-ttu-id="3bbb1-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bbb1-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3bbb1-113">Get directoryObject</span><span class="sxs-lookup"><span data-stu-id="3bbb1-113">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="3bbb1-114">directoryObject</span><span class="sxs-lookup"><span data-stu-id="3bbb1-114">directoryObject</span></span>](../resources/directoryobject.md) |<span data-ttu-id="3bbb1-115">Leia as propriedades de um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="3bbb1-115">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="3bbb1-116">Delete</span><span class="sxs-lookup"><span data-stu-id="3bbb1-116">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="3bbb1-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3bbb1-117">None</span></span> |<span data-ttu-id="3bbb1-118">Exclua um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="3bbb1-118">Delete a directory object.</span></span> |
|[<span data-ttu-id="3bbb1-119">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="3bbb1-119">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="3bbb1-120">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bbb1-120">String collection</span></span>|<span data-ttu-id="3bbb1-p103">Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="3bbb1-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="3bbb1-123">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="3bbb1-123">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="3bbb1-124">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bbb1-124">String collection</span></span>|<span data-ttu-id="3bbb1-p104">Retorne todos os grupos dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="3bbb1-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="3bbb1-127">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="3bbb1-127">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="3bbb1-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bbb1-128">String collection</span></span>| <span data-ttu-id="3bbb1-p105">Retorne todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="3bbb1-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="3bbb1-131">getByIds</span><span class="sxs-lookup"><span data-stu-id="3bbb1-131">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="3bbb1-132">Coleção [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="3bbb1-132">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="3bbb1-133">Obtenha um conjunto de objetos de diretório com base em um conjunto de ids fornecidas.</span><span class="sxs-lookup"><span data-stu-id="3bbb1-133">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="3bbb1-134">validateProperties</span><span class="sxs-lookup"><span data-stu-id="3bbb1-134">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="3bbb1-135">JSON</span><span class="sxs-lookup"><span data-stu-id="3bbb1-135">JSON</span></span>| <span data-ttu-id="3bbb1-136">Validar um nome de exibição ou um apelido de email do grupo do Office 365 em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="3bbb1-136">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="3bbb1-137">delta</span><span class="sxs-lookup"><span data-stu-id="3bbb1-137">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="3bbb1-138">Coleção directoryObject</span><span class="sxs-lookup"><span data-stu-id="3bbb1-138">directoryObject collection</span></span>| <span data-ttu-id="3bbb1-139">Obtenha alterações incrementais para objetos de diretório.</span><span class="sxs-lookup"><span data-stu-id="3bbb1-139">Get incremental changes for directory objects.</span></span> <span data-ttu-id="3bbb1-140">Oferece suporte à filtragem por tipo derivado.</span><span class="sxs-lookup"><span data-stu-id="3bbb1-140">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="3bbb1-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3bbb1-141">Properties</span></span>

| <span data-ttu-id="3bbb1-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3bbb1-142">Property</span></span>   | <span data-ttu-id="3bbb1-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bbb1-143">Type</span></span> |<span data-ttu-id="3bbb1-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bbb1-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3bbb1-145">id</span><span class="sxs-lookup"><span data-stu-id="3bbb1-145">id</span></span>|<span data-ttu-id="3bbb1-146">String</span><span class="sxs-lookup"><span data-stu-id="3bbb1-146">String</span></span>|<span data-ttu-id="3bbb1-147">Um Guid que é o identificador exclusivo do objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde12.</span><span class="sxs-lookup"><span data-stu-id="3bbb1-147">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span> <span data-ttu-id="3bbb1-148">Chave.</span><span class="sxs-lookup"><span data-stu-id="3bbb1-148">Key.</span></span> <span data-ttu-id="3bbb1-149">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="3bbb1-149">Not nullable.</span></span> <span data-ttu-id="3bbb1-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3bbb1-150">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3bbb1-151">Relações</span><span class="sxs-lookup"><span data-stu-id="3bbb1-151">Relationships</span></span>

<span data-ttu-id="3bbb1-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3bbb1-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3bbb1-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3bbb1-153">JSON representation</span></span>

<span data-ttu-id="3bbb1-154">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3bbb1-154">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
