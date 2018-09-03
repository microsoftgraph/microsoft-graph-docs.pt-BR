# <a name="driveitemversion-resource-type"></a><span data-ttu-id="e2613-101">Tipo de recurso DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="e2613-101">DriveItemVersion resource type</span></span>

<span data-ttu-id="e2613-102">O recurso **DriveItemVersion** representa uma versão específica de um [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e2613-102">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="e2613-103">Tarefas em recursos DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="e2613-103">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="e2613-104">As tarefas a seguir estão disponíveis para recursos driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="e2613-104">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="e2613-105">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="e2613-105">Common task</span></span>             |         <span data-ttu-id="e2613-106">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="e2613-106">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="e2613-107">[Versões de lista][version-list]</span><span class="sxs-lookup"><span data-stu-id="e2613-107">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="e2613-108">[Obter versão][version-get]</span><span class="sxs-lookup"><span data-stu-id="e2613-108">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="e2613-109">[Obter conteúdo][content-get]</span><span class="sxs-lookup"><span data-stu-id="e2613-109">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="e2613-110">[Restaurar versão][version-restore]</span><span class="sxs-lookup"><span data-stu-id="e2613-110">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem_list_versions.md
[version-get]: ../api/driveitemversion_get.md
[content-get]: ../api/driveitemversion_get_contents.md
[version-restore]: ../api/driveitemversion_restore.md

<span data-ttu-id="e2613-111">Na tabela anterior, os exemplos usam `/drive`, mas há muitas solicitações válidas.</span><span class="sxs-lookup"><span data-stu-id="e2613-111">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2613-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2613-112">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.driveItemVersion",
  "@type.aka": "oneDrive.driveItemVersion"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" },
  "size": 12356
}
```

## <a name="properties"></a><span data-ttu-id="e2613-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2613-113">Properties</span></span>

|      <span data-ttu-id="e2613-114">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e2613-114">Property name</span></span>       |                         <span data-ttu-id="e2613-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2613-115">Type</span></span>                         |                               <span data-ttu-id="e2613-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2613-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="e2613-117">**id**</span><span class="sxs-lookup"><span data-stu-id="e2613-117">**id**</span></span>                   | <span data-ttu-id="e2613-118">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2613-118">string</span></span>                                               | <span data-ttu-id="e2613-119">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="e2613-119">The ID of the version.</span></span> <span data-ttu-id="e2613-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e2613-120">Read-only.</span></span>                                       |
| <span data-ttu-id="e2613-121">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="e2613-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="e2613-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="e2613-122">IdentitySet</span></span>](../resources/identitySet.md)           | <span data-ttu-id="e2613-123">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e2613-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="e2613-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e2613-124">Read-only.</span></span>        |
| <span data-ttu-id="e2613-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e2613-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="e2613-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2613-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="e2613-127">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e2613-127">Date and time the version was last modified.</span></span> <span data-ttu-id="e2613-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e2613-128">Read-only.</span></span>                 |
| <span data-ttu-id="e2613-129">**publication**</span><span class="sxs-lookup"><span data-stu-id="e2613-129">**publication**</span></span>          | [<span data-ttu-id="e2613-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="e2613-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="e2613-131">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="e2613-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="e2613-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e2613-132">Read-only.</span></span> |
| <span data-ttu-id="e2613-133">**size**</span><span class="sxs-lookup"><span data-stu-id="e2613-133">**size**</span></span>                 | <span data-ttu-id="e2613-134">Int64</span><span class="sxs-lookup"><span data-stu-id="e2613-134">Int64</span></span>                                                | <span data-ttu-id="e2613-135">Indica o tamanho do fluxo de conteúdo para esta versão do item.</span><span class="sxs-lookup"><span data-stu-id="e2613-135">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="e2613-136">**content**</span><span class="sxs-lookup"><span data-stu-id="e2613-136">**content**</span></span>              | <span data-ttu-id="e2613-137">Fluxo</span><span class="sxs-lookup"><span data-stu-id="e2613-137">Stream</span></span>                                               | <span data-ttu-id="e2613-138">O fluxo de conteúdo para esta versão do item.</span><span class="sxs-lookup"><span data-stu-id="e2613-138">Indicates the size of the content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
