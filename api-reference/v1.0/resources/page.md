# <a name="page-resource-type"></a><span data-ttu-id="4a39c-101">Tipo de recurso page</span><span class="sxs-lookup"><span data-stu-id="4a39c-101">page resource type</span></span>

<span data-ttu-id="4a39c-102">Uma página em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="4a39c-102">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a39c-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a39c-103">JSON representation</span></span>

<span data-ttu-id="4a39c-104">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a39c-104">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenotePage"
}-->

```json
{
  "content": "stream",
  "contentUrl": "string",
  "createdByAppId": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "level": 1024,
  "links": {"@odata.type": "microsoft.graph.pageLinks"},
  "order": 1024,
  "self": "string",
  "title": "string"
}

```
## <a name="properties"></a><span data-ttu-id="4a39c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a39c-105">Properties</span></span>
| <span data-ttu-id="4a39c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a39c-106">Property</span></span>     | <span data-ttu-id="4a39c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a39c-107">Type</span></span>   |<span data-ttu-id="4a39c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a39c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a39c-109">content</span><span class="sxs-lookup"><span data-stu-id="4a39c-109">content</span></span>|<span data-ttu-id="4a39c-110">Fluxo</span><span class="sxs-lookup"><span data-stu-id="4a39c-110">Stream</span></span>|<span data-ttu-id="4a39c-111">O conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="4a39c-111">The page's HTML content.</span></span>|
|<span data-ttu-id="4a39c-112">contentUrl</span><span class="sxs-lookup"><span data-stu-id="4a39c-112">contentUrl</span></span>|<span data-ttu-id="4a39c-113">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a39c-113">String</span></span>|<span data-ttu-id="4a39c-p101">A URL do conteúdo HTML da página.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a39c-p101">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="4a39c-116">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="4a39c-116">createdByAppId</span></span>|<span data-ttu-id="4a39c-117">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a39c-117">String</span></span>|<span data-ttu-id="4a39c-p102">O identificador exclusivo do aplicativo que criou a página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a39c-p102">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="4a39c-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a39c-120">createdDateTime</span></span>|<span data-ttu-id="4a39c-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a39c-121">DateTimeOffset</span></span>|<span data-ttu-id="4a39c-p103">A data e a hora da criação da página. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a39c-p103">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="4a39c-126">id</span><span class="sxs-lookup"><span data-stu-id="4a39c-126">id</span></span>|<span data-ttu-id="4a39c-127">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a39c-127">String</span></span>|<span data-ttu-id="4a39c-p104">O identificador exclusivo da página.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a39c-p104">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="4a39c-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a39c-130">lastModifiedDateTime</span></span>|<span data-ttu-id="4a39c-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a39c-131">DateTimeOffset</span></span>|<span data-ttu-id="4a39c-p105">A data e a hora da última modificação da página. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a39c-p105">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="4a39c-136">nível</span><span class="sxs-lookup"><span data-stu-id="4a39c-136">level</span></span>|<span data-ttu-id="4a39c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4a39c-137">Int32</span></span>|<span data-ttu-id="4a39c-p106">O nível de recuo da página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a39c-p106">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="4a39c-140">links</span><span class="sxs-lookup"><span data-stu-id="4a39c-140">links</span></span>|[<span data-ttu-id="4a39c-141">PageLinks</span><span class="sxs-lookup"><span data-stu-id="4a39c-141">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="4a39c-p107">Links para abrir a página. O link `oneNoteClientURL` abre a página no cliente nativo do OneNote se ele estiver instalado. O link `oneNoteWebUrl` abre a página no OneNote Online. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a39c-p107">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="4a39c-146">ordem</span><span class="sxs-lookup"><span data-stu-id="4a39c-146">order</span></span>|<span data-ttu-id="4a39c-147">Int32</span><span class="sxs-lookup"><span data-stu-id="4a39c-147">Int32</span></span>|<span data-ttu-id="4a39c-p108">A ordem da página dentro da seção pai dela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a39c-p108">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="4a39c-150">self</span><span class="sxs-lookup"><span data-stu-id="4a39c-150">self</span></span>|<span data-ttu-id="4a39c-151">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a39c-151">String</span></span>|<span data-ttu-id="4a39c-p109">O ponto de extremidade onde você pode obter detalhes sobre a página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a39c-p109">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="4a39c-154">title</span><span class="sxs-lookup"><span data-stu-id="4a39c-154">title</span></span>|<span data-ttu-id="4a39c-155">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a39c-155">String</span></span>|<span data-ttu-id="4a39c-156">O título da página.</span><span class="sxs-lookup"><span data-stu-id="4a39c-156">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4a39c-157">Relações</span><span class="sxs-lookup"><span data-stu-id="4a39c-157">Relationships</span></span>
| <span data-ttu-id="4a39c-158">Relação</span><span class="sxs-lookup"><span data-stu-id="4a39c-158">Relationship</span></span> | <span data-ttu-id="4a39c-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a39c-159">Type</span></span>   |<span data-ttu-id="4a39c-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a39c-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a39c-161">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="4a39c-161">parentNotebook</span></span>|[<span data-ttu-id="4a39c-162">Bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="4a39c-162">Notebook</span></span>](notebook.md)|<span data-ttu-id="4a39c-p110">O bloco de anotações que contém a página.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a39c-p110">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="4a39c-165">parentSection</span><span class="sxs-lookup"><span data-stu-id="4a39c-165">parentSection</span></span>|[<span data-ttu-id="4a39c-166">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="4a39c-166">OnenoteSection</span></span>](section.md)|<span data-ttu-id="4a39c-p111">A seção que contém a página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a39c-p111">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="4a39c-169">Métodos</span><span class="sxs-lookup"><span data-stu-id="4a39c-169">Methods</span></span>

| <span data-ttu-id="4a39c-170">Método</span><span class="sxs-lookup"><span data-stu-id="4a39c-170">Method</span></span>           | <span data-ttu-id="4a39c-171">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4a39c-171">Return Type</span></span>    |<span data-ttu-id="4a39c-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a39c-172">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4a39c-173">Get page</span><span class="sxs-lookup"><span data-stu-id="4a39c-173">Get page</span></span>](../api/page_get.md) | [<span data-ttu-id="4a39c-174">Página</span><span class="sxs-lookup"><span data-stu-id="4a39c-174">Page</span></span>](page.md) |<span data-ttu-id="4a39c-175">Leia as propriedades e as relações da página.</span><span class="sxs-lookup"><span data-stu-id="4a39c-175">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="4a39c-176">Atualizar o conteúdo da página</span><span class="sxs-lookup"><span data-stu-id="4a39c-176">Update page content</span></span>](../api/page_update.md) | <span data-ttu-id="4a39c-177">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a39c-177">None</span></span> |<span data-ttu-id="4a39c-178">Atualizar o conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="4a39c-178">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="4a39c-179">Excluir página</span><span class="sxs-lookup"><span data-stu-id="4a39c-179">Delete page</span></span>](../api/page_delete.md) | <span data-ttu-id="4a39c-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a39c-180">None</span></span> |<span data-ttu-id="4a39c-181">Exclua a página.</span><span class="sxs-lookup"><span data-stu-id="4a39c-181">Delete the page.</span></span> |
|[<span data-ttu-id="4a39c-182">copyToSection</span><span class="sxs-lookup"><span data-stu-id="4a39c-182">copyToSection</span></span>](../api/page_copytosection.md)| <span data-ttu-id="4a39c-183">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a39c-183">None</span></span> |<span data-ttu-id="4a39c-184">Copia a página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="4a39c-184">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->