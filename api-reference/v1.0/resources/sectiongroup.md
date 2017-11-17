# <a name="sectiongroup-resource-type"></a><span data-ttu-id="6f69c-101">Tipo de recurso sectionGroup</span><span class="sxs-lookup"><span data-stu-id="6f69c-101">sectionGroup resource type</span></span>

<span data-ttu-id="6f69c-p101">Um grupo de seção em um bloco de anotações do OneNote. Grupos de seção podem conter seções e grupos de seção.</span><span class="sxs-lookup"><span data-stu-id="6f69c-p101">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f69c-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f69c-104">JSON representation</span></span>

<span data-ttu-id="6f69c-105">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f69c-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectiongroup"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="6f69c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f69c-106">Properties</span></span>
| <span data-ttu-id="6f69c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f69c-107">Property</span></span>     | <span data-ttu-id="6f69c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f69c-108">Type</span></span>   |<span data-ttu-id="6f69c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f69c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f69c-110">createdBy</span><span class="sxs-lookup"><span data-stu-id="6f69c-110">createdBy</span></span>|[<span data-ttu-id="6f69c-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="6f69c-111">identitySet</span></span>](identityset.md)|<span data-ttu-id="6f69c-p102">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f69c-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="6f69c-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f69c-114">createdDateTime</span></span>|<span data-ttu-id="6f69c-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f69c-115">DateTimeOffset</span></span>|<span data-ttu-id="6f69c-p103">A data e hora da criação do grupo de seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f69c-p103">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="6f69c-120">id</span><span class="sxs-lookup"><span data-stu-id="6f69c-120">id</span></span>|<span data-ttu-id="6f69c-121">String</span><span class="sxs-lookup"><span data-stu-id="6f69c-121">String</span></span>|<span data-ttu-id="6f69c-p104">O identificador exclusivo do grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f69c-p104">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="6f69c-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6f69c-124">lastModifiedBy</span></span>|[<span data-ttu-id="6f69c-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="6f69c-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="6f69c-p105">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f69c-p105">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="6f69c-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f69c-128">lastModifiedDateTime</span></span>|<span data-ttu-id="6f69c-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f69c-129">DateTimeOffset</span></span>|<span data-ttu-id="6f69c-p106">A data e hora da última modificação do grupo de seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f69c-p106">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="6f69c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6f69c-134">displayName</span></span>|<span data-ttu-id="6f69c-135">String</span><span class="sxs-lookup"><span data-stu-id="6f69c-135">String</span></span>|<span data-ttu-id="6f69c-136">O nome do grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="6f69c-136">The name of the section group.</span></span>|
|<span data-ttu-id="6f69c-137">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="6f69c-137">sectionGroupsUrl</span></span>|<span data-ttu-id="6f69c-138">String</span><span class="sxs-lookup"><span data-stu-id="6f69c-138">String</span></span>|<span data-ttu-id="6f69c-p107">A URL da propriedade de navegação `sectionGroups`, que retorna todos os grupos de seção no grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f69c-p107">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="6f69c-141">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="6f69c-141">sectionsUrl</span></span>|<span data-ttu-id="6f69c-142">String</span><span class="sxs-lookup"><span data-stu-id="6f69c-142">String</span></span>|<span data-ttu-id="6f69c-p108">A URL da propriedade de navegação `sections`, que retorna todas as seções no grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f69c-p108">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="6f69c-145">self</span><span class="sxs-lookup"><span data-stu-id="6f69c-145">self</span></span>|<span data-ttu-id="6f69c-146">String</span><span class="sxs-lookup"><span data-stu-id="6f69c-146">String</span></span>|<span data-ttu-id="6f69c-p109">O ponto de extremidade onde você pode obter detalhes sobre o grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f69c-p109">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f69c-149">Relações</span><span class="sxs-lookup"><span data-stu-id="6f69c-149">Relationships</span></span>
| <span data-ttu-id="6f69c-150">Relação</span><span class="sxs-lookup"><span data-stu-id="6f69c-150">Relationship</span></span> | <span data-ttu-id="6f69c-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f69c-151">Type</span></span>   |<span data-ttu-id="6f69c-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f69c-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f69c-153">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="6f69c-153">parentNotebook</span></span>|[<span data-ttu-id="6f69c-154">Notebook</span><span class="sxs-lookup"><span data-stu-id="6f69c-154">Notebook</span></span>](notebook.md)|<span data-ttu-id="6f69c-p110">O bloco de anotações que contém o grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f69c-p110">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="6f69c-157">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="6f69c-157">parentSectionGroup</span></span>|[<span data-ttu-id="6f69c-158">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="6f69c-158">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="6f69c-p111">O grupo de seção que contém o grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f69c-p111">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="6f69c-161">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="6f69c-161">sectionGroups</span></span>|<span data-ttu-id="6f69c-162">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="6f69c-162">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="6f69c-p112">Os grupos de seção na seção. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="6f69c-p112">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6f69c-166">sections</span><span class="sxs-lookup"><span data-stu-id="6f69c-166">sections</span></span>|<span data-ttu-id="6f69c-167">Coleção [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="6f69c-167">[Section](section.md) collection</span></span>|<span data-ttu-id="6f69c-p113">As seções no grupo de seção. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="6f69c-p113">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="6f69c-171">Métodos</span><span class="sxs-lookup"><span data-stu-id="6f69c-171">Methods</span></span>

| <span data-ttu-id="6f69c-172">Método</span><span class="sxs-lookup"><span data-stu-id="6f69c-172">Method</span></span>           | <span data-ttu-id="6f69c-173">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6f69c-173">Return Type</span></span>    |<span data-ttu-id="6f69c-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f69c-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6f69c-175">Get section group</span><span class="sxs-lookup"><span data-stu-id="6f69c-175">Get section group</span></span>](../api/sectiongroup_get.md) | [<span data-ttu-id="6f69c-176">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="6f69c-176">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="6f69c-177">Leia as propriedades e as relações do grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="6f69c-177">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="6f69c-178">Criar grupo de seção</span><span class="sxs-lookup"><span data-stu-id="6f69c-178">Create section group</span></span>](../api/sectiongroup_post_sectiongroups.md) |[<span data-ttu-id="6f69c-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="6f69c-179">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="6f69c-180">Crie um grupo de seção postando na coleção sectionGroups do grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="6f69c-180">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="6f69c-181">Listar grupos de seção</span><span class="sxs-lookup"><span data-stu-id="6f69c-181">List section groups</span></span>](../api/sectiongroup_list_sectiongroups.md) |<span data-ttu-id="6f69c-182">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="6f69c-182">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="6f69c-183">A coleção de grupos de seção no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="6f69c-183">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="6f69c-184">Criar seção</span><span class="sxs-lookup"><span data-stu-id="6f69c-184">Create section</span></span>](../api/sectiongroup_post_sections.md) |[<span data-ttu-id="6f69c-185">Section</span><span class="sxs-lookup"><span data-stu-id="6f69c-185">Section</span></span>](section.md)| <span data-ttu-id="6f69c-186">Crie uma seção postando na coleção sections do grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="6f69c-186">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="6f69c-187">Listar seções</span><span class="sxs-lookup"><span data-stu-id="6f69c-187">List sections</span></span>](../api/sectiongroup_list_sections.md) |<span data-ttu-id="6f69c-188">Coleção [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="6f69c-188">[Section](section.md) collection</span></span>| <span data-ttu-id="6f69c-189">Obtenha uma coleção de seções no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="6f69c-189">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
