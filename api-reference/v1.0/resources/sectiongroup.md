---
title: Tipo de recurso sectionGroup
description: Um grupo de seção em um bloco de anotações do OneNote. Grupos de seção podem conter seções e grupos de seção.
localization_priority: Normal
ms.openlocfilehash: f204c5422eb5f0f2580bfbed82ed28306dd0618f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806304"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="2ef84-104">Tipo de recurso sectionGroup</span><span class="sxs-lookup"><span data-stu-id="2ef84-104">sectionGroup resource type</span></span>

<span data-ttu-id="2ef84-p102">Um grupo de seção em um bloco de anotações do OneNote. Grupos de seção podem conter seções e grupos de seção.</span><span class="sxs-lookup"><span data-stu-id="2ef84-p102">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ef84-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ef84-107">JSON representation</span></span>

<span data-ttu-id="2ef84-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ef84-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectionGroup"
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
## <a name="properties"></a><span data-ttu-id="2ef84-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ef84-109">Properties</span></span>
| <span data-ttu-id="2ef84-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ef84-110">Property</span></span>     | <span data-ttu-id="2ef84-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ef84-111">Type</span></span>   |<span data-ttu-id="2ef84-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ef84-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ef84-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="2ef84-113">createdBy</span></span>|[<span data-ttu-id="2ef84-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="2ef84-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="2ef84-p103">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ef84-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="2ef84-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ef84-117">createdDateTime</span></span>|<span data-ttu-id="2ef84-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ef84-118">DateTimeOffset</span></span>|<span data-ttu-id="2ef84-p104">A data e hora da criação do grupo de seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ef84-p104">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="2ef84-123">id</span><span class="sxs-lookup"><span data-stu-id="2ef84-123">id</span></span>|<span data-ttu-id="2ef84-124">String</span><span class="sxs-lookup"><span data-stu-id="2ef84-124">String</span></span>|<span data-ttu-id="2ef84-p105">O identificador exclusivo do grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ef84-p105">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="2ef84-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2ef84-127">lastModifiedBy</span></span>|[<span data-ttu-id="2ef84-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="2ef84-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="2ef84-p106">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ef84-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="2ef84-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ef84-131">lastModifiedDateTime</span></span>|<span data-ttu-id="2ef84-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ef84-132">DateTimeOffset</span></span>|<span data-ttu-id="2ef84-p107">A data e hora da última modificação do grupo de seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ef84-p107">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="2ef84-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2ef84-137">displayName</span></span>|<span data-ttu-id="2ef84-138">String</span><span class="sxs-lookup"><span data-stu-id="2ef84-138">String</span></span>|<span data-ttu-id="2ef84-139">O nome do grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="2ef84-139">The name of the section group.</span></span>|
|<span data-ttu-id="2ef84-140">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="2ef84-140">sectionGroupsUrl</span></span>|<span data-ttu-id="2ef84-141">String</span><span class="sxs-lookup"><span data-stu-id="2ef84-141">String</span></span>|<span data-ttu-id="2ef84-p108">A URL da propriedade de navegação `sectionGroups`, que retorna todos os grupos de seção no grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ef84-p108">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="2ef84-144">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="2ef84-144">sectionsUrl</span></span>|<span data-ttu-id="2ef84-145">String</span><span class="sxs-lookup"><span data-stu-id="2ef84-145">String</span></span>|<span data-ttu-id="2ef84-p109">A URL da propriedade de navegação `sections`, que retorna todas as seções no grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ef84-p109">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="2ef84-148">self</span><span class="sxs-lookup"><span data-stu-id="2ef84-148">self</span></span>|<span data-ttu-id="2ef84-149">String</span><span class="sxs-lookup"><span data-stu-id="2ef84-149">String</span></span>|<span data-ttu-id="2ef84-p110">O ponto de extremidade onde você pode obter detalhes sobre o grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ef84-p110">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ef84-152">Relações</span><span class="sxs-lookup"><span data-stu-id="2ef84-152">Relationships</span></span>
| <span data-ttu-id="2ef84-153">Relação</span><span class="sxs-lookup"><span data-stu-id="2ef84-153">Relationship</span></span> | <span data-ttu-id="2ef84-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ef84-154">Type</span></span>   |<span data-ttu-id="2ef84-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ef84-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ef84-156">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="2ef84-156">parentNotebook</span></span>|[<span data-ttu-id="2ef84-157">Notebook</span><span class="sxs-lookup"><span data-stu-id="2ef84-157">Notebook</span></span>](notebook.md)|<span data-ttu-id="2ef84-p111">O bloco de anotações que contém o grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ef84-p111">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="2ef84-160">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="2ef84-160">parentSectionGroup</span></span>|[<span data-ttu-id="2ef84-161">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="2ef84-161">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="2ef84-p112">O grupo de seção que contém o grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ef84-p112">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="2ef84-164">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="2ef84-164">sectionGroups</span></span>|<span data-ttu-id="2ef84-165">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="2ef84-165">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="2ef84-p113">Os grupos de seção na seção. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2ef84-p113">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="2ef84-169">sections</span><span class="sxs-lookup"><span data-stu-id="2ef84-169">sections</span></span>|<span data-ttu-id="2ef84-170">Coleção [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="2ef84-170">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="2ef84-p114">As seções no grupo de seção. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2ef84-p114">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="2ef84-174">Métodos</span><span class="sxs-lookup"><span data-stu-id="2ef84-174">Methods</span></span>

| <span data-ttu-id="2ef84-175">Método</span><span class="sxs-lookup"><span data-stu-id="2ef84-175">Method</span></span>           | <span data-ttu-id="2ef84-176">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2ef84-176">Return Type</span></span>    |<span data-ttu-id="2ef84-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ef84-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2ef84-178">Get section group</span><span class="sxs-lookup"><span data-stu-id="2ef84-178">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="2ef84-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="2ef84-179">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="2ef84-180">Leia as propriedades e as relações do grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="2ef84-180">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="2ef84-181">Criar grupo de seção</span><span class="sxs-lookup"><span data-stu-id="2ef84-181">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="2ef84-182">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="2ef84-182">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="2ef84-183">Crie um grupo de seção postando na coleção sectionGroups do grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="2ef84-183">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="2ef84-184">Listar grupos de seção</span><span class="sxs-lookup"><span data-stu-id="2ef84-184">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="2ef84-185">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="2ef84-185">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="2ef84-186">A coleção de grupos de seção no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="2ef84-186">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="2ef84-187">Criar seção</span><span class="sxs-lookup"><span data-stu-id="2ef84-187">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="2ef84-188">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="2ef84-188">OnenoteSection</span></span>](section.md)| <span data-ttu-id="2ef84-189">Crie uma seção postando na coleção sections do grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="2ef84-189">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="2ef84-190">Listar seções</span><span class="sxs-lookup"><span data-stu-id="2ef84-190">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="2ef84-191">Coleção [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="2ef84-191">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="2ef84-192">Obtenha uma coleção de seções no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="2ef84-192">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
