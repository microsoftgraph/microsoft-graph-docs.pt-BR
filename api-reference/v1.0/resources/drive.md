# <a name="drive-resource-type"></a><span data-ttu-id="d9750-101">Tipo de unidade de recurso</span><span class="sxs-lookup"><span data-stu-id="d9750-101">Drive resource type</span></span>

<span data-ttu-id="d9750-102">O recurso drive é o objeto de nível superior que representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d9750-102">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="d9750-p101">Os usuários do OneDrive sempre terão pelo menos uma unidade disponível, sua unidade padrão. Usuários sem uma licença do OneDrive talvez não tenham uma unidade padrão disponível.</span><span class="sxs-lookup"><span data-stu-id="d9750-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9750-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9750-105">JSON representation</span></span>

<span data-ttu-id="d9750-106">Veja a seguir uma representação JSON de um recurso **drive**.</span><span class="sxs-lookup"><span data-stu-id="d9750-106">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="d9750-107">O recurso **drive** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="d9750-107">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "items", "root", "special", "owner", "description" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "id": "string (identifier)",
  "driveType": "string",
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "quota": {"@odata.type": "microsoft.graph.quota"},
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "root": {"@odata.type": "microsoft.graph.driveItem" },
  "items": [ {"@odata.type": "microsoft.graph.driveItem" }],
  "special": [ {"@odata.type": "microsoft.graph.driveItem" }],

  /* inherited from baseItem */
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="d9750-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9750-108">Properties</span></span>

| <span data-ttu-id="d9750-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9750-109">Property</span></span>             | <span data-ttu-id="d9750-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9750-110">Type</span></span>                          | <span data-ttu-id="d9750-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9750-111">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d9750-112">id</span><span class="sxs-lookup"><span data-stu-id="d9750-112">id</span></span>                   | <span data-ttu-id="d9750-113">String</span><span class="sxs-lookup"><span data-stu-id="d9750-113">String</span></span>                        | <span data-ttu-id="d9750-p102">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9750-p102">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="d9750-116">createdBy</span><span class="sxs-lookup"><span data-stu-id="d9750-116">createdBy</span></span>            | <span data-ttu-id="d9750-117">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d9750-117">[identitySet][]</span></span>               | <span data-ttu-id="d9750-p103">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9750-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="d9750-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9750-120">createdDateTime</span></span>      | <span data-ttu-id="d9750-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9750-121">dateTimeOffset</span></span>                | <span data-ttu-id="d9750-p104">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9750-p104">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="d9750-124">driveType</span><span class="sxs-lookup"><span data-stu-id="d9750-124">driveType</span></span>            | <span data-ttu-id="d9750-125">String</span><span class="sxs-lookup"><span data-stu-id="d9750-125">String</span></span>                        | <span data-ttu-id="d9750-p105">Descreve o tipo de unidade representado por esse recurso. As unidades pessoais do OneDrive retornarão `personal`. O OneDrive for Business retornará `business`. As bibliotecas de documentos do SharePoint retornarão `documentLibrary`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9750-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="d9750-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d9750-131">lastModifiedBy</span></span>       | <span data-ttu-id="d9750-132">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d9750-132">[identitySet][]</span></span>               | <span data-ttu-id="d9750-p106">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9750-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="d9750-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9750-135">lastModifiedDateTime</span></span> | <span data-ttu-id="d9750-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9750-136">dateTimeOffset</span></span>                | <span data-ttu-id="d9750-p107">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9750-p107">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="d9750-139">nome</span><span class="sxs-lookup"><span data-stu-id="d9750-139">name</span></span>                 | <span data-ttu-id="d9750-140">string</span><span class="sxs-lookup"><span data-stu-id="d9750-140">string</span></span>                        | <span data-ttu-id="d9750-p108">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="d9750-p108">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="d9750-143">owner</span><span class="sxs-lookup"><span data-stu-id="d9750-143">owner</span></span>                | [<span data-ttu-id="d9750-144">identitySet</span><span class="sxs-lookup"><span data-stu-id="d9750-144">identitySet</span></span>](identityset.md) | <span data-ttu-id="d9750-p109">Opcional. A conta do usuário que é proprietário da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9750-p109">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="d9750-148">cota</span><span class="sxs-lookup"><span data-stu-id="d9750-148">quota</span></span>                | [<span data-ttu-id="d9750-149">quota</span><span class="sxs-lookup"><span data-stu-id="d9750-149">quota</span></span>](quota.md)             | <span data-ttu-id="d9750-p110">Opcional. Informações sobre a cota de espaço de armazenamento da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9750-p110">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="d9750-153">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="d9750-153">sharepointIds</span></span>        | <span data-ttu-id="d9750-154">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="d9750-154">[sharepointIds][]</span></span>             | <span data-ttu-id="d9750-p111">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9750-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="d9750-157">webUrl</span><span class="sxs-lookup"><span data-stu-id="d9750-157">webUrl</span></span>               | <span data-ttu-id="d9750-158">string (url)</span><span class="sxs-lookup"><span data-stu-id="d9750-158">string (url)</span></span>                  | <span data-ttu-id="d9750-p112">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9750-p112">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

