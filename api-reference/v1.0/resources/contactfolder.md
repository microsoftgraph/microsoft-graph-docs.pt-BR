---
title: tipo de recurso contactFolder
description: Uma pasta que contém contatos.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 03bc6f2a2dfda74af701a14a5b59cbc8865420b8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449476"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="0186c-103">tipo de recurso contactFolder</span><span class="sxs-lookup"><span data-stu-id="0186c-103">contactFolder resource type</span></span>

<span data-ttu-id="0186c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0186c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0186c-105">Uma pasta que contém contatos.</span><span class="sxs-lookup"><span data-stu-id="0186c-105">A folder that contains contacts.</span></span>

<span data-ttu-id="0186c-106">Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/contactfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="0186c-106">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="0186c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="0186c-107">Methods</span></span>

| <span data-ttu-id="0186c-108">Método</span><span class="sxs-lookup"><span data-stu-id="0186c-108">Method</span></span>       | <span data-ttu-id="0186c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0186c-109">Return Type</span></span>  |<span data-ttu-id="0186c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0186c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0186c-111">Obter contactFolder</span><span class="sxs-lookup"><span data-stu-id="0186c-111">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="0186c-112">pastadeContatos</span><span class="sxs-lookup"><span data-stu-id="0186c-112">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="0186c-113">Obtenha uma pasta de contatos usando a respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="0186c-113">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="0186c-114">Update</span><span class="sxs-lookup"><span data-stu-id="0186c-114">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="0186c-115">pastadeContatos</span><span class="sxs-lookup"><span data-stu-id="0186c-115">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="0186c-116">Atualize o objeto contactFolder.</span><span class="sxs-lookup"><span data-stu-id="0186c-116">Update contactFolder object.</span></span> |
|[<span data-ttu-id="0186c-117">Excluir</span><span class="sxs-lookup"><span data-stu-id="0186c-117">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="0186c-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0186c-118">None</span></span> |<span data-ttu-id="0186c-119">Exclua um objeto contactFolder.</span><span class="sxs-lookup"><span data-stu-id="0186c-119">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="0186c-120">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="0186c-120">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="0186c-121">Coleção [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="0186c-121">[ContactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="0186c-122">Obtenha uma coleção de pastas filho sob a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="0186c-122">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="0186c-123">Criar contactFolder filho</span><span class="sxs-lookup"><span data-stu-id="0186c-123">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="0186c-124">ContactFolder</span><span class="sxs-lookup"><span data-stu-id="0186c-124">ContactFolder</span></span>](contactfolder.md)| <span data-ttu-id="0186c-125">Crie uma nova contactFolder como um filho de uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="0186c-125">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="0186c-126">delta</span><span class="sxs-lookup"><span data-stu-id="0186c-126">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="0186c-127">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="0186c-127">[contact](contact.md) collection</span></span>| <span data-ttu-id="0186c-128">Obtenha um conjunto de pastas de contatos que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="0186c-128">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="0186c-129">Listar contatos na pasta</span><span class="sxs-lookup"><span data-stu-id="0186c-129">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="0186c-130">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="0186c-130">[Contact](contact.md) collection</span></span>| <span data-ttu-id="0186c-131">Obtém uma coleção de contatos da pasta de contatos padrão do usuário conectado (`.../me/contacts`), ou da pasta contato especificada.</span><span class="sxs-lookup"><span data-stu-id="0186c-131">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="0186c-132">Criar contato na pasta</span><span class="sxs-lookup"><span data-stu-id="0186c-132">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="0186c-133">Contact</span><span class="sxs-lookup"><span data-stu-id="0186c-133">Contact</span></span>](contact.md)| <span data-ttu-id="0186c-134">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de `contacts` de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="0186c-134">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="0186c-135">Criar propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="0186c-135">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="0186c-136">pastadeContatos</span><span class="sxs-lookup"><span data-stu-id="0186c-136">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="0186c-137">Criar uma ou mais propriedades estendidas de valor único em uma contactFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="0186c-137">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="0186c-138">Obter contactFolder com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="0186c-138">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="0186c-139">pastadeContatos</span><span class="sxs-lookup"><span data-stu-id="0186c-139">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="0186c-140">Obtenha contactFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="0186c-140">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="0186c-141">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="0186c-141">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="0186c-142">pastadeContatos</span><span class="sxs-lookup"><span data-stu-id="0186c-142">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="0186c-143">Criar uma ou mais propriedades estendidas de vários valores em uma contactFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="0186c-143">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="0186c-144">Obter contactFolder com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="0186c-144">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="0186c-145">pastadeContatos</span><span class="sxs-lookup"><span data-stu-id="0186c-145">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="0186c-146">Obtenha uma contactFolder que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="0186c-146">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="0186c-147">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0186c-147">Properties</span></span>
| <span data-ttu-id="0186c-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0186c-148">Property</span></span>     | <span data-ttu-id="0186c-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="0186c-149">Type</span></span>   |<span data-ttu-id="0186c-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="0186c-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0186c-151">displayName</span><span class="sxs-lookup"><span data-stu-id="0186c-151">displayName</span></span>|<span data-ttu-id="0186c-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0186c-152">String</span></span>|<span data-ttu-id="0186c-153">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="0186c-153">The folder's display name.</span></span>|
|<span data-ttu-id="0186c-154">id</span><span class="sxs-lookup"><span data-stu-id="0186c-154">id</span></span>|<span data-ttu-id="0186c-155">String</span><span class="sxs-lookup"><span data-stu-id="0186c-155">String</span></span>|<span data-ttu-id="0186c-p101">Identificador exclusivo da pasta de contatos. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0186c-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="0186c-158">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="0186c-158">parentFolderId</span></span>|<span data-ttu-id="0186c-159">String</span><span class="sxs-lookup"><span data-stu-id="0186c-159">String</span></span>|<span data-ttu-id="0186c-160">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="0186c-160">The ID of the folder's parent folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0186c-161">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="0186c-161">Relationships</span></span>
| <span data-ttu-id="0186c-162">Relação</span><span class="sxs-lookup"><span data-stu-id="0186c-162">Relationship</span></span> | <span data-ttu-id="0186c-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="0186c-163">Type</span></span>   |<span data-ttu-id="0186c-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="0186c-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0186c-165">childFolders</span><span class="sxs-lookup"><span data-stu-id="0186c-165">childFolders</span></span>|<span data-ttu-id="0186c-166">Coleção [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="0186c-166">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="0186c-p102">A coleção de pastas filho na pasta. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0186c-p102">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="0186c-171">contatos</span><span class="sxs-lookup"><span data-stu-id="0186c-171">contacts</span></span>|<span data-ttu-id="0186c-172">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="0186c-172">[Contact](contact.md) collection</span></span>|<span data-ttu-id="0186c-p103">Os contatos na pasta. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0186c-p103">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="0186c-177">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="0186c-177">multiValueExtendedProperties</span></span>|<span data-ttu-id="0186c-178">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="0186c-178">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="0186c-p104">A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0186c-p104">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="0186c-182">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="0186c-182">singleValueExtendedProperties</span></span>|<span data-ttu-id="0186c-183">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="0186c-183">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="0186c-p105">A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0186c-p105">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0186c-187">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0186c-187">JSON representation</span></span>

<span data-ttu-id="0186c-188">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0186c-188">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="0186c-189">Confira também</span><span class="sxs-lookup"><span data-stu-id="0186c-189">See also</span></span>

- [<span data-ttu-id="0186c-190">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0186c-190">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="0186c-191">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="0186c-191">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
