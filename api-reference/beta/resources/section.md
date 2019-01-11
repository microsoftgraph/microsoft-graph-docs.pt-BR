---
title: Tipo de recurso section
description: Uma seção em um bloco de anotações do OneNote. As seções podem conter páginas.
localization_priority: Normal
ms.openlocfilehash: 181fa3399f13d0490d9cd7d4599d8208633107b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831841"
---
# <a name="section-resource-type"></a><span data-ttu-id="2269e-104">Tipo de recurso section</span><span class="sxs-lookup"><span data-stu-id="2269e-104">section resource type</span></span>

> <span data-ttu-id="2269e-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2269e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2269e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2269e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2269e-p103">Uma seção em um bloco de anotações do OneNote. As seções podem conter páginas.</span><span class="sxs-lookup"><span data-stu-id="2269e-p103">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2269e-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2269e-109">JSON representation</span></span>

<span data-ttu-id="2269e-110">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2269e-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="2269e-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2269e-111">Properties</span></span>
| <span data-ttu-id="2269e-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2269e-112">Property</span></span>     | <span data-ttu-id="2269e-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="2269e-113">Type</span></span>   |<span data-ttu-id="2269e-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="2269e-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2269e-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="2269e-115">createdBy</span></span>|[<span data-ttu-id="2269e-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="2269e-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="2269e-p104">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2269e-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="2269e-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2269e-119">createdDateTime</span></span>|<span data-ttu-id="2269e-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2269e-120">DateTimeOffset</span></span>|<span data-ttu-id="2269e-p105">A data e hora da criação da seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2269e-p105">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="2269e-125">id</span><span class="sxs-lookup"><span data-stu-id="2269e-125">id</span></span>|<span data-ttu-id="2269e-126">String</span><span class="sxs-lookup"><span data-stu-id="2269e-126">String</span></span>|<span data-ttu-id="2269e-p106">O identificador exclusivo da seção.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2269e-p106">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="2269e-129">isDefault</span><span class="sxs-lookup"><span data-stu-id="2269e-129">isDefault</span></span>|<span data-ttu-id="2269e-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="2269e-130">Boolean</span></span>|<span data-ttu-id="2269e-p107">Indica se esta é a seção padrão do usuário. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2269e-p107">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="2269e-133">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2269e-133">lastModifiedBy</span></span>|[<span data-ttu-id="2269e-134">identitySet</span><span class="sxs-lookup"><span data-stu-id="2269e-134">identitySet</span></span>](identityset.md)|<span data-ttu-id="2269e-p108">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2269e-p108">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="2269e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2269e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2269e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2269e-138">DateTimeOffset</span></span>|<span data-ttu-id="2269e-p109">A data e hora da última modificação da seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2269e-p109">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="2269e-143">links</span><span class="sxs-lookup"><span data-stu-id="2269e-143">links</span></span>|[<span data-ttu-id="2269e-144">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="2269e-144">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="2269e-p110">Links para abrir a seção. O link `oneNoteClientURL` abre a seção no cliente nativo do OneNote se ele estiver instalado. O link `oneNoteWebURL` abre a seção no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="2269e-p110">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="2269e-148">displayName</span><span class="sxs-lookup"><span data-stu-id="2269e-148">displayName</span></span>|<span data-ttu-id="2269e-149">String</span><span class="sxs-lookup"><span data-stu-id="2269e-149">String</span></span>|<span data-ttu-id="2269e-150">O nome da seção.</span><span class="sxs-lookup"><span data-stu-id="2269e-150">The name of the section.</span></span> |
|<span data-ttu-id="2269e-151">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="2269e-151">pagesUrl</span></span>|<span data-ttu-id="2269e-152">String</span><span class="sxs-lookup"><span data-stu-id="2269e-152">String</span></span>|<span data-ttu-id="2269e-p111">O ponto de extremidade `pages` onde você pode obter detalhes de todas as páginas na seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2269e-p111">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="2269e-155">self</span><span class="sxs-lookup"><span data-stu-id="2269e-155">self</span></span>|<span data-ttu-id="2269e-156">String</span><span class="sxs-lookup"><span data-stu-id="2269e-156">String</span></span>|<span data-ttu-id="2269e-p112">O ponto de extremidade onde você pode obter detalhes sobre a seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2269e-p112">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2269e-159">Relações</span><span class="sxs-lookup"><span data-stu-id="2269e-159">Relationships</span></span>
| <span data-ttu-id="2269e-160">Relação</span><span class="sxs-lookup"><span data-stu-id="2269e-160">Relationship</span></span> | <span data-ttu-id="2269e-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="2269e-161">Type</span></span>   |<span data-ttu-id="2269e-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="2269e-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2269e-163">páginas</span><span class="sxs-lookup"><span data-stu-id="2269e-163">pages</span></span>|<span data-ttu-id="2269e-164">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="2269e-164">[Page](page.md) collection</span></span>|<span data-ttu-id="2269e-p113">Obtém o conjunto de páginas da seção.  Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2269e-p113">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="2269e-168">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="2269e-168">parentNotebook</span></span>|[<span data-ttu-id="2269e-169">Notebook</span><span class="sxs-lookup"><span data-stu-id="2269e-169">Notebook</span></span>](notebook.md)|<span data-ttu-id="2269e-p114">O bloco de anotações que contém a seção.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2269e-p114">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="2269e-172">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="2269e-172">parentSectionGroup</span></span>|[<span data-ttu-id="2269e-173">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="2269e-173">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="2269e-p115">O grupo de seção que contém a seção.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2269e-p115">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="2269e-176">Métodos</span><span class="sxs-lookup"><span data-stu-id="2269e-176">Methods</span></span>

| <span data-ttu-id="2269e-177">Método</span><span class="sxs-lookup"><span data-stu-id="2269e-177">Method</span></span>           | <span data-ttu-id="2269e-178">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2269e-178">Return Type</span></span>    |<span data-ttu-id="2269e-179">Descrição</span><span class="sxs-lookup"><span data-stu-id="2269e-179">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2269e-180">Get section</span><span class="sxs-lookup"><span data-stu-id="2269e-180">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="2269e-181">Section</span><span class="sxs-lookup"><span data-stu-id="2269e-181">Section</span></span>](section.md) |<span data-ttu-id="2269e-182">Leia as propriedades e as relações da seção.</span><span class="sxs-lookup"><span data-stu-id="2269e-182">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="2269e-183">Criar página</span><span class="sxs-lookup"><span data-stu-id="2269e-183">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="2269e-184">Página</span><span class="sxs-lookup"><span data-stu-id="2269e-184">Page</span></span>](page.md)| <span data-ttu-id="2269e-185">Crie uma página postando na coleção pages do grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="2269e-185">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="2269e-186">Listar páginas</span><span class="sxs-lookup"><span data-stu-id="2269e-186">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="2269e-187">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="2269e-187">[Page](page.md) collection</span></span>| <span data-ttu-id="2269e-188">Obtém uma coleção de páginas na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="2269e-188">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="2269e-189">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="2269e-189">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="2269e-190">None</span><span class="sxs-lookup"><span data-stu-id="2269e-190">None</span></span>|<span data-ttu-id="2269e-191">Copia a seção para um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="2269e-191">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="2269e-192">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="2269e-192">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="2269e-193">None</span><span class="sxs-lookup"><span data-stu-id="2269e-193">None</span></span>|<span data-ttu-id="2269e-194">Copia uma seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="2269e-194">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
