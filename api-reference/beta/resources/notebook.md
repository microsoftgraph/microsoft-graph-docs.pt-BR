---
title: Tipo de recurso notebook
description: Um bloco de anotações do OneNote.
author: Jewan-microsoft
ms.openlocfilehash: b6301e53d1cc616897055df0185601400f87de54
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362213"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="ccc3e-103">Tipo de recurso notebook</span><span class="sxs-lookup"><span data-stu-id="ccc3e-103">notebook resource type</span></span>

> <span data-ttu-id="ccc3e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ccc3e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ccc3e-106">Um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-106">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccc3e-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ccc3e-107">JSON representation</span></span>

<span data-ttu-id="ccc3e-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ccc3e-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
## <a name="properties"></a><span data-ttu-id="ccc3e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ccc3e-109">Properties</span></span>
| <span data-ttu-id="ccc3e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccc3e-110">Property</span></span>     | <span data-ttu-id="ccc3e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccc3e-111">Type</span></span>   |<span data-ttu-id="ccc3e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccc3e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ccc3e-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="ccc3e-113">createdBy</span></span>|[<span data-ttu-id="ccc3e-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="ccc3e-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="ccc3e-p102">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="ccc3e-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ccc3e-117">createdDateTime</span></span>|<span data-ttu-id="ccc3e-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccc3e-118">DateTimeOffset</span></span>|<span data-ttu-id="ccc3e-p103">A data e hora da criação do bloco de anotações. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-p103">The date and time when the notebook was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="ccc3e-123">id</span><span class="sxs-lookup"><span data-stu-id="ccc3e-123">id</span></span>|<span data-ttu-id="ccc3e-124">String</span><span class="sxs-lookup"><span data-stu-id="ccc3e-124">String</span></span>|<span data-ttu-id="ccc3e-p104">O identificador exclusivo do bloco de anotações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-p104">The unique identifier of the notebook. Read-only.</span></span>|
|<span data-ttu-id="ccc3e-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="ccc3e-127">isDefault</span></span>|<span data-ttu-id="ccc3e-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="ccc3e-128">Boolean</span></span>|<span data-ttu-id="ccc3e-p105">Indica se este é o bloco de anotações padrão do usuário. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-p105">Indicates whether this is the user's default notebook. Read-only.</span></span>|
|<span data-ttu-id="ccc3e-131">isShared</span><span class="sxs-lookup"><span data-stu-id="ccc3e-131">isShared</span></span>|<span data-ttu-id="ccc3e-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="ccc3e-132">Boolean</span></span>|<span data-ttu-id="ccc3e-p106">Indica se o bloco de anotações é compartilhado. Se for verdadeiro, o conteúdo do bloco de anotações poderá ser visto por pessoas que não sejam o proprietário. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-p106">Indicates whether the notebook is shared. If true, the contents of the notebook can be seen by people other than the owner. Read-only.</span></span>|
|<span data-ttu-id="ccc3e-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ccc3e-136">lastModifiedBy</span></span>|[<span data-ttu-id="ccc3e-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="ccc3e-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="ccc3e-p107">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="ccc3e-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ccc3e-140">lastModifiedDateTime</span></span>|<span data-ttu-id="ccc3e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccc3e-141">DateTimeOffset</span></span>|<span data-ttu-id="ccc3e-p108">A data e hora da última modificação do bloco de anotações. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-p108">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="ccc3e-146">links</span><span class="sxs-lookup"><span data-stu-id="ccc3e-146">links</span></span>|[<span data-ttu-id="ccc3e-147">NotebookLinks</span><span class="sxs-lookup"><span data-stu-id="ccc3e-147">NotebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="ccc3e-p109">Links para abrir o bloco de anotações. O link `oneNoteClientURL` abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado. O link `oneNoteWebURL` abre o bloco de anotações no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-p109">Links for opening the notebook. The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="ccc3e-151">displayName</span><span class="sxs-lookup"><span data-stu-id="ccc3e-151">displayName</span></span>|<span data-ttu-id="ccc3e-152">String</span><span class="sxs-lookup"><span data-stu-id="ccc3e-152">String</span></span>|<span data-ttu-id="ccc3e-153">O nome do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-153">The name of the notebook.</span></span>|
|<span data-ttu-id="ccc3e-154">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="ccc3e-154">sectionGroupsUrl</span></span>|<span data-ttu-id="ccc3e-155">String</span><span class="sxs-lookup"><span data-stu-id="ccc3e-155">String</span></span>|<span data-ttu-id="ccc3e-p110">A URL da propriedade de navegação `sectionGroups` que retorna todos os grupos de seção no bloco de anotações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-p110">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook. Read-only.</span></span>|
|<span data-ttu-id="ccc3e-158">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="ccc3e-158">sectionsUrl</span></span>|<span data-ttu-id="ccc3e-159">String</span><span class="sxs-lookup"><span data-stu-id="ccc3e-159">String</span></span>|<span data-ttu-id="ccc3e-p111">A URL da propriedade de navegação `sections` que retorna todas as seções no bloco de anotações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-p111">The URL for the `sections` navigation property, which returns all the sections in the notebook. Read-only.</span></span>|
|<span data-ttu-id="ccc3e-162">self</span><span class="sxs-lookup"><span data-stu-id="ccc3e-162">self</span></span>|<span data-ttu-id="ccc3e-163">String</span><span class="sxs-lookup"><span data-stu-id="ccc3e-163">String</span></span>|<span data-ttu-id="ccc3e-p112">O ponto de extremidade onde você pode obter detalhes sobre o bloco de anotações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-p112">The endpoint where you can get details about the notebook. Read-only.</span></span>|
|<span data-ttu-id="ccc3e-166">userRole</span><span class="sxs-lookup"><span data-stu-id="ccc3e-166">userRole</span></span>|<span data-ttu-id="ccc3e-167">String</span><span class="sxs-lookup"><span data-stu-id="ccc3e-167">String</span></span>|<span data-ttu-id="ccc3e-p113">Os valores possíveis são: `Owner`, `Contributor`, `Reader`, `None`. O proprietário representa o acesso no nível de proprietário ao bloco de anotações. O proprietário representa o acesso de leitura/gravação ao bloco de anotações. O leitor representa o acesso somente leitura ao bloco de anotações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-p113">Possible values are: `Owner`, `Contributor`, `Reader`, `None`. Owner represents owner-level access to the notebook. Contributor represents read/write access to the notebook. Reader represents read-only access to the notebook. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccc3e-173">Relações</span><span class="sxs-lookup"><span data-stu-id="ccc3e-173">Relationships</span></span>
| <span data-ttu-id="ccc3e-174">Relação</span><span class="sxs-lookup"><span data-stu-id="ccc3e-174">Relationship</span></span> | <span data-ttu-id="ccc3e-175">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccc3e-175">Type</span></span>   |<span data-ttu-id="ccc3e-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccc3e-176">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ccc3e-177">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="ccc3e-177">sectionGroups</span></span>|<span data-ttu-id="ccc3e-178">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="ccc3e-178">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="ccc3e-p114">Obtém os grupos de seção no bloco de anotações. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-p114">The section groups in the notebook. Read-only. Nullable.</span></span>|
|<span data-ttu-id="ccc3e-182">sections</span><span class="sxs-lookup"><span data-stu-id="ccc3e-182">sections</span></span>|<span data-ttu-id="ccc3e-183">Coleção [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="ccc3e-183">[Section](section.md) collection</span></span>|<span data-ttu-id="ccc3e-p115">As seções no bloco de anotações. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-p115">The sections in the notebook. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="ccc3e-187">Métodos</span><span class="sxs-lookup"><span data-stu-id="ccc3e-187">Methods</span></span>

| <span data-ttu-id="ccc3e-188">Método</span><span class="sxs-lookup"><span data-stu-id="ccc3e-188">Method</span></span>           | <span data-ttu-id="ccc3e-189">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ccc3e-189">Return Type</span></span>    |<span data-ttu-id="ccc3e-190">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccc3e-190">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ccc3e-191">Obter bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="ccc3e-191">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="ccc3e-192">Notebook</span><span class="sxs-lookup"><span data-stu-id="ccc3e-192">Notebook</span></span>](notebook.md) |<span data-ttu-id="ccc3e-193">Leia as propriedades e as relações do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-193">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="ccc3e-194">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="ccc3e-194">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="ccc3e-195">coleção [recentNotebook](recentnotebook.md)</span><span class="sxs-lookup"><span data-stu-id="ccc3e-195">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="ccc3e-196">Obtenha uma coleção de blocos de anotações acessados mais recentemente para o usuário.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-196">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="ccc3e-197">Criar grupo de seção</span><span class="sxs-lookup"><span data-stu-id="ccc3e-197">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="ccc3e-198">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="ccc3e-198">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="ccc3e-199">Crie um grupo de seção postando na coleção sectionGroups no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-199">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="ccc3e-200">Listar grupos de seção</span><span class="sxs-lookup"><span data-stu-id="ccc3e-200">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="ccc3e-201">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="ccc3e-201">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="ccc3e-202">Obtenha uma coleção de grupos de seção no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-202">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="ccc3e-203">Criar seção</span><span class="sxs-lookup"><span data-stu-id="ccc3e-203">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="ccc3e-204">Section</span><span class="sxs-lookup"><span data-stu-id="ccc3e-204">Section</span></span>](section.md)| <span data-ttu-id="ccc3e-205">Crie uma seção postando na coleção sections no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-205">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="ccc3e-206">Listar seções</span><span class="sxs-lookup"><span data-stu-id="ccc3e-206">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="ccc3e-207">Coleção [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="ccc3e-207">[Section](section.md) collection</span></span>| <span data-ttu-id="ccc3e-208">Obtenha uma coleção de seções no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-208">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="ccc3e-209">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="ccc3e-209">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="ccc3e-210">None</span><span class="sxs-lookup"><span data-stu-id="ccc3e-210">None</span></span> | <span data-ttu-id="ccc3e-211">Copia um bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="ccc3e-211">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
