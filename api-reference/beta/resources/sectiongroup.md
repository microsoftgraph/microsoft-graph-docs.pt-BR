---
title: Tipo de recurso sectionGroup
description: Um grupo de seção em um bloco de anotações do OneNote. Grupos de seção podem conter seções e grupos de seção.
localization_priority: Normal
ms.openlocfilehash: 9e955d91fa49642100694da66421665a0d67b3da
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855423"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="50b24-104">Tipo de recurso sectionGroup</span><span class="sxs-lookup"><span data-stu-id="50b24-104">sectionGroup resource type</span></span>

> <span data-ttu-id="50b24-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="50b24-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50b24-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="50b24-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="50b24-p103">Um grupo de seção em um bloco de anotações do OneNote. Grupos de seção podem conter seções e grupos de seção.</span><span class="sxs-lookup"><span data-stu-id="50b24-p103">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="50b24-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50b24-109">JSON representation</span></span>

<span data-ttu-id="50b24-110">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50b24-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="50b24-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50b24-111">Properties</span></span>
| <span data-ttu-id="50b24-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50b24-112">Property</span></span>     | <span data-ttu-id="50b24-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="50b24-113">Type</span></span>   |<span data-ttu-id="50b24-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="50b24-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50b24-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="50b24-115">createdBy</span></span>|[<span data-ttu-id="50b24-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="50b24-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="50b24-p104">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50b24-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="50b24-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50b24-119">createdDateTime</span></span>|<span data-ttu-id="50b24-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50b24-120">DateTimeOffset</span></span>|<span data-ttu-id="50b24-p105">A data e hora da criação do grupo de seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50b24-p105">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="50b24-125">id</span><span class="sxs-lookup"><span data-stu-id="50b24-125">id</span></span>|<span data-ttu-id="50b24-126">String</span><span class="sxs-lookup"><span data-stu-id="50b24-126">String</span></span>|<span data-ttu-id="50b24-p106">O identificador exclusivo do grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50b24-p106">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="50b24-129">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="50b24-129">lastModifiedBy</span></span>|[<span data-ttu-id="50b24-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="50b24-130">identitySet</span></span>](identityset.md)|<span data-ttu-id="50b24-p107">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50b24-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="50b24-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50b24-133">lastModifiedDateTime</span></span>|<span data-ttu-id="50b24-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50b24-134">DateTimeOffset</span></span>|<span data-ttu-id="50b24-p108">A data e hora da última modificação do grupo de seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50b24-p108">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="50b24-139">displayName</span><span class="sxs-lookup"><span data-stu-id="50b24-139">displayName</span></span>|<span data-ttu-id="50b24-140">String</span><span class="sxs-lookup"><span data-stu-id="50b24-140">String</span></span>|<span data-ttu-id="50b24-141">O nome do grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="50b24-141">The name of the section group.</span></span>|
|<span data-ttu-id="50b24-142">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="50b24-142">sectionGroupsUrl</span></span>|<span data-ttu-id="50b24-143">String</span><span class="sxs-lookup"><span data-stu-id="50b24-143">String</span></span>|<span data-ttu-id="50b24-p109">A URL da propriedade de navegação `sectionGroups`, que retorna todos os grupos de seção no grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50b24-p109">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="50b24-146">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="50b24-146">sectionsUrl</span></span>|<span data-ttu-id="50b24-147">String</span><span class="sxs-lookup"><span data-stu-id="50b24-147">String</span></span>|<span data-ttu-id="50b24-p110">A URL da propriedade de navegação `sections`, que retorna todas as seções no grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50b24-p110">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="50b24-150">self</span><span class="sxs-lookup"><span data-stu-id="50b24-150">self</span></span>|<span data-ttu-id="50b24-151">String</span><span class="sxs-lookup"><span data-stu-id="50b24-151">String</span></span>|<span data-ttu-id="50b24-p111">O ponto de extremidade onde você pode obter detalhes sobre o grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50b24-p111">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50b24-154">Relações</span><span class="sxs-lookup"><span data-stu-id="50b24-154">Relationships</span></span>
| <span data-ttu-id="50b24-155">Relação</span><span class="sxs-lookup"><span data-stu-id="50b24-155">Relationship</span></span> | <span data-ttu-id="50b24-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="50b24-156">Type</span></span>   |<span data-ttu-id="50b24-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="50b24-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50b24-158">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="50b24-158">parentNotebook</span></span>|[<span data-ttu-id="50b24-159">Notebook</span><span class="sxs-lookup"><span data-stu-id="50b24-159">Notebook</span></span>](notebook.md)|<span data-ttu-id="50b24-p112">O bloco de anotações que contém o grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50b24-p112">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="50b24-162">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="50b24-162">parentSectionGroup</span></span>|[<span data-ttu-id="50b24-163">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="50b24-163">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="50b24-p113">O grupo de seção que contém o grupo de seção. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50b24-p113">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="50b24-166">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="50b24-166">sectionGroups</span></span>|<span data-ttu-id="50b24-167">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="50b24-167">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="50b24-p114">Os grupos de seção na seção. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="50b24-p114">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="50b24-171">sections</span><span class="sxs-lookup"><span data-stu-id="50b24-171">sections</span></span>|<span data-ttu-id="50b24-172">Coleção [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="50b24-172">[Section](section.md) collection</span></span>|<span data-ttu-id="50b24-p115">As seções no grupo de seção. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="50b24-p115">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="50b24-176">Métodos</span><span class="sxs-lookup"><span data-stu-id="50b24-176">Methods</span></span>

| <span data-ttu-id="50b24-177">Método</span><span class="sxs-lookup"><span data-stu-id="50b24-177">Method</span></span>           | <span data-ttu-id="50b24-178">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="50b24-178">Return Type</span></span>    |<span data-ttu-id="50b24-179">Descrição</span><span class="sxs-lookup"><span data-stu-id="50b24-179">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="50b24-180">Get section group</span><span class="sxs-lookup"><span data-stu-id="50b24-180">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="50b24-181">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="50b24-181">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="50b24-182">Leia as propriedades e as relações do grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="50b24-182">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="50b24-183">Criar grupo de seção</span><span class="sxs-lookup"><span data-stu-id="50b24-183">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="50b24-184">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="50b24-184">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="50b24-185">Crie um grupo de seção postando na coleção sectionGroups do grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="50b24-185">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="50b24-186">Listar grupos de seção</span><span class="sxs-lookup"><span data-stu-id="50b24-186">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="50b24-187">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="50b24-187">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="50b24-188">A coleção de grupos de seção no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="50b24-188">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="50b24-189">Criar seção</span><span class="sxs-lookup"><span data-stu-id="50b24-189">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="50b24-190">Section</span><span class="sxs-lookup"><span data-stu-id="50b24-190">Section</span></span>](section.md)| <span data-ttu-id="50b24-191">Crie uma seção postando na coleção sections do grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="50b24-191">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="50b24-192">Listar seções</span><span class="sxs-lookup"><span data-stu-id="50b24-192">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="50b24-193">Coleção [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="50b24-193">[Section](section.md) collection</span></span>| <span data-ttu-id="50b24-194">Obtenha uma coleção de seções no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="50b24-194">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
