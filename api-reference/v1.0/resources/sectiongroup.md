---
title: Tipo de recurso sectionGroup
description: Um grupo de seção em um bloco de anotações do OneNote. Os grupos de seções podem conter seções e grupos de seções.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 5968a327800c823cd5767a382d019fba39f66927
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722003"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="950e0-104">Tipo de recurso sectionGroup</span><span class="sxs-lookup"><span data-stu-id="950e0-104">sectionGroup resource type</span></span>

<span data-ttu-id="950e0-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="950e0-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="950e0-106">Um grupo de seção em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="950e0-106">A section group in a OneNote notebook.</span></span> <span data-ttu-id="950e0-107">Os grupos de seções podem conter seções e grupos de seções.</span><span class="sxs-lookup"><span data-stu-id="950e0-107">Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="950e0-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="950e0-108">JSON representation</span></span>

<span data-ttu-id="950e0-109">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="950e0-109">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="950e0-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="950e0-110">Properties</span></span>
| <span data-ttu-id="950e0-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="950e0-111">Property</span></span>     | <span data-ttu-id="950e0-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="950e0-112">Type</span></span>   |<span data-ttu-id="950e0-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="950e0-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="950e0-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="950e0-114">createdBy</span></span>|[<span data-ttu-id="950e0-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="950e0-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="950e0-p103">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="950e0-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="950e0-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="950e0-118">createdDateTime</span></span>|<span data-ttu-id="950e0-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="950e0-119">DateTimeOffset</span></span>|<span data-ttu-id="950e0-120">A data e a hora em que o grupo de seções foi criado.</span><span class="sxs-lookup"><span data-stu-id="950e0-120">The date and time when the section group was created.</span></span> <span data-ttu-id="950e0-121">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="950e0-121">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="950e0-122">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="950e0-122">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="950e0-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="950e0-123">Read-only.</span></span>|
|<span data-ttu-id="950e0-124">id</span><span class="sxs-lookup"><span data-stu-id="950e0-124">id</span></span>|<span data-ttu-id="950e0-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="950e0-125">String</span></span>|<span data-ttu-id="950e0-126">O identificador exclusivo do grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="950e0-126">The unique identifier of the section group.</span></span> <span data-ttu-id="950e0-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="950e0-127">Read-only.</span></span>|
|<span data-ttu-id="950e0-128">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="950e0-128">lastModifiedBy</span></span>|[<span data-ttu-id="950e0-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="950e0-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="950e0-p106">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="950e0-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="950e0-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="950e0-132">lastModifiedDateTime</span></span>|<span data-ttu-id="950e0-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="950e0-133">DateTimeOffset</span></span>|<span data-ttu-id="950e0-134">A data e a hora em que o grupo de seções foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="950e0-134">The date and time when the section group was last modified.</span></span> <span data-ttu-id="950e0-135">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="950e0-135">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="950e0-136">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="950e0-136">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="950e0-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="950e0-137">Read-only.</span></span>|
|<span data-ttu-id="950e0-138">displayName</span><span class="sxs-lookup"><span data-stu-id="950e0-138">displayName</span></span>|<span data-ttu-id="950e0-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="950e0-139">String</span></span>|<span data-ttu-id="950e0-140">O nome do grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="950e0-140">The name of the section group.</span></span>|
|<span data-ttu-id="950e0-141">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="950e0-141">sectionGroupsUrl</span></span>|<span data-ttu-id="950e0-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="950e0-142">String</span></span>|<span data-ttu-id="950e0-143">A URL da `sectionGroups` propriedade de navegação, que retorna todos os grupos de seções no grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="950e0-143">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group.</span></span> <span data-ttu-id="950e0-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="950e0-144">Read-only.</span></span>|
|<span data-ttu-id="950e0-145">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="950e0-145">sectionsUrl</span></span>|<span data-ttu-id="950e0-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="950e0-146">String</span></span>|<span data-ttu-id="950e0-147">A URL da `sections` propriedade de navegação, que retorna todas as seções no grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="950e0-147">The URL for the `sections` navigation property, which returns all the sections in the section group.</span></span> <span data-ttu-id="950e0-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="950e0-148">Read-only.</span></span>|
|<span data-ttu-id="950e0-149">self</span><span class="sxs-lookup"><span data-stu-id="950e0-149">self</span></span>|<span data-ttu-id="950e0-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="950e0-150">String</span></span>|<span data-ttu-id="950e0-151">O ponto de extremidade onde você pode obter detalhes sobre o grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="950e0-151">The endpoint where you can get details about the section group.</span></span> <span data-ttu-id="950e0-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="950e0-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="950e0-153">Relações</span><span class="sxs-lookup"><span data-stu-id="950e0-153">Relationships</span></span>
| <span data-ttu-id="950e0-154">Relação</span><span class="sxs-lookup"><span data-stu-id="950e0-154">Relationship</span></span> | <span data-ttu-id="950e0-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="950e0-155">Type</span></span>   |<span data-ttu-id="950e0-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="950e0-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="950e0-157">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="950e0-157">parentNotebook</span></span>|[<span data-ttu-id="950e0-158">Notebook</span><span class="sxs-lookup"><span data-stu-id="950e0-158">Notebook</span></span>](notebook.md)|<span data-ttu-id="950e0-159">O bloco de anotações que contém o grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="950e0-159">The notebook that contains the section group.</span></span> <span data-ttu-id="950e0-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="950e0-160">Read-only.</span></span>|
|<span data-ttu-id="950e0-161">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="950e0-161">parentSectionGroup</span></span>|[<span data-ttu-id="950e0-162">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="950e0-162">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="950e0-163">O grupo de seções que contém o grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="950e0-163">The section group that contains the section group.</span></span> <span data-ttu-id="950e0-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="950e0-164">Read-only.</span></span>|
|<span data-ttu-id="950e0-165">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="950e0-165">sectionGroups</span></span>|<span data-ttu-id="950e0-166">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="950e0-166">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="950e0-167">Os grupos de seção na seção.</span><span class="sxs-lookup"><span data-stu-id="950e0-167">The section groups in the section.</span></span> <span data-ttu-id="950e0-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="950e0-168">Read-only.</span></span> <span data-ttu-id="950e0-169">Anulável.</span><span class="sxs-lookup"><span data-stu-id="950e0-169">Nullable.</span></span>|
|<span data-ttu-id="950e0-170">seções</span><span class="sxs-lookup"><span data-stu-id="950e0-170">sections</span></span>|<span data-ttu-id="950e0-171">Coleção [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="950e0-171">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="950e0-172">As seções no grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="950e0-172">The sections in the section group.</span></span> <span data-ttu-id="950e0-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="950e0-173">Read-only.</span></span> <span data-ttu-id="950e0-174">Anulável.</span><span class="sxs-lookup"><span data-stu-id="950e0-174">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="950e0-175">Métodos</span><span class="sxs-lookup"><span data-stu-id="950e0-175">Methods</span></span>

| <span data-ttu-id="950e0-176">Método</span><span class="sxs-lookup"><span data-stu-id="950e0-176">Method</span></span>           | <span data-ttu-id="950e0-177">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="950e0-177">Return Type</span></span>    |<span data-ttu-id="950e0-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="950e0-178">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="950e0-179">Obter grupo de seções</span><span class="sxs-lookup"><span data-stu-id="950e0-179">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="950e0-180">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="950e0-180">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="950e0-181">Leia as propriedades e as relações do grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="950e0-181">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="950e0-182">Criar grupo de seções</span><span class="sxs-lookup"><span data-stu-id="950e0-182">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="950e0-183">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="950e0-183">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="950e0-184">Crie um grupo de seções postando na coleção sectionGroups no grupo de seções especificado.</span><span class="sxs-lookup"><span data-stu-id="950e0-184">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="950e0-185">List section groups</span><span class="sxs-lookup"><span data-stu-id="950e0-185">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="950e0-186">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="950e0-186">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="950e0-187">Obter coleção de grupos de seções no grupo de seções especificado.</span><span class="sxs-lookup"><span data-stu-id="950e0-187">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="950e0-188">Criar seção</span><span class="sxs-lookup"><span data-stu-id="950e0-188">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="950e0-189">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="950e0-189">OnenoteSection</span></span>](section.md)| <span data-ttu-id="950e0-190">Crie uma seção postando na coleção sections no grupo de seções especificado.</span><span class="sxs-lookup"><span data-stu-id="950e0-190">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="950e0-191">Listar seções</span><span class="sxs-lookup"><span data-stu-id="950e0-191">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="950e0-192">Coleção [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="950e0-192">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="950e0-193">Obter uma coleção de seções no grupo de seções especificado.</span><span class="sxs-lookup"><span data-stu-id="950e0-193">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

