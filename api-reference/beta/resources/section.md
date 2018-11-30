---
title: Tipo de recurso section
description: Uma seção em um bloco de anotações do OneNote. As seções podem conter páginas.
ms.openlocfilehash: c07f8f2e5c9f9f9d367cbc1186983c0870b2e979
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033826"
---
# <a name="section-resource-type"></a><span data-ttu-id="53ef7-104">Tipo de recurso section</span><span class="sxs-lookup"><span data-stu-id="53ef7-104">section resource type</span></span>

> <span data-ttu-id="53ef7-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="53ef7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53ef7-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="53ef7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="53ef7-p103">Uma seção em um bloco de anotações do OneNote. As seções podem conter páginas.</span><span class="sxs-lookup"><span data-stu-id="53ef7-p103">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="53ef7-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53ef7-109">JSON representation</span></span>

<span data-ttu-id="53ef7-110">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="53ef7-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="53ef7-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53ef7-111">Properties</span></span>
| <span data-ttu-id="53ef7-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53ef7-112">Property</span></span>     | <span data-ttu-id="53ef7-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="53ef7-113">Type</span></span>   |<span data-ttu-id="53ef7-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="53ef7-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53ef7-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="53ef7-115">createdBy</span></span>|[<span data-ttu-id="53ef7-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="53ef7-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="53ef7-p104">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53ef7-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="53ef7-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53ef7-119">createdDateTime</span></span>|<span data-ttu-id="53ef7-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53ef7-120">DateTimeOffset</span></span>|<span data-ttu-id="53ef7-p105">A data e hora da criação da seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53ef7-p105">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="53ef7-125">id</span><span class="sxs-lookup"><span data-stu-id="53ef7-125">id</span></span>|<span data-ttu-id="53ef7-126">String</span><span class="sxs-lookup"><span data-stu-id="53ef7-126">String</span></span>|<span data-ttu-id="53ef7-p106">O identificador exclusivo da seção.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53ef7-p106">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="53ef7-129">isDefault</span><span class="sxs-lookup"><span data-stu-id="53ef7-129">isDefault</span></span>|<span data-ttu-id="53ef7-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="53ef7-130">Boolean</span></span>|<span data-ttu-id="53ef7-p107">Indica se esta é a seção padrão do usuário. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53ef7-p107">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="53ef7-133">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="53ef7-133">lastModifiedBy</span></span>|[<span data-ttu-id="53ef7-134">identitySet</span><span class="sxs-lookup"><span data-stu-id="53ef7-134">identitySet</span></span>](identityset.md)|<span data-ttu-id="53ef7-p108">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53ef7-p108">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="53ef7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53ef7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="53ef7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53ef7-138">DateTimeOffset</span></span>|<span data-ttu-id="53ef7-p109">A data e hora da última modificação da seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53ef7-p109">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="53ef7-143">links</span><span class="sxs-lookup"><span data-stu-id="53ef7-143">links</span></span>|[<span data-ttu-id="53ef7-144">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="53ef7-144">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="53ef7-p110">Links para abrir a seção. O link `oneNoteClientURL` abre a seção no cliente nativo do OneNote se ele estiver instalado. O link `oneNoteWebURL` abre a seção no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="53ef7-p110">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="53ef7-148">displayName</span><span class="sxs-lookup"><span data-stu-id="53ef7-148">displayName</span></span>|<span data-ttu-id="53ef7-149">String</span><span class="sxs-lookup"><span data-stu-id="53ef7-149">String</span></span>|<span data-ttu-id="53ef7-150">O nome da seção.</span><span class="sxs-lookup"><span data-stu-id="53ef7-150">The name of the section.</span></span> |
|<span data-ttu-id="53ef7-151">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="53ef7-151">pagesUrl</span></span>|<span data-ttu-id="53ef7-152">String</span><span class="sxs-lookup"><span data-stu-id="53ef7-152">String</span></span>|<span data-ttu-id="53ef7-p111">O ponto de extremidade `pages` onde você pode obter detalhes de todas as páginas na seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53ef7-p111">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="53ef7-155">self</span><span class="sxs-lookup"><span data-stu-id="53ef7-155">self</span></span>|<span data-ttu-id="53ef7-156">String</span><span class="sxs-lookup"><span data-stu-id="53ef7-156">String</span></span>|<span data-ttu-id="53ef7-p112">O ponto de extremidade onde você pode obter detalhes sobre a seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53ef7-p112">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53ef7-159">Relações</span><span class="sxs-lookup"><span data-stu-id="53ef7-159">Relationships</span></span>
| <span data-ttu-id="53ef7-160">Relação</span><span class="sxs-lookup"><span data-stu-id="53ef7-160">Relationship</span></span> | <span data-ttu-id="53ef7-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="53ef7-161">Type</span></span>   |<span data-ttu-id="53ef7-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="53ef7-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53ef7-163">páginas</span><span class="sxs-lookup"><span data-stu-id="53ef7-163">pages</span></span>|<span data-ttu-id="53ef7-164">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="53ef7-164">[Page](page.md) collection</span></span>|<span data-ttu-id="53ef7-p113">Obtém o conjunto de páginas da seção.  Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="53ef7-p113">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="53ef7-168">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="53ef7-168">parentNotebook</span></span>|[<span data-ttu-id="53ef7-169">Notebook</span><span class="sxs-lookup"><span data-stu-id="53ef7-169">Notebook</span></span>](notebook.md)|<span data-ttu-id="53ef7-p114">O bloco de anotações que contém a seção.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53ef7-p114">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="53ef7-172">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="53ef7-172">parentSectionGroup</span></span>|[<span data-ttu-id="53ef7-173">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="53ef7-173">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="53ef7-p115">O grupo de seção que contém a seção.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53ef7-p115">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="53ef7-176">Métodos</span><span class="sxs-lookup"><span data-stu-id="53ef7-176">Methods</span></span>

| <span data-ttu-id="53ef7-177">Método</span><span class="sxs-lookup"><span data-stu-id="53ef7-177">Method</span></span>           | <span data-ttu-id="53ef7-178">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="53ef7-178">Return Type</span></span>    |<span data-ttu-id="53ef7-179">Descrição</span><span class="sxs-lookup"><span data-stu-id="53ef7-179">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="53ef7-180">Get section</span><span class="sxs-lookup"><span data-stu-id="53ef7-180">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="53ef7-181">Section</span><span class="sxs-lookup"><span data-stu-id="53ef7-181">Section</span></span>](section.md) |<span data-ttu-id="53ef7-182">Leia as propriedades e as relações da seção.</span><span class="sxs-lookup"><span data-stu-id="53ef7-182">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="53ef7-183">Criar página</span><span class="sxs-lookup"><span data-stu-id="53ef7-183">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="53ef7-184">Página</span><span class="sxs-lookup"><span data-stu-id="53ef7-184">Page</span></span>](page.md)| <span data-ttu-id="53ef7-185">Crie uma página postando na coleção pages do grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="53ef7-185">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="53ef7-186">Listar páginas</span><span class="sxs-lookup"><span data-stu-id="53ef7-186">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="53ef7-187">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="53ef7-187">[Page](page.md) collection</span></span>| <span data-ttu-id="53ef7-188">Obtém uma coleção de páginas na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="53ef7-188">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="53ef7-189">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="53ef7-189">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="53ef7-190">None</span><span class="sxs-lookup"><span data-stu-id="53ef7-190">None</span></span>|<span data-ttu-id="53ef7-191">Copia a seção para um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="53ef7-191">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="53ef7-192">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="53ef7-192">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="53ef7-193">None</span><span class="sxs-lookup"><span data-stu-id="53ef7-193">None</span></span>|<span data-ttu-id="53ef7-194">Copia uma seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="53ef7-194">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
