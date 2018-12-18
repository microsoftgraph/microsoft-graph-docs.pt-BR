---
title: tipo de recurso contactFolder
description: Uma pasta que contém contatos.
author: angelgolfer-ms
ms.openlocfilehash: 93b4586272e3e762cf182bddc489326503411c84
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325638"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="520c6-103">tipo de recurso contactFolder</span><span class="sxs-lookup"><span data-stu-id="520c6-103">contactFolder resource type</span></span>

> <span data-ttu-id="520c6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="520c6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="520c6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="520c6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="520c6-106">Uma pasta que contém contatos.</span><span class="sxs-lookup"><span data-stu-id="520c6-106">A folder that contains contacts.</span></span>

<span data-ttu-id="520c6-107">Esse recurso suporta a utilização da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/contactfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="520c6-107">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="520c6-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="520c6-108">Methods</span></span>

| <span data-ttu-id="520c6-109">Método</span><span class="sxs-lookup"><span data-stu-id="520c6-109">Method</span></span>       | <span data-ttu-id="520c6-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="520c6-110">Return Type</span></span>  |<span data-ttu-id="520c6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="520c6-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="520c6-112">Obter contactFolder</span><span class="sxs-lookup"><span data-stu-id="520c6-112">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="520c6-113">contactFolder</span><span class="sxs-lookup"><span data-stu-id="520c6-113">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="520c6-114">Obtenha uma pasta de contatos usando a respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="520c6-114">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="520c6-115">Update</span><span class="sxs-lookup"><span data-stu-id="520c6-115">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="520c6-116">contactFolder</span><span class="sxs-lookup"><span data-stu-id="520c6-116">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="520c6-117">Atualize o objeto contactFolder.</span><span class="sxs-lookup"><span data-stu-id="520c6-117">Update contactFolder object.</span></span> |
|[<span data-ttu-id="520c6-118">Delete</span><span class="sxs-lookup"><span data-stu-id="520c6-118">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="520c6-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="520c6-119">None</span></span> |<span data-ttu-id="520c6-120">Exclua um objeto contactFolder.</span><span class="sxs-lookup"><span data-stu-id="520c6-120">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="520c6-121">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="520c6-121">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="520c6-122">coleção [contactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="520c6-122">[contactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="520c6-123">Obtenha uma coleção de pastas filho sob a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="520c6-123">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="520c6-124">Criar contactFolder filho</span><span class="sxs-lookup"><span data-stu-id="520c6-124">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="520c6-125">contactFolder</span><span class="sxs-lookup"><span data-stu-id="520c6-125">contactFolder</span></span>](contactfolder.md)| <span data-ttu-id="520c6-126">Crie uma nova contactFolder como um filho de uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="520c6-126">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="520c6-127">delta</span><span class="sxs-lookup"><span data-stu-id="520c6-127">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="520c6-128">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="520c6-128">[contact](contact.md) collection</span></span>| <span data-ttu-id="520c6-129">Obtenha um conjunto de pastas de contatos que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="520c6-129">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="520c6-130">Listar contatos na pasta</span><span class="sxs-lookup"><span data-stu-id="520c6-130">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="520c6-131">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="520c6-131">[contact](contact.md) collection</span></span>| <span data-ttu-id="520c6-132">Obtém uma coleção de contatos da pasta de contatos padrão do usuário conectado (`.../me/contacts`), ou da pasta contato especificada.</span><span class="sxs-lookup"><span data-stu-id="520c6-132">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="520c6-133">Criar contato na pasta</span><span class="sxs-lookup"><span data-stu-id="520c6-133">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="520c6-134">contato</span><span class="sxs-lookup"><span data-stu-id="520c6-134">contact</span></span>](contact.md)| <span data-ttu-id="520c6-135">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de `contacts` de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="520c6-135">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|<span data-ttu-id="520c6-136">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="520c6-136">**Extended properties**</span></span>| | |
|[<span data-ttu-id="520c6-137">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="520c6-137">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="520c6-138">contactFolder</span><span class="sxs-lookup"><span data-stu-id="520c6-138">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="520c6-139">Criar uma ou mais propriedades estendidas de valor único em uma contactFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="520c6-139">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="520c6-140">Obter contactFolder com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="520c6-140">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="520c6-141">contactFolder</span><span class="sxs-lookup"><span data-stu-id="520c6-141">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="520c6-142">Obtenha contactFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="520c6-142">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="520c6-143">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="520c6-143">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="520c6-144">contactFolder</span><span class="sxs-lookup"><span data-stu-id="520c6-144">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="520c6-145">Criar uma ou mais propriedades estendidas de vários valores em uma contactFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="520c6-145">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="520c6-146">Obter contactFolder com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="520c6-146">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="520c6-147">contactFolder</span><span class="sxs-lookup"><span data-stu-id="520c6-147">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="520c6-148">Obtenha uma contactFolder que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="520c6-148">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="520c6-149">Propriedades</span><span class="sxs-lookup"><span data-stu-id="520c6-149">Properties</span></span>
| <span data-ttu-id="520c6-150">Propriedade</span><span class="sxs-lookup"><span data-stu-id="520c6-150">Property</span></span>     | <span data-ttu-id="520c6-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="520c6-151">Type</span></span>   |<span data-ttu-id="520c6-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="520c6-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="520c6-153">displayName</span><span class="sxs-lookup"><span data-stu-id="520c6-153">displayName</span></span>|<span data-ttu-id="520c6-154">String</span><span class="sxs-lookup"><span data-stu-id="520c6-154">String</span></span>|<span data-ttu-id="520c6-155">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="520c6-155">The folder's display name.</span></span>|
|<span data-ttu-id="520c6-156">id</span><span class="sxs-lookup"><span data-stu-id="520c6-156">id</span></span>|<span data-ttu-id="520c6-157">String</span><span class="sxs-lookup"><span data-stu-id="520c6-157">String</span></span>|<span data-ttu-id="520c6-p102">Identificador exclusivo da pasta de contatos. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="520c6-p102">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="520c6-160">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="520c6-160">parentFolderId</span></span>|<span data-ttu-id="520c6-161">String</span><span class="sxs-lookup"><span data-stu-id="520c6-161">String</span></span>|<span data-ttu-id="520c6-162">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="520c6-162">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="520c6-163">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="520c6-163">wellKnownName</span></span>|<span data-ttu-id="520c6-164">string</span><span class="sxs-lookup"><span data-stu-id="520c6-164">string</span></span>|<span data-ttu-id="520c6-165">O nome da pasta se a pasta for uma pasta reconhecida.</span><span class="sxs-lookup"><span data-stu-id="520c6-165">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="520c6-166">No momento `contacts` é a única pasta Contatos reconhecidas.</span><span class="sxs-lookup"><span data-stu-id="520c6-166">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="520c6-167">Relações</span><span class="sxs-lookup"><span data-stu-id="520c6-167">Relationships</span></span>
| <span data-ttu-id="520c6-168">Relação</span><span class="sxs-lookup"><span data-stu-id="520c6-168">Relationship</span></span> | <span data-ttu-id="520c6-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="520c6-169">Type</span></span>   |<span data-ttu-id="520c6-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="520c6-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="520c6-171">childFolders</span><span class="sxs-lookup"><span data-stu-id="520c6-171">childFolders</span></span>|<span data-ttu-id="520c6-172">Coleção [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="520c6-172">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="520c6-p104">A coleção de pastas filho na pasta. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="520c6-p104">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="520c6-177">contatos</span><span class="sxs-lookup"><span data-stu-id="520c6-177">contacts</span></span>|<span data-ttu-id="520c6-178">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="520c6-178">[Contact](contact.md) collection</span></span>|<span data-ttu-id="520c6-p105">Os contatos na pasta. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="520c6-p105">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="520c6-183">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="520c6-183">multiValueExtendedProperties</span></span>|<span data-ttu-id="520c6-184">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="520c6-184">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="520c6-p106">A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="520c6-p106">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="520c6-188">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="520c6-188">singleValueExtendedProperties</span></span>|<span data-ttu-id="520c6-189">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="520c6-189">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="520c6-p107">A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="520c6-p107">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="520c6-193">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="520c6-193">JSON representation</span></span>

<span data-ttu-id="520c6-194">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="520c6-194">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactFolder"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "wellKnownName": "string"
}

```

## <a name="see-also"></a><span data-ttu-id="520c6-195">Confira também</span><span class="sxs-lookup"><span data-stu-id="520c6-195">See also</span></span>

- [<span data-ttu-id="520c6-196">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="520c6-196">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="520c6-197">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="520c6-197">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
