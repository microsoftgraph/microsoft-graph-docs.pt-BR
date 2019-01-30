---
title: Tipo de recurso section
description: Uma seção em um bloco de anotações do OneNote. As seções podem conter páginas.
localization_priority: Normal
ms.openlocfilehash: faecf31ad09f3ea3b5614480fc051ad1054d442b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642601"
---
# <a name="section-resource-type"></a><span data-ttu-id="2b297-104">Tipo de recurso section</span><span class="sxs-lookup"><span data-stu-id="2b297-104">section resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b297-p102">Uma seção em um bloco de anotações do OneNote. As seções podem conter páginas.</span><span class="sxs-lookup"><span data-stu-id="2b297-p102">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b297-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b297-107">JSON representation</span></span>

<span data-ttu-id="2b297-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b297-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="2b297-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b297-109">Properties</span></span>
| <span data-ttu-id="2b297-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b297-110">Property</span></span>     | <span data-ttu-id="2b297-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b297-111">Type</span></span>   |<span data-ttu-id="2b297-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b297-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b297-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="2b297-113">createdBy</span></span>|[<span data-ttu-id="2b297-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="2b297-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="2b297-p103">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b297-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="2b297-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b297-117">createdDateTime</span></span>|<span data-ttu-id="2b297-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b297-118">DateTimeOffset</span></span>|<span data-ttu-id="2b297-p104">A data e hora da criação da seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b297-p104">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="2b297-123">id</span><span class="sxs-lookup"><span data-stu-id="2b297-123">id</span></span>|<span data-ttu-id="2b297-124">String</span><span class="sxs-lookup"><span data-stu-id="2b297-124">String</span></span>|<span data-ttu-id="2b297-p105">O identificador exclusivo da seção.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b297-p105">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="2b297-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="2b297-127">isDefault</span></span>|<span data-ttu-id="2b297-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="2b297-128">Boolean</span></span>|<span data-ttu-id="2b297-p106">Indica se esta é a seção padrão do usuário. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b297-p106">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="2b297-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2b297-131">lastModifiedBy</span></span>|[<span data-ttu-id="2b297-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="2b297-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="2b297-p107">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b297-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="2b297-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b297-135">lastModifiedDateTime</span></span>|<span data-ttu-id="2b297-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b297-136">DateTimeOffset</span></span>|<span data-ttu-id="2b297-p108">A data e hora da última modificação da seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b297-p108">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="2b297-141">links</span><span class="sxs-lookup"><span data-stu-id="2b297-141">links</span></span>|[<span data-ttu-id="2b297-142">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="2b297-142">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="2b297-p109">Links para abrir a seção. O link `oneNoteClientURL` abre a seção no cliente nativo do OneNote se ele estiver instalado. O link `oneNoteWebURL` abre a seção no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="2b297-p109">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="2b297-146">displayName</span><span class="sxs-lookup"><span data-stu-id="2b297-146">displayName</span></span>|<span data-ttu-id="2b297-147">String</span><span class="sxs-lookup"><span data-stu-id="2b297-147">String</span></span>|<span data-ttu-id="2b297-148">O nome da seção.</span><span class="sxs-lookup"><span data-stu-id="2b297-148">The name of the section.</span></span> |
|<span data-ttu-id="2b297-149">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="2b297-149">pagesUrl</span></span>|<span data-ttu-id="2b297-150">String</span><span class="sxs-lookup"><span data-stu-id="2b297-150">String</span></span>|<span data-ttu-id="2b297-p110">O ponto de extremidade `pages` onde você pode obter detalhes de todas as páginas na seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b297-p110">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="2b297-153">self</span><span class="sxs-lookup"><span data-stu-id="2b297-153">self</span></span>|<span data-ttu-id="2b297-154">String</span><span class="sxs-lookup"><span data-stu-id="2b297-154">String</span></span>|<span data-ttu-id="2b297-p111">O ponto de extremidade onde você pode obter detalhes sobre a seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b297-p111">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b297-157">Relações</span><span class="sxs-lookup"><span data-stu-id="2b297-157">Relationships</span></span>
| <span data-ttu-id="2b297-158">Relação</span><span class="sxs-lookup"><span data-stu-id="2b297-158">Relationship</span></span> | <span data-ttu-id="2b297-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b297-159">Type</span></span>   |<span data-ttu-id="2b297-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b297-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b297-161">páginas</span><span class="sxs-lookup"><span data-stu-id="2b297-161">pages</span></span>|<span data-ttu-id="2b297-162">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="2b297-162">[Page](page.md) collection</span></span>|<span data-ttu-id="2b297-p112">Obtém o conjunto de páginas da seção.  Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2b297-p112">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="2b297-166">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="2b297-166">parentNotebook</span></span>|[<span data-ttu-id="2b297-167">Notebook</span><span class="sxs-lookup"><span data-stu-id="2b297-167">Notebook</span></span>](notebook.md)|<span data-ttu-id="2b297-p113">O bloco de anotações que contém a seção.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b297-p113">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="2b297-170">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="2b297-170">parentSectionGroup</span></span>|[<span data-ttu-id="2b297-171">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="2b297-171">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="2b297-p114">O grupo de seção que contém a seção.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b297-p114">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="2b297-174">Métodos</span><span class="sxs-lookup"><span data-stu-id="2b297-174">Methods</span></span>

| <span data-ttu-id="2b297-175">Método</span><span class="sxs-lookup"><span data-stu-id="2b297-175">Method</span></span>           | <span data-ttu-id="2b297-176">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2b297-176">Return Type</span></span>    |<span data-ttu-id="2b297-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b297-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2b297-178">Get section</span><span class="sxs-lookup"><span data-stu-id="2b297-178">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="2b297-179">Section</span><span class="sxs-lookup"><span data-stu-id="2b297-179">Section</span></span>](section.md) |<span data-ttu-id="2b297-180">Leia as propriedades e as relações da seção.</span><span class="sxs-lookup"><span data-stu-id="2b297-180">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="2b297-181">Criar página</span><span class="sxs-lookup"><span data-stu-id="2b297-181">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="2b297-182">Página</span><span class="sxs-lookup"><span data-stu-id="2b297-182">Page</span></span>](page.md)| <span data-ttu-id="2b297-183">Crie uma página postando na coleção pages do grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="2b297-183">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="2b297-184">Listar páginas</span><span class="sxs-lookup"><span data-stu-id="2b297-184">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="2b297-185">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="2b297-185">[Page](page.md) collection</span></span>| <span data-ttu-id="2b297-186">Obtém uma coleção de páginas na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="2b297-186">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="2b297-187">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="2b297-187">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="2b297-188">None</span><span class="sxs-lookup"><span data-stu-id="2b297-188">None</span></span>|<span data-ttu-id="2b297-189">Copia a seção para um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="2b297-189">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="2b297-190">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="2b297-190">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="2b297-191">None</span><span class="sxs-lookup"><span data-stu-id="2b297-191">None</span></span>|<span data-ttu-id="2b297-192">Copia uma seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="2b297-192">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/section.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
