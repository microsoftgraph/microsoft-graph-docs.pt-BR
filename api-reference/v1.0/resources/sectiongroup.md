---
title: tipo de recurso de @ @ @ Section
description: Um grupo de seções em um bloco de anotações do OneNote. Os grupos de seções podem conter seções e grupos de seções.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ec27343121ba20ef65703f3df1d53e6c62ccc8e4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579139"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="f4b29-104">tipo de recurso de @ @ @ Section</span><span class="sxs-lookup"><span data-stu-id="f4b29-104">sectionGroup resource type</span></span>

<span data-ttu-id="f4b29-105">Um grupo de seções em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f4b29-105">A section group in a OneNote notebook.</span></span> <span data-ttu-id="f4b29-106">Os grupos de seções podem conter seções e grupos de seções.</span><span class="sxs-lookup"><span data-stu-id="f4b29-106">Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4b29-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4b29-107">JSON representation</span></span>

<span data-ttu-id="f4b29-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4b29-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="f4b29-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4b29-109">Properties</span></span>
| <span data-ttu-id="f4b29-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4b29-110">Property</span></span>     | <span data-ttu-id="f4b29-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4b29-111">Type</span></span>   |<span data-ttu-id="f4b29-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4b29-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4b29-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="f4b29-113">createdBy</span></span>|[<span data-ttu-id="f4b29-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="f4b29-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="f4b29-p103">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4b29-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="f4b29-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4b29-117">createdDateTime</span></span>|<span data-ttu-id="f4b29-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4b29-118">DateTimeOffset</span></span>|<span data-ttu-id="f4b29-119">A data e a hora em que o grupo de seções foi criado.</span><span class="sxs-lookup"><span data-stu-id="f4b29-119">The date and time when the section group was created.</span></span> <span data-ttu-id="f4b29-120">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f4b29-120">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f4b29-121">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f4b29-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f4b29-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4b29-122">Read-only.</span></span>|
|<span data-ttu-id="f4b29-123">id</span><span class="sxs-lookup"><span data-stu-id="f4b29-123">id</span></span>|<span data-ttu-id="f4b29-124">String</span><span class="sxs-lookup"><span data-stu-id="f4b29-124">String</span></span>|<span data-ttu-id="f4b29-125">O identificador exclusivo do grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="f4b29-125">The unique identifier of the section group.</span></span> <span data-ttu-id="f4b29-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4b29-126">Read-only.</span></span>|
|<span data-ttu-id="f4b29-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f4b29-127">lastModifiedBy</span></span>|[<span data-ttu-id="f4b29-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="f4b29-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="f4b29-p106">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4b29-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="f4b29-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4b29-131">lastModifiedDateTime</span></span>|<span data-ttu-id="f4b29-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4b29-132">DateTimeOffset</span></span>|<span data-ttu-id="f4b29-133">A data e a hora em que o grupo de seções foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f4b29-133">The date and time when the section group was last modified.</span></span> <span data-ttu-id="f4b29-134">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f4b29-134">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f4b29-135">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f4b29-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f4b29-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4b29-136">Read-only.</span></span>|
|<span data-ttu-id="f4b29-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f4b29-137">displayName</span></span>|<span data-ttu-id="f4b29-138">String</span><span class="sxs-lookup"><span data-stu-id="f4b29-138">String</span></span>|<span data-ttu-id="f4b29-139">O nome do grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="f4b29-139">The name of the section group.</span></span>|
|<span data-ttu-id="f4b29-140">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="f4b29-140">sectionGroupsUrl</span></span>|<span data-ttu-id="f4b29-141">String</span><span class="sxs-lookup"><span data-stu-id="f4b29-141">String</span></span>|<span data-ttu-id="f4b29-142">A URL da propriedade `sectionGroups` de navegação, que retorna todos os grupos de seção no grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="f4b29-142">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group.</span></span> <span data-ttu-id="f4b29-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4b29-143">Read-only.</span></span>|
|<span data-ttu-id="f4b29-144">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="f4b29-144">sectionsUrl</span></span>|<span data-ttu-id="f4b29-145">String</span><span class="sxs-lookup"><span data-stu-id="f4b29-145">String</span></span>|<span data-ttu-id="f4b29-146">A URL da propriedade `sections` de navegação, que retorna todas as seções no grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="f4b29-146">The URL for the `sections` navigation property, which returns all the sections in the section group.</span></span> <span data-ttu-id="f4b29-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4b29-147">Read-only.</span></span>|
|<span data-ttu-id="f4b29-148">própria</span><span class="sxs-lookup"><span data-stu-id="f4b29-148">self</span></span>|<span data-ttu-id="f4b29-149">String</span><span class="sxs-lookup"><span data-stu-id="f4b29-149">String</span></span>|<span data-ttu-id="f4b29-150">O ponto de extremidade onde você pode obter detalhes sobre o grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="f4b29-150">The endpoint where you can get details about the section group.</span></span> <span data-ttu-id="f4b29-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4b29-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4b29-152">Relações</span><span class="sxs-lookup"><span data-stu-id="f4b29-152">Relationships</span></span>
| <span data-ttu-id="f4b29-153">Relação</span><span class="sxs-lookup"><span data-stu-id="f4b29-153">Relationship</span></span> | <span data-ttu-id="f4b29-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4b29-154">Type</span></span>   |<span data-ttu-id="f4b29-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4b29-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4b29-156">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="f4b29-156">parentNotebook</span></span>|[<span data-ttu-id="f4b29-157">Bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="f4b29-157">Notebook</span></span>](notebook.md)|<span data-ttu-id="f4b29-158">O bloco de anotações que contém o grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="f4b29-158">The notebook that contains the section group.</span></span> <span data-ttu-id="f4b29-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4b29-159">Read-only.</span></span>|
|<span data-ttu-id="f4b29-160">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="f4b29-160">parentSectionGroup</span></span>|[<span data-ttu-id="f4b29-161">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="f4b29-161">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="f4b29-162">O grupo de seções que contém o grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="f4b29-162">The section group that contains the section group.</span></span> <span data-ttu-id="f4b29-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4b29-163">Read-only.</span></span>|
|<span data-ttu-id="f4b29-164">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="f4b29-164">sectionGroups</span></span>|<span data-ttu-id="f4b29-165">Coleção de [seções](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="f4b29-165">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="f4b29-166">Os grupos de seção na seção.</span><span class="sxs-lookup"><span data-stu-id="f4b29-166">The section groups in the section.</span></span> <span data-ttu-id="f4b29-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4b29-167">Read-only.</span></span> <span data-ttu-id="f4b29-168">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f4b29-168">Nullable.</span></span>|
|<span data-ttu-id="f4b29-169">sections</span><span class="sxs-lookup"><span data-stu-id="f4b29-169">sections</span></span>|<span data-ttu-id="f4b29-170">Coleção [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="f4b29-170">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="f4b29-171">As seções no grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="f4b29-171">The sections in the section group.</span></span> <span data-ttu-id="f4b29-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4b29-172">Read-only.</span></span> <span data-ttu-id="f4b29-173">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f4b29-173">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="f4b29-174">Métodos</span><span class="sxs-lookup"><span data-stu-id="f4b29-174">Methods</span></span>

| <span data-ttu-id="f4b29-175">Método</span><span class="sxs-lookup"><span data-stu-id="f4b29-175">Method</span></span>           | <span data-ttu-id="f4b29-176">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f4b29-176">Return Type</span></span>    |<span data-ttu-id="f4b29-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4b29-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f4b29-178">Obter grupo de seções</span><span class="sxs-lookup"><span data-stu-id="f4b29-178">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="f4b29-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="f4b29-179">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="f4b29-180">Leia as propriedades e as relações do grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="f4b29-180">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="f4b29-181">Criar grupo de seções</span><span class="sxs-lookup"><span data-stu-id="f4b29-181">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="f4b29-182">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="f4b29-182">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="f4b29-183">Crie um grupo de seção postando na coleção sectionGroups no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="f4b29-183">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="f4b29-184">Listar grupos de seções</span><span class="sxs-lookup"><span data-stu-id="f4b29-184">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="f4b29-185">Coleção de [seções](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="f4b29-185">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="f4b29-186">Obtém a coleção de grupos de seção no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="f4b29-186">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="f4b29-187">Criar seção</span><span class="sxs-lookup"><span data-stu-id="f4b29-187">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="f4b29-188">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="f4b29-188">OnenoteSection</span></span>](section.md)| <span data-ttu-id="f4b29-189">Crie uma seção postando na coleção Sections no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="f4b29-189">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="f4b29-190">Listar seções</span><span class="sxs-lookup"><span data-stu-id="f4b29-190">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="f4b29-191">Coleção [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="f4b29-191">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="f4b29-192">Obter uma coleção de seções no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="f4b29-192">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
