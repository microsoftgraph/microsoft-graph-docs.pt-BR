---
title: tipo de recurso contactFolder
description: Uma pasta que contém contatos.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 10e48459645c8af6d03787a3b2395398098cc7e0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998926"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="399a5-103">tipo de recurso contactFolder</span><span class="sxs-lookup"><span data-stu-id="399a5-103">contactFolder resource type</span></span>

<span data-ttu-id="399a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="399a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="399a5-105">Uma pasta que contém contatos.</span><span class="sxs-lookup"><span data-stu-id="399a5-105">A folder that contains contacts.</span></span>

<span data-ttu-id="399a5-106">Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/contactfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="399a5-106">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="399a5-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="399a5-107">Methods</span></span>

| <span data-ttu-id="399a5-108">Método</span><span class="sxs-lookup"><span data-stu-id="399a5-108">Method</span></span>       | <span data-ttu-id="399a5-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="399a5-109">Return Type</span></span>  |<span data-ttu-id="399a5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="399a5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="399a5-111">Obter contactFolder</span><span class="sxs-lookup"><span data-stu-id="399a5-111">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="399a5-112">contactFolder</span><span class="sxs-lookup"><span data-stu-id="399a5-112">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="399a5-113">Obtenha uma pasta de contatos usando a respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="399a5-113">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="399a5-114">Update</span><span class="sxs-lookup"><span data-stu-id="399a5-114">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="399a5-115">contactFolder</span><span class="sxs-lookup"><span data-stu-id="399a5-115">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="399a5-116">Atualize o objeto contactFolder.</span><span class="sxs-lookup"><span data-stu-id="399a5-116">Update contactFolder object.</span></span> |
|[<span data-ttu-id="399a5-117">Delete</span><span class="sxs-lookup"><span data-stu-id="399a5-117">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="399a5-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="399a5-118">None</span></span> |<span data-ttu-id="399a5-119">Exclua um objeto contactFolder.</span><span class="sxs-lookup"><span data-stu-id="399a5-119">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="399a5-120">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="399a5-120">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="399a5-121">Coleção [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="399a5-121">[contactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="399a5-122">Obtenha uma coleção de pastas filho sob a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="399a5-122">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="399a5-123">Criar contactFolder filho</span><span class="sxs-lookup"><span data-stu-id="399a5-123">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="399a5-124">contactFolder</span><span class="sxs-lookup"><span data-stu-id="399a5-124">contactFolder</span></span>](contactfolder.md)| <span data-ttu-id="399a5-125">Cria uma nova contactFolder como um filho de uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="399a5-125">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="399a5-126">delta</span><span class="sxs-lookup"><span data-stu-id="399a5-126">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="399a5-127">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="399a5-127">[contact](contact.md) collection</span></span>| <span data-ttu-id="399a5-128">Obtenha um conjunto de pastas de contatos que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="399a5-128">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="399a5-129">Listar contatos na pasta</span><span class="sxs-lookup"><span data-stu-id="399a5-129">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="399a5-130">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="399a5-130">[contact](contact.md) collection</span></span>| <span data-ttu-id="399a5-131">Obtém uma coleção de contatos da pasta de contatos padrão do usuário conectado (`.../me/contacts`), ou da pasta contato especificada.</span><span class="sxs-lookup"><span data-stu-id="399a5-131">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="399a5-132">Criar contato na pasta</span><span class="sxs-lookup"><span data-stu-id="399a5-132">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="399a5-133">contato</span><span class="sxs-lookup"><span data-stu-id="399a5-133">contact</span></span>](contact.md)| <span data-ttu-id="399a5-134">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade do `contacts` de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="399a5-134">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|<span data-ttu-id="399a5-135">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="399a5-135">**Extended properties**</span></span>| | |
|[<span data-ttu-id="399a5-136">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="399a5-136">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="399a5-137">contactFolder</span><span class="sxs-lookup"><span data-stu-id="399a5-137">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="399a5-138">Criar uma ou mais propriedades estendidas de valor único em uma contactFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="399a5-138">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="399a5-139">Obter contactFolder com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="399a5-139">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="399a5-140">contactFolder</span><span class="sxs-lookup"><span data-stu-id="399a5-140">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="399a5-141">Obtenha contactFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="399a5-141">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="399a5-142">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="399a5-142">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="399a5-143">contactFolder</span><span class="sxs-lookup"><span data-stu-id="399a5-143">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="399a5-144">Criar uma ou mais propriedades estendidas de vários valores em uma contactFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="399a5-144">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="399a5-145">Obter contactFolder com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="399a5-145">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="399a5-146">contactFolder</span><span class="sxs-lookup"><span data-stu-id="399a5-146">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="399a5-147">Obtenha uma contactFolder que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="399a5-147">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="399a5-148">Propriedades</span><span class="sxs-lookup"><span data-stu-id="399a5-148">Properties</span></span>
| <span data-ttu-id="399a5-149">Propriedade</span><span class="sxs-lookup"><span data-stu-id="399a5-149">Property</span></span>     | <span data-ttu-id="399a5-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="399a5-150">Type</span></span>   |<span data-ttu-id="399a5-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="399a5-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="399a5-152">displayName</span><span class="sxs-lookup"><span data-stu-id="399a5-152">displayName</span></span>|<span data-ttu-id="399a5-153">String</span><span class="sxs-lookup"><span data-stu-id="399a5-153">String</span></span>|<span data-ttu-id="399a5-154">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="399a5-154">The folder's display name.</span></span>|
|<span data-ttu-id="399a5-155">id</span><span class="sxs-lookup"><span data-stu-id="399a5-155">id</span></span>|<span data-ttu-id="399a5-156">String</span><span class="sxs-lookup"><span data-stu-id="399a5-156">String</span></span>|<span data-ttu-id="399a5-p101">Identificador exclusivo da pasta de contatos. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="399a5-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="399a5-159">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="399a5-159">parentFolderId</span></span>|<span data-ttu-id="399a5-160">String</span><span class="sxs-lookup"><span data-stu-id="399a5-160">String</span></span>|<span data-ttu-id="399a5-161">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="399a5-161">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="399a5-162">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="399a5-162">wellKnownName</span></span>|<span data-ttu-id="399a5-163">string</span><span class="sxs-lookup"><span data-stu-id="399a5-163">string</span></span>|<span data-ttu-id="399a5-164">O nome da pasta se a pasta for uma pasta reconhecida.</span><span class="sxs-lookup"><span data-stu-id="399a5-164">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="399a5-165">Atualmente `contacts` é a única pasta de contatos reconhecida.</span><span class="sxs-lookup"><span data-stu-id="399a5-165">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="399a5-166">Relações</span><span class="sxs-lookup"><span data-stu-id="399a5-166">Relationships</span></span>
| <span data-ttu-id="399a5-167">Relação</span><span class="sxs-lookup"><span data-stu-id="399a5-167">Relationship</span></span> | <span data-ttu-id="399a5-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="399a5-168">Type</span></span>   |<span data-ttu-id="399a5-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="399a5-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="399a5-170">childFolders</span><span class="sxs-lookup"><span data-stu-id="399a5-170">childFolders</span></span>|<span data-ttu-id="399a5-171">Coleção [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="399a5-171">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="399a5-p103">A coleção de pastas filho na pasta. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="399a5-p103">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="399a5-176">contatos</span><span class="sxs-lookup"><span data-stu-id="399a5-176">contacts</span></span>|<span data-ttu-id="399a5-177">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="399a5-177">[Contact](contact.md) collection</span></span>|<span data-ttu-id="399a5-p104">Os contatos na pasta. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="399a5-p104">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="399a5-182">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="399a5-182">multiValueExtendedProperties</span></span>|<span data-ttu-id="399a5-183">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="399a5-183">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="399a5-p105">A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="399a5-p105">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="399a5-187">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="399a5-187">singleValueExtendedProperties</span></span>|<span data-ttu-id="399a5-188">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="399a5-188">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="399a5-p106">A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="399a5-p106">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="399a5-192">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="399a5-192">JSON representation</span></span>

<span data-ttu-id="399a5-193">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="399a5-193">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="399a5-194">Confira também</span><span class="sxs-lookup"><span data-stu-id="399a5-194">See also</span></span>

- [<span data-ttu-id="399a5-195">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="399a5-195">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="399a5-196">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="399a5-196">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


