---
title: Tipo de recurso directoryObject
description: Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.
localization_priority: Priority
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 83750686b4075f7577e88e1e6107dd2f2a5f4d2f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439902"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="a62fd-104">Tipo de recurso directoryObject</span><span class="sxs-lookup"><span data-stu-id="a62fd-104">directoryObject resource type</span></span>

<span data-ttu-id="a62fd-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a62fd-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a62fd-p102">Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.</span><span class="sxs-lookup"><span data-stu-id="a62fd-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="a62fd-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="a62fd-108">Methods</span></span>

| <span data-ttu-id="a62fd-109">Método</span><span class="sxs-lookup"><span data-stu-id="a62fd-109">Method</span></span>       | <span data-ttu-id="a62fd-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a62fd-110">Return Type</span></span>  |<span data-ttu-id="a62fd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a62fd-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a62fd-112">Get directoryObject</span><span class="sxs-lookup"><span data-stu-id="a62fd-112">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="a62fd-113">directoryObject</span><span class="sxs-lookup"><span data-stu-id="a62fd-113">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="a62fd-114">Leia as propriedades de um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="a62fd-114">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="a62fd-115">Delete directoryObject</span><span class="sxs-lookup"><span data-stu-id="a62fd-115">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="a62fd-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a62fd-116">None</span></span> |<span data-ttu-id="a62fd-117">Exclua um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="a62fd-117">Delete a directory object.</span></span> |
|[<span data-ttu-id="a62fd-118">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="a62fd-118">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="a62fd-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a62fd-119">String collection</span></span>|<span data-ttu-id="a62fd-p103">Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="a62fd-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="a62fd-122">Obtenha as propriedades de extensão disponíveis</span><span class="sxs-lookup"><span data-stu-id="a62fd-122">Get available extension properties</span></span>](../api/directoryobject-getavailableextensionproperties.md)|<span data-ttu-id="a62fd-123">Coleção [extensionProperty](../resources/extensionproperty.md)</span><span class="sxs-lookup"><span data-stu-id="a62fd-123">[extensionProperty](../resources/extensionproperty.md) collection</span></span>|<span data-ttu-id="a62fd-124">Obtenha todas as listas ou uma lista filtrada das propriedades de extensão do diretório que foram registradas em um diretório.</span><span class="sxs-lookup"><span data-stu-id="a62fd-124">Get all or a filtered list of the directory extension properties that have been registered in a directory.</span></span>|
|[<span data-ttu-id="a62fd-125">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="a62fd-125">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="a62fd-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a62fd-126">String collection</span></span>|<span data-ttu-id="a62fd-p104">Retorne todos os grupos dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="a62fd-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="a62fd-129">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="a62fd-129">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="a62fd-130">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a62fd-130">String collection</span></span>| <span data-ttu-id="a62fd-p105">Retorne todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="a62fd-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="a62fd-133">getByIds</span><span class="sxs-lookup"><span data-stu-id="a62fd-133">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="a62fd-134">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a62fd-134">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="a62fd-135">Obtenha um conjunto de objetos de diretório com base em um conjunto de ids fornecidas.</span><span class="sxs-lookup"><span data-stu-id="a62fd-135">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="a62fd-136">validateProperties</span><span class="sxs-lookup"><span data-stu-id="a62fd-136">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="a62fd-137">Json</span><span class="sxs-lookup"><span data-stu-id="a62fd-137">Json</span></span>| <span data-ttu-id="a62fd-138">Valide se o nome de exibição ou apelido de email de um grupo da Microsoft 365 está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="a62fd-138">Validate that a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span> |

## <a name="properties"></a><span data-ttu-id="a62fd-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a62fd-139">Properties</span></span>

| <span data-ttu-id="a62fd-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a62fd-140">Property</span></span>   | <span data-ttu-id="a62fd-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="a62fd-141">Type</span></span> |<span data-ttu-id="a62fd-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="a62fd-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a62fd-143">id</span><span class="sxs-lookup"><span data-stu-id="a62fd-143">id</span></span>|<span data-ttu-id="a62fd-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a62fd-144">String</span></span>|<span data-ttu-id="a62fd-145">O identificador exclusivo para o objeto.</span><span class="sxs-lookup"><span data-stu-id="a62fd-145">The unique identifier for the object.</span></span> <span data-ttu-id="a62fd-146">Por exemplo, 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="a62fd-146">For example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="a62fd-147">O valor da propriedade **ID** é frequentemente, mas não exclusivamente, sob o formato de um GUID; O valor deve ser tratado como um identificador opaco e não confie no fato de ser um GUID.</span><span class="sxs-lookup"><span data-stu-id="a62fd-147">The value of the **id** property is often but not exclusively in the form of a GUID; treat it as an opaque identifier and do not rely on it being a GUID.</span></span> <span data-ttu-id="a62fd-148">Chave.</span><span class="sxs-lookup"><span data-stu-id="a62fd-148">Key.</span></span> <span data-ttu-id="a62fd-149">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="a62fd-149">Not nullable.</span></span> <span data-ttu-id="a62fd-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a62fd-150">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a62fd-151">Relações</span><span class="sxs-lookup"><span data-stu-id="a62fd-151">Relationships</span></span>

<span data-ttu-id="a62fd-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a62fd-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a62fd-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a62fd-153">JSON representation</span></span>

<span data-ttu-id="a62fd-154">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a62fd-154">Here is a JSON representation of the resource</span></span>

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

