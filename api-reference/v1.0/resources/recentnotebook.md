# <a name="recentnotebook-resource-type"></a><span data-ttu-id="7333c-101">tipo de recurso recentNotebook</span><span class="sxs-lookup"><span data-stu-id="7333c-101">recentNotebook resource type</span></span>

<span data-ttu-id="7333c-102">Um bloco de notas do OneNote recentemente acessado.</span><span class="sxs-lookup"><span data-stu-id="7333c-102">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="7333c-103">Um **recentNotebook** é similar a um [notebook](notebook.md), mas tem menos propriedades.</span><span class="sxs-lookup"><span data-stu-id="7333c-103">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="7333c-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7333c-104">Properties</span></span>
| <span data-ttu-id="7333c-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7333c-105">Property</span></span>     | <span data-ttu-id="7333c-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="7333c-106">Type</span></span>   |<span data-ttu-id="7333c-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="7333c-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7333c-108">displayName</span><span class="sxs-lookup"><span data-stu-id="7333c-108">displayName</span></span>|<span data-ttu-id="7333c-109">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="7333c-109">String</span></span>|<span data-ttu-id="7333c-110">O nome do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="7333c-110">The name of the notebook.</span></span>|
|<span data-ttu-id="7333c-111">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="7333c-111">lastAccessedTime</span></span>|<span data-ttu-id="7333c-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7333c-112">DateTimeOffset</span></span>|<span data-ttu-id="7333c-p102">A data e hora da última modificação do bloco de anotações. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7333c-p102">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="7333c-117">links</span><span class="sxs-lookup"><span data-stu-id="7333c-117">links</span></span>|[<span data-ttu-id="7333c-118">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="7333c-118">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="7333c-119">Links para abrir o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="7333c-119">Links for opening the notebook.</span></span> <span data-ttu-id="7333c-120">O link `oneNoteClientURL` abre o bloco de anotações no cliente do OneNote quando ele está instalado.</span><span class="sxs-lookup"><span data-stu-id="7333c-120">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="7333c-121">O link `oneNoteWebURL` abre o bloco de anotações no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="7333c-121">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="7333c-122">sourceService</span><span class="sxs-lookup"><span data-stu-id="7333c-122">sourceService</span></span>|<span data-ttu-id="7333c-123">onenoteSourceService</span><span class="sxs-lookup"><span data-stu-id="7333c-123">onenoteSourceService values</span></span>|<span data-ttu-id="7333c-124">A loja de back-end onde o bloco de anotações (notebook) reside, tanto em `OneDriveForBusiness` ou em `OneDrive`.</span><span class="sxs-lookup"><span data-stu-id="7333c-124">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7333c-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7333c-125">JSON representation</span></span>

<span data-ttu-id="7333c-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7333c-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebook"
}-->

```json
{
  "displayName": "String",
  "lastAccessedTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.recentNotebookLinks"},
  "sourceService": "String"
}
```

## <a name="methods"></a><span data-ttu-id="7333c-127">Métodos</span><span class="sxs-lookup"><span data-stu-id="7333c-127">Methods</span></span>

| <span data-ttu-id="7333c-128">Método</span><span class="sxs-lookup"><span data-stu-id="7333c-128">Method</span></span>           | <span data-ttu-id="7333c-129">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7333c-129">Return Type</span></span>    |<span data-ttu-id="7333c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7333c-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7333c-131">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="7333c-131">getRecentNotebooks</span></span>](../api/notebook_getrecentnotebooks.md) | <span data-ttu-id="7333c-132">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="7333c-132">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="7333c-133">Obtenha uma coleção de blocos de anotações acessados mais recentemente para o usuário.</span><span class="sxs-lookup"><span data-stu-id="7333c-133">Get a collection of the most recently accessed notebooks for the user.</span></span> |
