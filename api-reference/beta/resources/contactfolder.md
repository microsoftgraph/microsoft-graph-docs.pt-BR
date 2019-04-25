---
title: tipo de recurso contactFolder
description: Uma pasta que contém contatos.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 599f1765b6305d2dc4d482ec035ee4b24eb5183a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543382"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="0ff91-103">tipo de recurso contactFolder</span><span class="sxs-lookup"><span data-stu-id="0ff91-103">contactFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ff91-104">Uma pasta que contém contatos.</span><span class="sxs-lookup"><span data-stu-id="0ff91-104">A folder that contains contacts.</span></span>

<span data-ttu-id="0ff91-105">Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/contactfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="0ff91-105">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="0ff91-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="0ff91-106">Methods</span></span>

| <span data-ttu-id="0ff91-107">Método</span><span class="sxs-lookup"><span data-stu-id="0ff91-107">Method</span></span>       | <span data-ttu-id="0ff91-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0ff91-108">Return Type</span></span>  |<span data-ttu-id="0ff91-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ff91-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0ff91-110">Obter contactFolder</span><span class="sxs-lookup"><span data-stu-id="0ff91-110">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="0ff91-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="0ff91-111">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="0ff91-112">Obtenha uma pasta de contatos usando a respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="0ff91-112">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="0ff91-113">Update</span><span class="sxs-lookup"><span data-stu-id="0ff91-113">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="0ff91-114">contactFolder</span><span class="sxs-lookup"><span data-stu-id="0ff91-114">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="0ff91-115">Atualize o objeto contactFolder.</span><span class="sxs-lookup"><span data-stu-id="0ff91-115">Update contactFolder object.</span></span> |
|[<span data-ttu-id="0ff91-116">Excluir</span><span class="sxs-lookup"><span data-stu-id="0ff91-116">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="0ff91-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0ff91-117">None</span></span> |<span data-ttu-id="0ff91-118">Exclua um objeto contactFolder.</span><span class="sxs-lookup"><span data-stu-id="0ff91-118">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="0ff91-119">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="0ff91-119">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="0ff91-120">Coleção [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="0ff91-120">[contactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="0ff91-121">Obtenha uma coleção de pastas filho sob a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="0ff91-121">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="0ff91-122">Criar contactFolder filho</span><span class="sxs-lookup"><span data-stu-id="0ff91-122">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="0ff91-123">contactFolder</span><span class="sxs-lookup"><span data-stu-id="0ff91-123">contactFolder</span></span>](contactfolder.md)| <span data-ttu-id="0ff91-124">Cria uma nova contactFolder como um filho de uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="0ff91-124">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="0ff91-125">delta</span><span class="sxs-lookup"><span data-stu-id="0ff91-125">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="0ff91-126">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="0ff91-126">[contact](contact.md) collection</span></span>| <span data-ttu-id="0ff91-127">Obtenha um conjunto de pastas de contatos que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="0ff91-127">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="0ff91-128">Listar contatos na pasta</span><span class="sxs-lookup"><span data-stu-id="0ff91-128">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="0ff91-129">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="0ff91-129">[contact](contact.md) collection</span></span>| <span data-ttu-id="0ff91-130">Obtém uma coleção de contatos da pasta de contatos padrão do usuário conectado (`.../me/contacts`), ou da pasta contato especificada.</span><span class="sxs-lookup"><span data-stu-id="0ff91-130">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="0ff91-131">Criar contato na pasta</span><span class="sxs-lookup"><span data-stu-id="0ff91-131">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="0ff91-132">contato</span><span class="sxs-lookup"><span data-stu-id="0ff91-132">contact</span></span>](contact.md)| <span data-ttu-id="0ff91-133">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade do `contacts` de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="0ff91-133">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|<span data-ttu-id="0ff91-134">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="0ff91-134">**Extended properties**</span></span>| | |
|[<span data-ttu-id="0ff91-135">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="0ff91-135">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="0ff91-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="0ff91-136">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="0ff91-137">Criar uma ou mais propriedades estendidas de valor único em uma contactFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="0ff91-137">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="0ff91-138">Obter contactFolder com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="0ff91-138">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="0ff91-139">contactFolder</span><span class="sxs-lookup"><span data-stu-id="0ff91-139">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="0ff91-140">Obtenha contactFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="0ff91-140">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="0ff91-141">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="0ff91-141">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="0ff91-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="0ff91-142">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="0ff91-143">Criar uma ou mais propriedades estendidas de vários valores em uma contactFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="0ff91-143">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="0ff91-144">Obter contactFolder com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="0ff91-144">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="0ff91-145">contactFolder</span><span class="sxs-lookup"><span data-stu-id="0ff91-145">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="0ff91-146">Obtenha uma contactFolder que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="0ff91-146">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="0ff91-147">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ff91-147">Properties</span></span>
| <span data-ttu-id="0ff91-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ff91-148">Property</span></span>     | <span data-ttu-id="0ff91-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ff91-149">Type</span></span>   |<span data-ttu-id="0ff91-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ff91-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ff91-151">displayName</span><span class="sxs-lookup"><span data-stu-id="0ff91-151">displayName</span></span>|<span data-ttu-id="0ff91-152">String</span><span class="sxs-lookup"><span data-stu-id="0ff91-152">String</span></span>|<span data-ttu-id="0ff91-153">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="0ff91-153">The folder's display name.</span></span>|
|<span data-ttu-id="0ff91-154">id</span><span class="sxs-lookup"><span data-stu-id="0ff91-154">id</span></span>|<span data-ttu-id="0ff91-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ff91-155">String</span></span>|<span data-ttu-id="0ff91-p101">Identificador exclusivo da pasta de contatos. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ff91-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="0ff91-158">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="0ff91-158">parentFolderId</span></span>|<span data-ttu-id="0ff91-159">String</span><span class="sxs-lookup"><span data-stu-id="0ff91-159">String</span></span>|<span data-ttu-id="0ff91-160">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="0ff91-160">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="0ff91-161">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="0ff91-161">wellKnownName</span></span>|<span data-ttu-id="0ff91-162">string</span><span class="sxs-lookup"><span data-stu-id="0ff91-162">string</span></span>|<span data-ttu-id="0ff91-163">O nome da pasta se a pasta for uma pasta reconhecida.</span><span class="sxs-lookup"><span data-stu-id="0ff91-163">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="0ff91-164">Atualmente `contacts` é a única pasta de contatos reconhecida.</span><span class="sxs-lookup"><span data-stu-id="0ff91-164">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ff91-165">Relações</span><span class="sxs-lookup"><span data-stu-id="0ff91-165">Relationships</span></span>
| <span data-ttu-id="0ff91-166">Relação</span><span class="sxs-lookup"><span data-stu-id="0ff91-166">Relationship</span></span> | <span data-ttu-id="0ff91-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ff91-167">Type</span></span>   |<span data-ttu-id="0ff91-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ff91-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ff91-169">childFolders</span><span class="sxs-lookup"><span data-stu-id="0ff91-169">childFolders</span></span>|<span data-ttu-id="0ff91-170">Coleção [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="0ff91-170">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="0ff91-p103">A coleção de pastas filho na pasta. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0ff91-p103">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="0ff91-175">contatos</span><span class="sxs-lookup"><span data-stu-id="0ff91-175">contacts</span></span>|<span data-ttu-id="0ff91-176">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="0ff91-176">[Contact](contact.md) collection</span></span>|<span data-ttu-id="0ff91-p104">Os contatos na pasta. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0ff91-p104">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="0ff91-181">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="0ff91-181">multiValueExtendedProperties</span></span>|<span data-ttu-id="0ff91-182">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="0ff91-182">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="0ff91-p105">A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0ff91-p105">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="0ff91-186">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="0ff91-186">singleValueExtendedProperties</span></span>|<span data-ttu-id="0ff91-187">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="0ff91-187">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="0ff91-p106">A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0ff91-p106">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ff91-191">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ff91-191">JSON representation</span></span>

<span data-ttu-id="0ff91-192">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0ff91-192">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="0ff91-193">Confira também</span><span class="sxs-lookup"><span data-stu-id="0ff91-193">See also</span></span>

- [<span data-ttu-id="0ff91-194">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0ff91-194">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="0ff91-195">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="0ff91-195">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/contactfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