<span data-ttu-id="d9750-161">[identitySet]: identityset.md</span><span class="sxs-lookup"><span data-stu-id="d9750-161">[identitySet]: identityset.md</span></span>
<span data-ttu-id="d9750-162">[sharepointIds]: sharepointids.md</span><span class="sxs-lookup"><span data-stu-id="d9750-162">[sharepointIds]: sharepointids.md</span></span>

## <a name="relationships"></a><span data-ttu-id="d9750-163">Relações</span><span class="sxs-lookup"><span data-stu-id="d9750-163">Relationships</span></span>

| <span data-ttu-id="d9750-164">Relação</span><span class="sxs-lookup"><span data-stu-id="d9750-164">Relationship</span></span> | <span data-ttu-id="d9750-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9750-165">Type</span></span>                                 | <span data-ttu-id="d9750-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9750-166">Description</span></span>                                                              |
| :----------- | :----------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="d9750-167">items</span><span class="sxs-lookup"><span data-stu-id="d9750-167">items</span></span>        | <span data-ttu-id="d9750-168">Coleção [driveitem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="d9750-168">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="d9750-p113">Todos os itens contidos na unidade. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="d9750-p113">All items contained in the drive. Read-only. Nullable.</span></span>                   |
| <span data-ttu-id="d9750-172">root</span><span class="sxs-lookup"><span data-stu-id="d9750-172">root</span></span>         | [<span data-ttu-id="d9750-173">driveitem</span><span class="sxs-lookup"><span data-stu-id="d9750-173">driveitem</span></span>](driveitem.md)            | <span data-ttu-id="d9750-p114">A pasta raiz da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9750-p114">The root folder of the drive. Read-only.</span></span>                                 |
| <span data-ttu-id="d9750-176">special</span><span class="sxs-lookup"><span data-stu-id="d9750-176">special</span></span>      | <span data-ttu-id="d9750-177">Coleção [driveitem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="d9750-177">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="d9750-p115">Coleção de pastas comuns disponíveis no OneDrive. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="d9750-p115">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span> |

## <a name="methods"></a><span data-ttu-id="d9750-181">Métodos</span><span class="sxs-lookup"><span data-stu-id="d9750-181">Methods</span></span>

<span data-ttu-id="d9750-182">Os métodos a seguir estão disponíveis para os recursos drive.</span><span class="sxs-lookup"><span data-stu-id="d9750-182">The following methods are available for drive resources.</span></span>

| <span data-ttu-id="d9750-183">Método</span><span class="sxs-lookup"><span data-stu-id="d9750-183">Method</span></span>                                                | <span data-ttu-id="d9750-184">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="d9750-184">REST Path</span></span>                        |
| :---------------------------------------------------- | :------------------------------- |
| [<span data-ttu-id="d9750-185">Obter unidade padrão do usuário</span><span class="sxs-lookup"><span data-stu-id="d9750-185">Get user's default drive</span></span>](../api/drive_get.md)       | `GET /me/drive`                  |
| [<span data-ttu-id="d9750-186">Obter a unidade de outro usuário</span><span class="sxs-lookup"><span data-stu-id="d9750-186">Get another user's drive</span></span>](../api/drive_get.md)       | `GET /users/{user-id}/drive`     |
| [<span data-ttu-id="d9750-187">Obter pasta raiz de uma unidade</span><span class="sxs-lookup"><span data-stu-id="d9750-187">Get root folder for a drive</span></span>](../api/item_get.md)     | `GET /drives/{drive-id}/root`    |
| [<span data-ttu-id="d9750-188">Listar itens em uma unidade</span><span class="sxs-lookup"><span data-stu-id="d9750-188">List items in a drive</span></span>](../api/item_list_children.md) | `GET /me/drive/root/children`    |
| [<span data-ttu-id="d9750-189">Listar alterações em uma unidade</span><span class="sxs-lookup"><span data-stu-id="d9750-189">List changes in a drive</span></span>](../api/item_delta.md)       | `GET /me/drive/root/delta`       |
| [<span data-ttu-id="d9750-190">Pesquisar itens em uma unidade</span><span class="sxs-lookup"><span data-stu-id="d9750-190">Search items in a drive</span></span>](../api/item_search.md)      | `GET /me/drive/search(q='text')` |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "drive resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive"
}-->
