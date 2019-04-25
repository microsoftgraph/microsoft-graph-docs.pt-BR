---
title: tipo de recurso contactFolder
description: Uma pasta que contém contatos.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6cf4d6ed75427dce527ced6cb64d0cdcb9afed99
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548163"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="ab250-103">tipo de recurso contactFolder</span><span class="sxs-lookup"><span data-stu-id="ab250-103">contactFolder resource type</span></span>

<span data-ttu-id="ab250-104">Uma pasta que contém contatos.</span><span class="sxs-lookup"><span data-stu-id="ab250-104">A folder that contains contacts.</span></span>

<span data-ttu-id="ab250-105">Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/contactfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="ab250-105">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="ab250-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ab250-106">Methods</span></span>

| <span data-ttu-id="ab250-107">Método</span><span class="sxs-lookup"><span data-stu-id="ab250-107">Method</span></span>       | <span data-ttu-id="ab250-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ab250-108">Return Type</span></span>  |<span data-ttu-id="ab250-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab250-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ab250-110">Obter contactFolder</span><span class="sxs-lookup"><span data-stu-id="ab250-110">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="ab250-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ab250-111">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="ab250-112">Obtenha uma pasta de contatos usando a respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="ab250-112">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="ab250-113">Update</span><span class="sxs-lookup"><span data-stu-id="ab250-113">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="ab250-114">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ab250-114">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="ab250-115">Atualize o objeto contactFolder.</span><span class="sxs-lookup"><span data-stu-id="ab250-115">Update contactFolder object.</span></span> |
|[<span data-ttu-id="ab250-116">Excluir</span><span class="sxs-lookup"><span data-stu-id="ab250-116">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="ab250-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ab250-117">None</span></span> |<span data-ttu-id="ab250-118">Exclua um objeto contactFolder.</span><span class="sxs-lookup"><span data-stu-id="ab250-118">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="ab250-119">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="ab250-119">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="ab250-120">Coleção [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="ab250-120">[ContactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="ab250-121">Obtenha uma coleção de pastas filho sob a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="ab250-121">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="ab250-122">Criar contactFolder filho</span><span class="sxs-lookup"><span data-stu-id="ab250-122">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="ab250-123">ContactFolder</span><span class="sxs-lookup"><span data-stu-id="ab250-123">ContactFolder</span></span>](contactfolder.md)| <span data-ttu-id="ab250-124">Crie uma nova contactFolder como um filho de uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="ab250-124">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="ab250-125">delta</span><span class="sxs-lookup"><span data-stu-id="ab250-125">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="ab250-126">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="ab250-126">[contact](contact.md) collection</span></span>| <span data-ttu-id="ab250-127">Obtenha um conjunto de pastas de contatos que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ab250-127">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="ab250-128">Listar contatos na pasta</span><span class="sxs-lookup"><span data-stu-id="ab250-128">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="ab250-129">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="ab250-129">[Contact](contact.md) collection</span></span>| <span data-ttu-id="ab250-130">Obtém uma coleção de contatos da pasta de contatos padrão do usuário conectado (`.../me/contacts`), ou da pasta contato especificada.</span><span class="sxs-lookup"><span data-stu-id="ab250-130">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="ab250-131">Criar contato na pasta</span><span class="sxs-lookup"><span data-stu-id="ab250-131">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="ab250-132">Contact</span><span class="sxs-lookup"><span data-stu-id="ab250-132">Contact</span></span>](contact.md)| <span data-ttu-id="ab250-133">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de `contacts` de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="ab250-133">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="ab250-134">Criar propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="ab250-134">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="ab250-135">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ab250-135">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="ab250-136">Criar uma ou mais propriedades estendidas de valor único em uma contactFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="ab250-136">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="ab250-137">Obter contactFolder com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="ab250-137">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="ab250-138">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ab250-138">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="ab250-139">Obtenha contactFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ab250-139">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="ab250-140">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="ab250-140">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="ab250-141">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ab250-141">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="ab250-142">Criar uma ou mais propriedades estendidas de vários valores em uma contactFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="ab250-142">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="ab250-143">Obter contactFolder com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="ab250-143">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="ab250-144">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ab250-144">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="ab250-145">Obtenha uma contactFolder que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="ab250-145">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="ab250-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab250-146">Properties</span></span>
| <span data-ttu-id="ab250-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab250-147">Property</span></span>     | <span data-ttu-id="ab250-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab250-148">Type</span></span>   |<span data-ttu-id="ab250-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab250-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab250-150">displayName</span><span class="sxs-lookup"><span data-stu-id="ab250-150">displayName</span></span>|<span data-ttu-id="ab250-151">String</span><span class="sxs-lookup"><span data-stu-id="ab250-151">String</span></span>|<span data-ttu-id="ab250-152">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="ab250-152">The folder's display name.</span></span>|
|<span data-ttu-id="ab250-153">id</span><span class="sxs-lookup"><span data-stu-id="ab250-153">id</span></span>|<span data-ttu-id="ab250-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab250-154">String</span></span>|<span data-ttu-id="ab250-p101">Identificador exclusivo da pasta de contatos. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab250-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="ab250-157">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="ab250-157">parentFolderId</span></span>|<span data-ttu-id="ab250-158">String</span><span class="sxs-lookup"><span data-stu-id="ab250-158">String</span></span>|<span data-ttu-id="ab250-159">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="ab250-159">The ID of the folder's parent folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab250-160">Relações</span><span class="sxs-lookup"><span data-stu-id="ab250-160">Relationships</span></span>
| <span data-ttu-id="ab250-161">Relação</span><span class="sxs-lookup"><span data-stu-id="ab250-161">Relationship</span></span> | <span data-ttu-id="ab250-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab250-162">Type</span></span>   |<span data-ttu-id="ab250-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab250-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab250-164">childFolders</span><span class="sxs-lookup"><span data-stu-id="ab250-164">childFolders</span></span>|<span data-ttu-id="ab250-165">Coleção [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="ab250-165">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="ab250-p102">A coleção de pastas filho na pasta. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ab250-p102">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="ab250-170">contatos</span><span class="sxs-lookup"><span data-stu-id="ab250-170">contacts</span></span>|<span data-ttu-id="ab250-171">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="ab250-171">[Contact](contact.md) collection</span></span>|<span data-ttu-id="ab250-p103">Os contatos na pasta. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ab250-p103">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="ab250-176">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="ab250-176">multiValueExtendedProperties</span></span>|<span data-ttu-id="ab250-177">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="ab250-177">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="ab250-p104">A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ab250-p104">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="ab250-181">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="ab250-181">singleValueExtendedProperties</span></span>|<span data-ttu-id="ab250-182">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="ab250-182">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="ab250-p105">A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ab250-p105">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab250-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab250-186">JSON representation</span></span>

<span data-ttu-id="ab250-187">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ab250-187">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="ab250-188">Confira também</span><span class="sxs-lookup"><span data-stu-id="ab250-188">See also</span></span>

- [<span data-ttu-id="ab250-189">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ab250-189">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="ab250-190">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="ab250-190">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
