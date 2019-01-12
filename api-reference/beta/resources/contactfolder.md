---
title: tipo de recurso contactFolder
description: Uma pasta que contém contatos.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 450c683d91eeb789c8c54b2bbfd38db695fbbba2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967543"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="ce4bf-103">tipo de recurso contactFolder</span><span class="sxs-lookup"><span data-stu-id="ce4bf-103">contactFolder resource type</span></span>

> <span data-ttu-id="ce4bf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce4bf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ce4bf-106">Uma pasta que contém contatos.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-106">A folder that contains contacts.</span></span>

<span data-ttu-id="ce4bf-107">Esse recurso suporta a utilização da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/contactfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="ce4bf-107">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="ce4bf-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="ce4bf-108">Methods</span></span>

| <span data-ttu-id="ce4bf-109">Método</span><span class="sxs-lookup"><span data-stu-id="ce4bf-109">Method</span></span>       | <span data-ttu-id="ce4bf-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ce4bf-110">Return Type</span></span>  |<span data-ttu-id="ce4bf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce4bf-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ce4bf-112">Obter contactFolder</span><span class="sxs-lookup"><span data-stu-id="ce4bf-112">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="ce4bf-113">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ce4bf-113">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="ce4bf-114">Obtenha uma pasta de contatos usando a respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-114">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="ce4bf-115">Update</span><span class="sxs-lookup"><span data-stu-id="ce4bf-115">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="ce4bf-116">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ce4bf-116">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="ce4bf-117">Atualize o objeto contactFolder.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-117">Update contactFolder object.</span></span> |
|[<span data-ttu-id="ce4bf-118">Delete</span><span class="sxs-lookup"><span data-stu-id="ce4bf-118">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="ce4bf-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ce4bf-119">None</span></span> |<span data-ttu-id="ce4bf-120">Exclua um objeto contactFolder.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-120">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="ce4bf-121">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="ce4bf-121">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="ce4bf-122">coleção [contactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="ce4bf-122">[contactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="ce4bf-123">Obtenha uma coleção de pastas filho sob a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-123">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="ce4bf-124">Criar contactFolder filho</span><span class="sxs-lookup"><span data-stu-id="ce4bf-124">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="ce4bf-125">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ce4bf-125">contactFolder</span></span>](contactfolder.md)| <span data-ttu-id="ce4bf-126">Crie uma nova contactFolder como um filho de uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-126">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="ce4bf-127">delta</span><span class="sxs-lookup"><span data-stu-id="ce4bf-127">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="ce4bf-128">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="ce4bf-128">[contact](contact.md) collection</span></span>| <span data-ttu-id="ce4bf-129">Obtenha um conjunto de pastas de contatos que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-129">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="ce4bf-130">Listar contatos na pasta</span><span class="sxs-lookup"><span data-stu-id="ce4bf-130">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="ce4bf-131">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="ce4bf-131">[contact](contact.md) collection</span></span>| <span data-ttu-id="ce4bf-132">Obtém uma coleção de contatos da pasta de contatos padrão do usuário conectado (`.../me/contacts`), ou da pasta contato especificada.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-132">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="ce4bf-133">Criar contato na pasta</span><span class="sxs-lookup"><span data-stu-id="ce4bf-133">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="ce4bf-134">contato</span><span class="sxs-lookup"><span data-stu-id="ce4bf-134">contact</span></span>](contact.md)| <span data-ttu-id="ce4bf-135">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de `contacts` de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-135">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|<span data-ttu-id="ce4bf-136">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="ce4bf-136">**Extended properties**</span></span>| | |
|[<span data-ttu-id="ce4bf-137">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="ce4bf-137">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="ce4bf-138">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ce4bf-138">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="ce4bf-139">Criar uma ou mais propriedades estendidas de valor único em uma contactFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-139">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="ce4bf-140">Obter contactFolder com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="ce4bf-140">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="ce4bf-141">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ce4bf-141">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="ce4bf-142">Obtenha contactFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-142">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="ce4bf-143">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="ce4bf-143">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="ce4bf-144">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ce4bf-144">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="ce4bf-145">Criar uma ou mais propriedades estendidas de vários valores em uma contactFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-145">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="ce4bf-146">Obter contactFolder com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="ce4bf-146">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="ce4bf-147">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ce4bf-147">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="ce4bf-148">Obtenha uma contactFolder que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-148">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="ce4bf-149">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce4bf-149">Properties</span></span>
| <span data-ttu-id="ce4bf-150">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce4bf-150">Property</span></span>     | <span data-ttu-id="ce4bf-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce4bf-151">Type</span></span>   |<span data-ttu-id="ce4bf-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce4bf-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce4bf-153">displayName</span><span class="sxs-lookup"><span data-stu-id="ce4bf-153">displayName</span></span>|<span data-ttu-id="ce4bf-154">String</span><span class="sxs-lookup"><span data-stu-id="ce4bf-154">String</span></span>|<span data-ttu-id="ce4bf-155">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-155">The folder's display name.</span></span>|
|<span data-ttu-id="ce4bf-156">id</span><span class="sxs-lookup"><span data-stu-id="ce4bf-156">id</span></span>|<span data-ttu-id="ce4bf-157">String</span><span class="sxs-lookup"><span data-stu-id="ce4bf-157">String</span></span>|<span data-ttu-id="ce4bf-p102">Identificador exclusivo da pasta de contatos. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-p102">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="ce4bf-160">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="ce4bf-160">parentFolderId</span></span>|<span data-ttu-id="ce4bf-161">String</span><span class="sxs-lookup"><span data-stu-id="ce4bf-161">String</span></span>|<span data-ttu-id="ce4bf-162">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-162">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="ce4bf-163">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="ce4bf-163">wellKnownName</span></span>|<span data-ttu-id="ce4bf-164">string</span><span class="sxs-lookup"><span data-stu-id="ce4bf-164">string</span></span>|<span data-ttu-id="ce4bf-165">O nome da pasta se a pasta for uma pasta reconhecida.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-165">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="ce4bf-166">No momento `contacts` é a única pasta Contatos reconhecidas.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-166">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce4bf-167">Relações</span><span class="sxs-lookup"><span data-stu-id="ce4bf-167">Relationships</span></span>
| <span data-ttu-id="ce4bf-168">Relação</span><span class="sxs-lookup"><span data-stu-id="ce4bf-168">Relationship</span></span> | <span data-ttu-id="ce4bf-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce4bf-169">Type</span></span>   |<span data-ttu-id="ce4bf-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce4bf-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce4bf-171">childFolders</span><span class="sxs-lookup"><span data-stu-id="ce4bf-171">childFolders</span></span>|<span data-ttu-id="ce4bf-172">Coleção [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="ce4bf-172">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="ce4bf-p104">A coleção de pastas filho na pasta. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-p104">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="ce4bf-177">contatos</span><span class="sxs-lookup"><span data-stu-id="ce4bf-177">contacts</span></span>|<span data-ttu-id="ce4bf-178">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="ce4bf-178">[Contact](contact.md) collection</span></span>|<span data-ttu-id="ce4bf-p105">Os contatos na pasta. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-p105">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="ce4bf-183">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="ce4bf-183">multiValueExtendedProperties</span></span>|<span data-ttu-id="ce4bf-184">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="ce4bf-184">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="ce4bf-p106">A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-p106">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="ce4bf-188">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="ce4bf-188">singleValueExtendedProperties</span></span>|<span data-ttu-id="ce4bf-189">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="ce4bf-189">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="ce4bf-p107">A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ce4bf-p107">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ce4bf-193">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce4bf-193">JSON representation</span></span>

<span data-ttu-id="ce4bf-194">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ce4bf-194">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="ce4bf-195">Confira também</span><span class="sxs-lookup"><span data-stu-id="ce4bf-195">See also</span></span>

- [<span data-ttu-id="ce4bf-196">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ce4bf-196">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="ce4bf-197">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="ce4bf-197">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
