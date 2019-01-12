---
title: Tipo de recurso notebook
description: Um bloco de anotações do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: ed2d37de2dded71053f44bbcdd9de2b82505efc5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978799"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="6d395-103">Tipo de recurso notebook</span><span class="sxs-lookup"><span data-stu-id="6d395-103">notebook resource type</span></span>

<span data-ttu-id="6d395-104">Um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="6d395-104">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d395-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d395-105">JSON representation</span></span>

<span data-ttu-id="6d395-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6d395-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.notebook"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "isShared": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.notebookLinks"},
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string",
  "userRole": "String"
}

```
## <a name="properties"></a><span data-ttu-id="6d395-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d395-107">Properties</span></span>
| <span data-ttu-id="6d395-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d395-108">Property</span></span>     | <span data-ttu-id="6d395-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d395-109">Type</span></span>   |<span data-ttu-id="6d395-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d395-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d395-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="6d395-111">createdBy</span></span>|[<span data-ttu-id="6d395-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="6d395-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="6d395-p101">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d395-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="6d395-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d395-115">createdDateTime</span></span>|<span data-ttu-id="6d395-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d395-116">DateTimeOffset</span></span>|<span data-ttu-id="6d395-p102">A data e hora da criação do bloco de anotações. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d395-p102">The date and time when the notebook was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="6d395-121">id</span><span class="sxs-lookup"><span data-stu-id="6d395-121">id</span></span>|<span data-ttu-id="6d395-122">String</span><span class="sxs-lookup"><span data-stu-id="6d395-122">String</span></span>|<span data-ttu-id="6d395-p103">O identificador exclusivo do bloco de anotações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d395-p103">The unique identifier of the notebook. Read-only.</span></span>|
|<span data-ttu-id="6d395-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="6d395-125">isDefault</span></span>|<span data-ttu-id="6d395-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="6d395-126">Boolean</span></span>|<span data-ttu-id="6d395-p104">Indica se este é o bloco de anotações padrão do usuário. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d395-p104">Indicates whether this is the user's default notebook. Read-only.</span></span>|
|<span data-ttu-id="6d395-129">isShared</span><span class="sxs-lookup"><span data-stu-id="6d395-129">isShared</span></span>|<span data-ttu-id="6d395-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="6d395-130">Boolean</span></span>|<span data-ttu-id="6d395-p105">Indica se o bloco de anotações é compartilhado. Se for verdadeiro, o conteúdo do bloco de anotações poderá ser visto por pessoas que não sejam o proprietário. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d395-p105">Indicates whether the notebook is shared. If true, the contents of the notebook can be seen by people other than the owner. Read-only.</span></span>|
|<span data-ttu-id="6d395-134">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6d395-134">lastModifiedBy</span></span>|[<span data-ttu-id="6d395-135">identitySet</span><span class="sxs-lookup"><span data-stu-id="6d395-135">identitySet</span></span>](identityset.md)|<span data-ttu-id="6d395-p106">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d395-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="6d395-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d395-138">lastModifiedDateTime</span></span>|<span data-ttu-id="6d395-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d395-139">DateTimeOffset</span></span>|<span data-ttu-id="6d395-p107">A data e hora da última modificação do bloco de anotações. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d395-p107">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="6d395-144">links</span><span class="sxs-lookup"><span data-stu-id="6d395-144">links</span></span>|[<span data-ttu-id="6d395-145">NotebookLinks</span><span class="sxs-lookup"><span data-stu-id="6d395-145">NotebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="6d395-p108">Links para abrir o bloco de anotações. O link `oneNoteClientURL` abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado. O link `oneNoteWebURL` abre o bloco de anotações no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="6d395-p108">Links for opening the notebook. The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="6d395-149">displayName</span><span class="sxs-lookup"><span data-stu-id="6d395-149">displayName</span></span>|<span data-ttu-id="6d395-150">String</span><span class="sxs-lookup"><span data-stu-id="6d395-150">String</span></span>|<span data-ttu-id="6d395-151">O nome do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="6d395-151">The name of the notebook.</span></span>|
|<span data-ttu-id="6d395-152">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="6d395-152">sectionGroupsUrl</span></span>|<span data-ttu-id="6d395-153">String</span><span class="sxs-lookup"><span data-stu-id="6d395-153">String</span></span>|<span data-ttu-id="6d395-p109">A URL da propriedade de navegação `sectionGroups` que retorna todos os grupos de seção no bloco de anotações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d395-p109">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook. Read-only.</span></span>|
|<span data-ttu-id="6d395-156">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="6d395-156">sectionsUrl</span></span>|<span data-ttu-id="6d395-157">String</span><span class="sxs-lookup"><span data-stu-id="6d395-157">String</span></span>|<span data-ttu-id="6d395-p110">A URL da propriedade de navegação `sections` que retorna todas as seções no bloco de anotações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d395-p110">The URL for the `sections` navigation property, which returns all the sections in the notebook. Read-only.</span></span>|
|<span data-ttu-id="6d395-160">self</span><span class="sxs-lookup"><span data-stu-id="6d395-160">self</span></span>|<span data-ttu-id="6d395-161">String</span><span class="sxs-lookup"><span data-stu-id="6d395-161">String</span></span>|<span data-ttu-id="6d395-p111">O ponto de extremidade onde você pode obter detalhes sobre o bloco de anotações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d395-p111">The endpoint where you can get details about the notebook. Read-only.</span></span>|
|<span data-ttu-id="6d395-164">userRole</span><span class="sxs-lookup"><span data-stu-id="6d395-164">userRole</span></span>|<span data-ttu-id="6d395-165">onenoteUserRole</span><span class="sxs-lookup"><span data-stu-id="6d395-165">onenoteUserRole</span></span>|<span data-ttu-id="6d395-p112">Os valores possíveis são: `Owner`, `Contributor`, `Reader`, `None`. O proprietário representa o acesso no nível de proprietário ao bloco de anotações. O proprietário representa o acesso de leitura/gravação ao bloco de anotações. O leitor representa o acesso somente leitura ao bloco de anotações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d395-p112">Possible values are: `Owner`, `Contributor`, `Reader`, `None`. Owner represents owner-level access to the notebook. Contributor represents read/write access to the notebook. Reader represents read-only access to the notebook. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d395-171">Relações</span><span class="sxs-lookup"><span data-stu-id="6d395-171">Relationships</span></span>
| <span data-ttu-id="6d395-172">Relação</span><span class="sxs-lookup"><span data-stu-id="6d395-172">Relationship</span></span> | <span data-ttu-id="6d395-173">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d395-173">Type</span></span>   |<span data-ttu-id="6d395-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d395-174">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d395-175">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="6d395-175">sectionGroups</span></span>|<span data-ttu-id="6d395-176">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="6d395-176">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="6d395-p113">Obtém os grupos de seção no bloco de anotações. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="6d395-p113">The section groups in the notebook. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6d395-180">sections</span><span class="sxs-lookup"><span data-stu-id="6d395-180">sections</span></span>|<span data-ttu-id="6d395-181">Coleção [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="6d395-181">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="6d395-p114">As seções no bloco de anotações. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="6d395-p114">The sections in the notebook. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="6d395-185">Métodos</span><span class="sxs-lookup"><span data-stu-id="6d395-185">Methods</span></span>

| <span data-ttu-id="6d395-186">Método</span><span class="sxs-lookup"><span data-stu-id="6d395-186">Method</span></span>           | <span data-ttu-id="6d395-187">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6d395-187">Return Type</span></span>    |<span data-ttu-id="6d395-188">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d395-188">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6d395-189">Obter bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="6d395-189">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="6d395-190">Notebook</span><span class="sxs-lookup"><span data-stu-id="6d395-190">Notebook</span></span>](notebook.md) |<span data-ttu-id="6d395-191">Leia as propriedades e as relações do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="6d395-191">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="6d395-192">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="6d395-192">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="6d395-193">coleção [recentNotebook](recentnotebook.md)</span><span class="sxs-lookup"><span data-stu-id="6d395-193">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="6d395-194">Obtenha uma coleção de blocos de anotações acessados mais recentemente para o usuário.</span><span class="sxs-lookup"><span data-stu-id="6d395-194">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="6d395-195">Criar grupo de seção</span><span class="sxs-lookup"><span data-stu-id="6d395-195">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="6d395-196">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="6d395-196">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="6d395-197">Crie um grupo de seção postando na coleção sectionGroups no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="6d395-197">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="6d395-198">Listar grupos de seção</span><span class="sxs-lookup"><span data-stu-id="6d395-198">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="6d395-199">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="6d395-199">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="6d395-200">Obtenha uma coleção de grupos de seção no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="6d395-200">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="6d395-201">Criar seção</span><span class="sxs-lookup"><span data-stu-id="6d395-201">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="6d395-202">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="6d395-202">OnenoteSection</span></span>](section.md)| <span data-ttu-id="6d395-203">Crie uma seção postando na coleção sections no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="6d395-203">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="6d395-204">Listar seções</span><span class="sxs-lookup"><span data-stu-id="6d395-204">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="6d395-205">Coleção [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="6d395-205">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="6d395-206">Obtenha uma coleção de seções no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="6d395-206">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="6d395-207">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="6d395-207">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="6d395-208">None</span><span class="sxs-lookup"><span data-stu-id="6d395-208">None</span></span> | <span data-ttu-id="6d395-209">Copia um bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="6d395-209">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
