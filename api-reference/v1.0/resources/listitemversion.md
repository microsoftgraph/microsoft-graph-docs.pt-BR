# <a name="listitemversion-resource-type"></a><span data-ttu-id="4eb39-101">Tipo de recurso ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="4eb39-101">ListItemVersion resource type</span></span>

<span data-ttu-id="4eb39-102">O recurso **listItemVersion** representa uma versão anterior de um recurso [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="4eb39-102">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="4eb39-103">Tarefas em recursos ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="4eb39-103">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="4eb39-104">As seguintes tarefas estão disponíveis para os recursos listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="4eb39-104">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="4eb39-105">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="4eb39-105">Common task</span></span>             |         <span data-ttu-id="4eb39-106">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="4eb39-106">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="4eb39-107">[Versões de lista][version-list]</span><span class="sxs-lookup"><span data-stu-id="4eb39-107">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="4eb39-108">[Obter versão][version-get]</span><span class="sxs-lookup"><span data-stu-id="4eb39-108">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="4eb39-109">[Restaurar versão][version-restore]</span><span class="sxs-lookup"><span data-stu-id="4eb39-109">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem_list_versions.md
[version-get]: ../api/listitemversion_get.md
[version-restore]: ../api/listitemversion_restore.md


## <a name="json-representation"></a><span data-ttu-id="4eb39-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4eb39-110">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.listItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "published": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="4eb39-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4eb39-111">Properties</span></span>

|      <span data-ttu-id="4eb39-112">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="4eb39-112">Property name</span></span>       |                         <span data-ttu-id="4eb39-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="4eb39-113">Type</span></span>                         |                               <span data-ttu-id="4eb39-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="4eb39-114">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="4eb39-115">**id**</span><span class="sxs-lookup"><span data-stu-id="4eb39-115">**id**</span></span>                   | <span data-ttu-id="4eb39-116">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="4eb39-116">string</span></span>                                               | <span data-ttu-id="4eb39-117">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="4eb39-117">The ID of the version.</span></span> <span data-ttu-id="4eb39-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4eb39-118">Read-only.</span></span>                                       |
| <span data-ttu-id="4eb39-119">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="4eb39-119">**lastModifiedBy**</span></span>       | [<span data-ttu-id="4eb39-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="4eb39-120">IdentitySet</span></span>](../resources/identitySet.md)           | <span data-ttu-id="4eb39-121">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4eb39-121">Identity of the user which last modified the version.</span></span> <span data-ttu-id="4eb39-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4eb39-122">Read-only.</span></span>        |
| <span data-ttu-id="4eb39-123">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="4eb39-123">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="4eb39-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eb39-124">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="4eb39-125">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4eb39-125">Date and time the version was last modified.</span></span> <span data-ttu-id="4eb39-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4eb39-126">Read-only.</span></span>                 |
| <span data-ttu-id="4eb39-127">**published**</span><span class="sxs-lookup"><span data-stu-id="4eb39-127">**published**</span></span>            | [<span data-ttu-id="4eb39-128">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="4eb39-128">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="4eb39-129">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="4eb39-129">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="4eb39-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4eb39-130">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="4eb39-131">Relações</span><span class="sxs-lookup"><span data-stu-id="4eb39-131">Relationships</span></span>

<span data-ttu-id="4eb39-132">A tabela a seguir define as relações que o recurso **driveItemVersion** tem com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="4eb39-132">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="4eb39-133">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="4eb39-133">Relationship name</span></span> |                      <span data-ttu-id="4eb39-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="4eb39-134">Type</span></span>                      |                               <span data-ttu-id="4eb39-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="4eb39-135">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="4eb39-136">**fields**</span><span class="sxs-lookup"><span data-stu-id="4eb39-136">**fields**</span></span>        | [<span data-ttu-id="4eb39-137">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="4eb39-137">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="4eb39-138">Uma coleção de campos e valores para esta versão do item da lista.</span><span class="sxs-lookup"><span data-stu-id="4eb39-138">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
