# <a name="contactfolder-resource-type"></a><span data-ttu-id="3506b-101">tipo de recurso contactFolder</span><span class="sxs-lookup"><span data-stu-id="3506b-101">contactFolder resource type</span></span>

<span data-ttu-id="3506b-102">Uma pasta que contém contatos.</span><span class="sxs-lookup"><span data-stu-id="3506b-102">A folder that contains contacts.</span></span>

<span data-ttu-id="3506b-103">Esse recurso suporta a utilização da [consulta delta](../../../concepts/delta_query_overview.md) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/contactfolder_delta.md).</span><span class="sxs-lookup"><span data-stu-id="3506b-103">This resource supports using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder_delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="3506b-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="3506b-104">Methods</span></span>

| <span data-ttu-id="3506b-105">Método</span><span class="sxs-lookup"><span data-stu-id="3506b-105">Method</span></span>       | <span data-ttu-id="3506b-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3506b-106">Return Type</span></span>  |<span data-ttu-id="3506b-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="3506b-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3506b-108">Obter contactFolder</span><span class="sxs-lookup"><span data-stu-id="3506b-108">Get contactFolder</span></span>](../api/contactfolder_get.md) | [<span data-ttu-id="3506b-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3506b-109">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="3506b-110">Obtenha uma pasta de contatos usando a respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="3506b-110">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="3506b-111">Atualizar</span><span class="sxs-lookup"><span data-stu-id="3506b-111">Update</span></span>](../api/contactfolder_update.md) | [<span data-ttu-id="3506b-112">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3506b-112">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="3506b-113">Atualize o objeto contactFolder.</span><span class="sxs-lookup"><span data-stu-id="3506b-113">Update contactFolder object.</span></span> |
|[<span data-ttu-id="3506b-114">Excluir</span><span class="sxs-lookup"><span data-stu-id="3506b-114">Delete</span></span>](../api/contactfolder_delete.md) | <span data-ttu-id="3506b-115">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3506b-115">None</span></span> |<span data-ttu-id="3506b-116">Exclua um objeto contactFolder.</span><span class="sxs-lookup"><span data-stu-id="3506b-116">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="3506b-117">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="3506b-117">List childFolders</span></span>](../api/contactfolder_list_childfolders.md) |<span data-ttu-id="3506b-118">Coleção [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="3506b-118">[ContactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="3506b-119">Obtenha uma coleção de pastas filho sob a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="3506b-119">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="3506b-120">Criar contactFolder filho</span><span class="sxs-lookup"><span data-stu-id="3506b-120">Create child contactFolder</span></span>](../api/contactfolder_post_childfolders.md) |[<span data-ttu-id="3506b-121">ContactFolder</span><span class="sxs-lookup"><span data-stu-id="3506b-121">ContactFolder</span></span>](contactfolder.md)| <span data-ttu-id="3506b-122">Crie uma nova contactFolder como um filho de uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="3506b-122">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="3506b-123">delta</span><span class="sxs-lookup"><span data-stu-id="3506b-123">delta</span></span>](../api/contact_delta.md)|<span data-ttu-id="3506b-124">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="3506b-124">[contact](contact.md) collection</span></span>| <span data-ttu-id="3506b-125">Obtenha um conjunto de pastas de contatos que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="3506b-125">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="3506b-126">Listar contatos na pasta</span><span class="sxs-lookup"><span data-stu-id="3506b-126">List contacts in folder</span></span>](../api/contactfolder_list_contacts.md) |<span data-ttu-id="3506b-127">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="3506b-127">[Contact](contact.md) collection</span></span>| <span data-ttu-id="3506b-128">Obtém uma coleção de contatos da pasta de contatos padrão do usuário conectado (`.../me/contacts`), ou da pasta contato especificada.</span><span class="sxs-lookup"><span data-stu-id="3506b-128">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="3506b-129">Criar contato na pasta</span><span class="sxs-lookup"><span data-stu-id="3506b-129">Create contact in folder</span></span>](../api/contactfolder_post_contacts.md) |[<span data-ttu-id="3506b-130">Contato</span><span class="sxs-lookup"><span data-stu-id="3506b-130">Contact</span></span>](contact.md)| <span data-ttu-id="3506b-131">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de `contacts` de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="3506b-131">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="3506b-132">Criar propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="3506b-132">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="3506b-133">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3506b-133">contactFolder</span></span>](contactFolder.md)  |<span data-ttu-id="3506b-134">Criar uma ou mais propriedades estendidas de valor único em uma contactFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="3506b-134">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="3506b-135">Obter contactFolder com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="3506b-135">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="3506b-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3506b-136">contactFolder</span></span>](contactFolder.md) | <span data-ttu-id="3506b-137">Obtenha contactFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="3506b-137">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="3506b-138">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="3506b-138">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="3506b-139">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3506b-139">contactFolder</span></span>](contactFolder.md) | <span data-ttu-id="3506b-140">Criar uma ou mais propriedades estendidas de vários valores em uma contactFolder nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="3506b-140">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="3506b-141">Obter contactFolder com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="3506b-141">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="3506b-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3506b-142">contactFolder</span></span>](contactFolder.md) | <span data-ttu-id="3506b-143">Obtenha uma contactFolder que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="3506b-143">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="3506b-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3506b-144">Properties</span></span>
| <span data-ttu-id="3506b-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3506b-145">Property</span></span>     | <span data-ttu-id="3506b-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="3506b-146">Type</span></span>   |<span data-ttu-id="3506b-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="3506b-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3506b-148">displayName</span><span class="sxs-lookup"><span data-stu-id="3506b-148">displayName</span></span>|<span data-ttu-id="3506b-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3506b-149">String</span></span>|<span data-ttu-id="3506b-150">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="3506b-150">The folder's display name.</span></span>|
|<span data-ttu-id="3506b-151">id</span><span class="sxs-lookup"><span data-stu-id="3506b-151">id</span></span>|<span data-ttu-id="3506b-152">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="3506b-152">String</span></span>|<span data-ttu-id="3506b-p101">Identificador exclusivo da pasta de contatos. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3506b-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="3506b-155">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="3506b-155">parentFolderId</span></span>|<span data-ttu-id="3506b-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3506b-156">String</span></span>|<span data-ttu-id="3506b-157">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="3506b-157">The ID of the folder's parent folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3506b-158">Relações</span><span class="sxs-lookup"><span data-stu-id="3506b-158">Relationships</span></span>
| <span data-ttu-id="3506b-159">Relação</span><span class="sxs-lookup"><span data-stu-id="3506b-159">Relationship</span></span> | <span data-ttu-id="3506b-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="3506b-160">Type</span></span>   |<span data-ttu-id="3506b-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="3506b-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3506b-162">childFolders</span><span class="sxs-lookup"><span data-stu-id="3506b-162">childFolders</span></span>|<span data-ttu-id="3506b-163">Coleção [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="3506b-163">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="3506b-p102">A coleção de pastas filho na pasta. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="3506b-p102">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="3506b-168">contatos</span><span class="sxs-lookup"><span data-stu-id="3506b-168">contacts</span></span>|<span data-ttu-id="3506b-169">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="3506b-169">[Contact](contact.md) collection</span></span>|<span data-ttu-id="3506b-p103">Os contatos na pasta. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="3506b-p103">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="3506b-174">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="3506b-174">multiValueExtendedProperties</span></span>|<span data-ttu-id="3506b-175">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="3506b-175">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="3506b-p104">A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="3506b-p104">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="3506b-179">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="3506b-179">singleValueExtendedProperties</span></span>|<span data-ttu-id="3506b-180">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="3506b-180">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="3506b-p105">A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="3506b-p105">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3506b-184">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3506b-184">JSON representation</span></span>

<span data-ttu-id="3506b-185">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3506b-185">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="3506b-186">Confira também</span><span class="sxs-lookup"><span data-stu-id="3506b-186">See also</span></span>

- [<span data-ttu-id="3506b-187">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3506b-187">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="3506b-188">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="3506b-188">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
