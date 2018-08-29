# <a name="directoryobject-resource-type"></a><span data-ttu-id="28b85-101">tipo de recurso directoryObject</span><span class="sxs-lookup"><span data-stu-id="28b85-101">directoryObject resource type</span></span>

<span data-ttu-id="28b85-p101">Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.</span><span class="sxs-lookup"><span data-stu-id="28b85-p101">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="28b85-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="28b85-104">Methods</span></span>

| <span data-ttu-id="28b85-105">Método</span><span class="sxs-lookup"><span data-stu-id="28b85-105">Method</span></span>       | <span data-ttu-id="28b85-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="28b85-106">Return Type</span></span>  |<span data-ttu-id="28b85-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="28b85-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="28b85-108">Obter directoryObject</span><span class="sxs-lookup"><span data-stu-id="28b85-108">Get directoryObject</span></span>](../api/directoryobject_get.md) | [<span data-ttu-id="28b85-109">directoryObject</span><span class="sxs-lookup"><span data-stu-id="28b85-109">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="28b85-110">Ler as propriedades de um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="28b85-110">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="28b85-111">Excluir directoryObject</span><span class="sxs-lookup"><span data-stu-id="28b85-111">Delete directoryObject</span></span>](../api/directoryobject_delete.md) | <span data-ttu-id="28b85-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="28b85-112">None</span></span> |<span data-ttu-id="28b85-113">Excluir um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="28b85-113">Delete a directory object.</span></span> |
|[<span data-ttu-id="28b85-114">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="28b85-114">checkMemberGroups</span></span>](../api/directoryobject_checkmembergroups.md)|<span data-ttu-id="28b85-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="28b85-115">String collection</span></span>|<span data-ttu-id="28b85-p102">Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="28b85-p102">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="28b85-118">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="28b85-118">getMemberGroups</span></span>](../api/directoryobject_getmembergroups.md)|<span data-ttu-id="28b85-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="28b85-119">String collection</span></span>|<span data-ttu-id="28b85-p103">Retornar todos os grupos dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="28b85-p103">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="28b85-122">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="28b85-122">getMemberObjects</span></span>](../api/directoryobject_getmemberobjects.md)|<span data-ttu-id="28b85-123">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="28b85-123">String collection</span></span>| <span data-ttu-id="28b85-p104">Retornar todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="28b85-p104">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="28b85-126">getByIds</span><span class="sxs-lookup"><span data-stu-id="28b85-126">getByIds</span></span>](../api/directoryobject_getbyids.md) | <span data-ttu-id="28b85-127">coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="28b85-127">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="28b85-128">Obter um conjunto de objetos de diretório com base em um conjunto de ids fornecidas.</span><span class="sxs-lookup"><span data-stu-id="28b85-128">Get a set of directory objects based on a set of supplied ids.</span></span> |

## <a name="properties"></a><span data-ttu-id="28b85-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28b85-129">Properties</span></span>

| <span data-ttu-id="28b85-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28b85-130">Property</span></span>   | <span data-ttu-id="28b85-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="28b85-131">Type</span></span> |<span data-ttu-id="28b85-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="28b85-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28b85-133">id</span><span class="sxs-lookup"><span data-stu-id="28b85-133">id</span></span>|<span data-ttu-id="28b85-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28b85-134">String</span></span>|<span data-ttu-id="28b85-p105">Um GUID que é o identificador exclusivo do objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde. Chave. Não anulável. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="28b85-p105">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28b85-139">Relações</span><span class="sxs-lookup"><span data-stu-id="28b85-139">Relationships</span></span>

<span data-ttu-id="28b85-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="28b85-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="28b85-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28b85-141">JSON representation</span></span>

<span data-ttu-id="28b85-142">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="28b85-142">Here is a JSON representation of the resource</span></span>

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
