---
title: tipo de recurso contactFolder
description: Uma pasta que contém contatos.
author: angelgolfer-ms
ms.openlocfilehash: 4630547bdee34d6e012c3747dba248eef9f908b9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320269"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="45416-103">tipo de recurso contactFolder</span><span class="sxs-lookup"><span data-stu-id="45416-103">contactFolder resource type</span></span>

<span data-ttu-id="45416-104">Uma pasta que contém contatos.</span><span class="sxs-lookup"><span data-stu-id="45416-104">A folder that contains contacts.</span></span>

<span data-ttu-id="45416-105">Esse recurso suporta a utilização da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/contactfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="45416-105">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="45416-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="45416-106">Methods</span></span>

| <span data-ttu-id="45416-107">Método</span><span class="sxs-lookup"><span data-stu-id="45416-107">Method</span></span>       | <span data-ttu-id="45416-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="45416-108">Return Type</span></span>  |<span data-ttu-id="45416-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="45416-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="45416-110">Obter contactFolder</span><span class="sxs-lookup"><span data-stu-id="45416-110">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="45416-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="45416-111">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="45416-112">Obtenha uma pasta de contatos usando a respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="45416-112">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="45416-113">Update</span><span class="sxs-lookup"><span data-stu-id="45416-113">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="45416-114">contactFolder</span><span class="sxs-lookup"><span data-stu-id="45416-114">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="45416-115">Atualize o objeto contactFolder.</span><span class="sxs-lookup"><span data-stu-id="45416-115">Update contactFolder object.</span></span> |
|[<span data-ttu-id="45416-116">Delete</span><span class="sxs-lookup"><span data-stu-id="45416-116">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="45416-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="45416-117">None</span></span> |<span data-ttu-id="45416-118">Exclua um objeto contactFolder.</span><span class="sxs-lookup"><span data-stu-id="45416-118">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="45416-119">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="45416-119">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="45416-120">Coleção [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="45416-120">[ContactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="45416-121">Obtenha uma coleção de pastas filho sob a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="45416-121">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="45416-122">Criar contactFolder filho</span><span class="sxs-lookup"><span data-stu-id="45416-122">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="45416-123">ContactFolder</span><span class="sxs-lookup"><span data-stu-id="45416-123">ContactFolder</span></span>](contactfolder.md)| <span data-ttu-id="45416-124">Crie uma nova contactFolder como um filho de uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="45416-124">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="45416-125">delta</span><span class="sxs-lookup"><span data-stu-id="45416-125">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="45416-126">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="45416-126">[contact](contact.md) collection</span></span>| <span data-ttu-id="45416-127">Obtenha um conjunto de pastas de contatos que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="45416-127">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="45416-128">Listar contatos na pasta</span><span class="sxs-lookup"><span data-stu-id="45416-128">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="45416-129">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="45416-129">[Contact](contact.md) collection</span></span>| <span data-ttu-id="45416-130">Obtém uma coleção de contatos da pasta de contatos padrão do usuário conectado (`.../me/contacts`), ou da pasta contato especificada.</span><span class="sxs-lookup"><span data-stu-id="45416-130">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="45416-131">Criar contato na pasta</span><span class="sxs-lookup"><span data-stu-id="45416-131">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="45416-132">Contact</span><span class="sxs-lookup"><span data-stu-id="45416-132">Contact</span></span>](contact.md)| <span data-ttu-id="45416-133">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de `contacts` de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="45416-133">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="45416-134">Criar propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="45416-134">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="45416-135">contactFolder</span><span class="sxs-lookup"><span data-stu-id="45416-135">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="45416-136">Criar uma ou mais propriedades estendidas de valor único em uma contactFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="45416-136">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="45416-137">Obter contactFolder com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="45416-137">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="45416-138">contactFolder</span><span class="sxs-lookup"><span data-stu-id="45416-138">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="45416-139">Obtenha contactFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="45416-139">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="45416-140">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="45416-140">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="45416-141">contactFolder</span><span class="sxs-lookup"><span data-stu-id="45416-141">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="45416-142">Criar uma ou mais propriedades estendidas de vários valores em uma contactFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="45416-142">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="45416-143">Obter contactFolder com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="45416-143">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="45416-144">contactFolder</span><span class="sxs-lookup"><span data-stu-id="45416-144">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="45416-145">Obtenha uma contactFolder que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="45416-145">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="45416-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45416-146">Properties</span></span>
| <span data-ttu-id="45416-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45416-147">Property</span></span>     | <span data-ttu-id="45416-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="45416-148">Type</span></span>   |<span data-ttu-id="45416-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="45416-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45416-150">displayName</span><span class="sxs-lookup"><span data-stu-id="45416-150">displayName</span></span>|<span data-ttu-id="45416-151">String</span><span class="sxs-lookup"><span data-stu-id="45416-151">String</span></span>|<span data-ttu-id="45416-152">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="45416-152">The folder's display name.</span></span>|
|<span data-ttu-id="45416-153">id</span><span class="sxs-lookup"><span data-stu-id="45416-153">id</span></span>|<span data-ttu-id="45416-154">String</span><span class="sxs-lookup"><span data-stu-id="45416-154">String</span></span>|<span data-ttu-id="45416-p101">Identificador exclusivo da pasta de contatos. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45416-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="45416-157">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="45416-157">parentFolderId</span></span>|<span data-ttu-id="45416-158">String</span><span class="sxs-lookup"><span data-stu-id="45416-158">String</span></span>|<span data-ttu-id="45416-159">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="45416-159">The ID of the folder's parent folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45416-160">Relações</span><span class="sxs-lookup"><span data-stu-id="45416-160">Relationships</span></span>
| <span data-ttu-id="45416-161">Relação</span><span class="sxs-lookup"><span data-stu-id="45416-161">Relationship</span></span> | <span data-ttu-id="45416-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="45416-162">Type</span></span>   |<span data-ttu-id="45416-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="45416-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45416-164">childFolders</span><span class="sxs-lookup"><span data-stu-id="45416-164">childFolders</span></span>|<span data-ttu-id="45416-165">Coleção [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="45416-165">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="45416-p102">A coleção de pastas filho na pasta. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="45416-p102">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="45416-170">contatos</span><span class="sxs-lookup"><span data-stu-id="45416-170">contacts</span></span>|<span data-ttu-id="45416-171">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="45416-171">[Contact](contact.md) collection</span></span>|<span data-ttu-id="45416-p103">Os contatos na pasta. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="45416-p103">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="45416-176">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="45416-176">multiValueExtendedProperties</span></span>|<span data-ttu-id="45416-177">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="45416-177">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="45416-p104">A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="45416-p104">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="45416-181">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="45416-181">singleValueExtendedProperties</span></span>|<span data-ttu-id="45416-182">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="45416-182">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="45416-p105">A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="45416-p105">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45416-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45416-186">JSON representation</span></span>

<span data-ttu-id="45416-187">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="45416-187">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.contactFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "navigability": "single",
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string"
}

```

## <a name="see-also"></a><span data-ttu-id="45416-188">Confira também</span><span class="sxs-lookup"><span data-stu-id="45416-188">See also</span></span>

- [<span data-ttu-id="45416-189">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="45416-189">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="45416-190">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="45416-190">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
