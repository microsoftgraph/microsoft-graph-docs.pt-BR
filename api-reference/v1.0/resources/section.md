# <a name="section-resource-type"></a><span data-ttu-id="d8a4c-101">Tipo de recurso section</span><span class="sxs-lookup"><span data-stu-id="d8a4c-101">section resource type</span></span>

<span data-ttu-id="d8a4c-p101">Uma seção em um bloco de anotações do OneNote. As seções podem conter páginas.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-p101">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8a4c-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8a4c-104">JSON representation</span></span>

<span data-ttu-id="d8a4c-105">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "@odata.type": "microsoft.graph.onenoteSection"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.sectionLinks"},
  "displayName": "string",
  "pagesUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="d8a4c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8a4c-106">Properties</span></span>
| <span data-ttu-id="d8a4c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8a4c-107">Property</span></span>     | <span data-ttu-id="d8a4c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8a4c-108">Type</span></span>   |<span data-ttu-id="d8a4c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8a4c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8a4c-110">createdBy</span><span class="sxs-lookup"><span data-stu-id="d8a4c-110">createdBy</span></span>|[<span data-ttu-id="d8a4c-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="d8a4c-111">identitySet</span></span>](identityset.md)|<span data-ttu-id="d8a4c-p102">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="d8a4c-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8a4c-114">createdDateTime</span></span>|<span data-ttu-id="d8a4c-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8a4c-115">DateTimeOffset</span></span>|<span data-ttu-id="d8a4c-p103">A data e hora da criação da seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-p103">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="d8a4c-120">id</span><span class="sxs-lookup"><span data-stu-id="d8a4c-120">id</span></span>|<span data-ttu-id="d8a4c-121">String</span><span class="sxs-lookup"><span data-stu-id="d8a4c-121">String</span></span>|<span data-ttu-id="d8a4c-p104">O identificador exclusivo da seção.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-p104">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="d8a4c-124">isDefault</span><span class="sxs-lookup"><span data-stu-id="d8a4c-124">isDefault</span></span>|<span data-ttu-id="d8a4c-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a4c-125">Boolean</span></span>|<span data-ttu-id="d8a4c-p105">Indica se esta é a seção padrão do usuário. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-p105">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="d8a4c-128">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d8a4c-128">lastModifiedBy</span></span>|[<span data-ttu-id="d8a4c-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="d8a4c-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="d8a4c-p106">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="d8a4c-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8a4c-132">lastModifiedDateTime</span></span>|<span data-ttu-id="d8a4c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8a4c-133">DateTimeOffset</span></span>|<span data-ttu-id="d8a4c-p107">A data e hora da última modificação da seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-p107">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="d8a4c-138">links</span><span class="sxs-lookup"><span data-stu-id="d8a4c-138">links</span></span>|[<span data-ttu-id="d8a4c-139">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="d8a4c-139">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="d8a4c-p108">Links para abrir a seção. O link `oneNoteClientURL` abre a seção no cliente nativo do OneNote se ele estiver instalado. O link `oneNoteWebURL` abre a seção no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-p108">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="d8a4c-143">displayName</span><span class="sxs-lookup"><span data-stu-id="d8a4c-143">displayName</span></span>|<span data-ttu-id="d8a4c-144">String</span><span class="sxs-lookup"><span data-stu-id="d8a4c-144">String</span></span>|<span data-ttu-id="d8a4c-145">O nome da seção.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-145">The name of the section.</span></span> |
|<span data-ttu-id="d8a4c-146">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="d8a4c-146">pagesUrl</span></span>|<span data-ttu-id="d8a4c-147">String</span><span class="sxs-lookup"><span data-stu-id="d8a4c-147">String</span></span>|<span data-ttu-id="d8a4c-p109">O ponto de extremidade `pages` onde você pode obter detalhes de todas as páginas na seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-p109">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="d8a4c-150">self</span><span class="sxs-lookup"><span data-stu-id="d8a4c-150">self</span></span>|<span data-ttu-id="d8a4c-151">String</span><span class="sxs-lookup"><span data-stu-id="d8a4c-151">String</span></span>|<span data-ttu-id="d8a4c-p110">O ponto de extremidade onde você pode obter detalhes sobre a seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-p110">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8a4c-154">Relações</span><span class="sxs-lookup"><span data-stu-id="d8a4c-154">Relationships</span></span>
| <span data-ttu-id="d8a4c-155">Relação</span><span class="sxs-lookup"><span data-stu-id="d8a4c-155">Relationship</span></span> | <span data-ttu-id="d8a4c-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8a4c-156">Type</span></span>   |<span data-ttu-id="d8a4c-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8a4c-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8a4c-158">páginas</span><span class="sxs-lookup"><span data-stu-id="d8a4c-158">pages</span></span>|<span data-ttu-id="d8a4c-159">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="d8a4c-159">[Page](page.md) collection</span></span>|<span data-ttu-id="d8a4c-p111">Obtém o conjunto de páginas da seção.  Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-p111">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="d8a4c-163">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="d8a4c-163">parentNotebook</span></span>|[<span data-ttu-id="d8a4c-164">Notebook</span><span class="sxs-lookup"><span data-stu-id="d8a4c-164">Notebook</span></span>](notebook.md)|<span data-ttu-id="d8a4c-p112">O bloco de anotações que contém a seção.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-p112">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="d8a4c-167">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="d8a4c-167">parentSectionGroup</span></span>|[<span data-ttu-id="d8a4c-168">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="d8a4c-168">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="d8a4c-p113">O grupo de seção que contém a seção.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-p113">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="d8a4c-171">Métodos</span><span class="sxs-lookup"><span data-stu-id="d8a4c-171">Methods</span></span>

| <span data-ttu-id="d8a4c-172">Método</span><span class="sxs-lookup"><span data-stu-id="d8a4c-172">Method</span></span>           | <span data-ttu-id="d8a4c-173">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d8a4c-173">Return Type</span></span>    |<span data-ttu-id="d8a4c-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8a4c-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8a4c-175">Get section</span><span class="sxs-lookup"><span data-stu-id="d8a4c-175">Get section</span></span>](../api/section_get.md) | [<span data-ttu-id="d8a4c-176">Section</span><span class="sxs-lookup"><span data-stu-id="d8a4c-176">Section</span></span>](section.md) |<span data-ttu-id="d8a4c-177">Leia as propriedades e as relações da seção.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-177">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="d8a4c-178">Criar página</span><span class="sxs-lookup"><span data-stu-id="d8a4c-178">Create page</span></span>](../api/section_post_pages.md) |[<span data-ttu-id="d8a4c-179">Página</span><span class="sxs-lookup"><span data-stu-id="d8a4c-179">Page</span></span>](page.md)| <span data-ttu-id="d8a4c-180">Crie uma página postando na coleção pages do grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-180">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="d8a4c-181">Listar páginas</span><span class="sxs-lookup"><span data-stu-id="d8a4c-181">List pages</span></span>](../api/section_list_pages.md) |<span data-ttu-id="d8a4c-182">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="d8a4c-182">[Page](page.md) collection</span></span>| <span data-ttu-id="d8a4c-183">Obtém uma coleção de páginas na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-183">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="d8a4c-184">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="d8a4c-184">copyToNotebook</span></span>](../api/section_copytonotebook.md)|<span data-ttu-id="d8a4c-185">None</span><span class="sxs-lookup"><span data-stu-id="d8a4c-185">None</span></span>|<span data-ttu-id="d8a4c-186">Copia a seção para um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-186">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="d8a4c-187">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="d8a4c-187">copyToSectionGroup</span></span>](../api/section_copytosectiongroup.md)|<span data-ttu-id="d8a4c-188">None</span><span class="sxs-lookup"><span data-stu-id="d8a4c-188">None</span></span>|<span data-ttu-id="d8a4c-189">Copia uma seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="d8a4c-189">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
