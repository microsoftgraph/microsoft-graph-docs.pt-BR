---
title: tipo de recurso de @ @ @ Section
description: Um grupo de seções em um bloco de anotações do OneNote. Os grupos de seções podem conter seções e grupos de seções.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: dee2ca947af83f81f482ad280d0ae0c77b69fc56
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087625"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="23fae-104">tipo de recurso de @ @ @ Section</span><span class="sxs-lookup"><span data-stu-id="23fae-104">sectionGroup resource type</span></span>

<span data-ttu-id="23fae-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23fae-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23fae-106">Um grupo de seções em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="23fae-106">A section group in a OneNote notebook.</span></span> <span data-ttu-id="23fae-107">Os grupos de seções podem conter seções e grupos de seções.</span><span class="sxs-lookup"><span data-stu-id="23fae-107">Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23fae-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23fae-108">JSON representation</span></span>

<span data-ttu-id="23fae-109">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23fae-109">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "keyProperty": "id",
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
## <a name="properties"></a><span data-ttu-id="23fae-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23fae-110">Properties</span></span>
| <span data-ttu-id="23fae-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23fae-111">Property</span></span>     | <span data-ttu-id="23fae-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="23fae-112">Type</span></span>   |<span data-ttu-id="23fae-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="23fae-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23fae-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="23fae-114">createdBy</span></span>|[<span data-ttu-id="23fae-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="23fae-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="23fae-p103">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23fae-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="23fae-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23fae-118">createdDateTime</span></span>|<span data-ttu-id="23fae-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23fae-119">DateTimeOffset</span></span>|<span data-ttu-id="23fae-120">A data e a hora em que o grupo de seções foi criado.</span><span class="sxs-lookup"><span data-stu-id="23fae-120">The date and time when the section group was created.</span></span> <span data-ttu-id="23fae-121">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="23fae-121">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="23fae-122">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="23fae-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="23fae-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23fae-123">Read-only.</span></span>|
|<span data-ttu-id="23fae-124">id</span><span class="sxs-lookup"><span data-stu-id="23fae-124">id</span></span>|<span data-ttu-id="23fae-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23fae-125">String</span></span>|<span data-ttu-id="23fae-126">O identificador exclusivo do grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="23fae-126">The unique identifier of the section group.</span></span> <span data-ttu-id="23fae-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23fae-127">Read-only.</span></span>|
|<span data-ttu-id="23fae-128">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="23fae-128">lastModifiedBy</span></span>|[<span data-ttu-id="23fae-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="23fae-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="23fae-p106">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23fae-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="23fae-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23fae-132">lastModifiedDateTime</span></span>|<span data-ttu-id="23fae-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23fae-133">DateTimeOffset</span></span>|<span data-ttu-id="23fae-134">A data e a hora em que o grupo de seções foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="23fae-134">The date and time when the section group was last modified.</span></span> <span data-ttu-id="23fae-135">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="23fae-135">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="23fae-136">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="23fae-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="23fae-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23fae-137">Read-only.</span></span>|
|<span data-ttu-id="23fae-138">displayName</span><span class="sxs-lookup"><span data-stu-id="23fae-138">displayName</span></span>|<span data-ttu-id="23fae-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23fae-139">String</span></span>|<span data-ttu-id="23fae-140">O nome do grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="23fae-140">The name of the section group.</span></span>|
|<span data-ttu-id="23fae-141">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="23fae-141">sectionGroupsUrl</span></span>|<span data-ttu-id="23fae-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23fae-142">String</span></span>|<span data-ttu-id="23fae-143">A URL da `sectionGroups` propriedade de navegação, que retorna todos os grupos de seção no grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="23fae-143">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group.</span></span> <span data-ttu-id="23fae-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23fae-144">Read-only.</span></span>|
|<span data-ttu-id="23fae-145">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="23fae-145">sectionsUrl</span></span>|<span data-ttu-id="23fae-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23fae-146">String</span></span>|<span data-ttu-id="23fae-147">A URL da `sections` propriedade de navegação, que retorna todas as seções no grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="23fae-147">The URL for the `sections` navigation property, which returns all the sections in the section group.</span></span> <span data-ttu-id="23fae-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23fae-148">Read-only.</span></span>|
|<span data-ttu-id="23fae-149">própria</span><span class="sxs-lookup"><span data-stu-id="23fae-149">self</span></span>|<span data-ttu-id="23fae-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23fae-150">String</span></span>|<span data-ttu-id="23fae-151">O ponto de extremidade onde você pode obter detalhes sobre o grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="23fae-151">The endpoint where you can get details about the section group.</span></span> <span data-ttu-id="23fae-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23fae-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23fae-153">Relações</span><span class="sxs-lookup"><span data-stu-id="23fae-153">Relationships</span></span>
| <span data-ttu-id="23fae-154">Relação</span><span class="sxs-lookup"><span data-stu-id="23fae-154">Relationship</span></span> | <span data-ttu-id="23fae-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="23fae-155">Type</span></span>   |<span data-ttu-id="23fae-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="23fae-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23fae-157">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="23fae-157">parentNotebook</span></span>|[<span data-ttu-id="23fae-158">bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="23fae-158">notebook</span></span>](notebook.md)|<span data-ttu-id="23fae-159">O bloco de anotações que contém o grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="23fae-159">The notebook that contains the section group.</span></span> <span data-ttu-id="23fae-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23fae-160">Read-only.</span></span>|
|<span data-ttu-id="23fae-161">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="23fae-161">parentSectionGroup</span></span>|[<span data-ttu-id="23fae-162">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="23fae-162">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="23fae-163">O grupo de seções que contém o grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="23fae-163">The section group that contains the section group.</span></span> <span data-ttu-id="23fae-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23fae-164">Read-only.</span></span>|
|<span data-ttu-id="23fae-165">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="23fae-165">sectionGroups</span></span>|<span data-ttu-id="23fae-166">coleção de [seções](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="23fae-166">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="23fae-167">Os grupos de seção na seção.</span><span class="sxs-lookup"><span data-stu-id="23fae-167">The section groups in the section.</span></span> <span data-ttu-id="23fae-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23fae-168">Read-only.</span></span> <span data-ttu-id="23fae-169">Anulável.</span><span class="sxs-lookup"><span data-stu-id="23fae-169">Nullable.</span></span>|
|<span data-ttu-id="23fae-170">seções</span><span class="sxs-lookup"><span data-stu-id="23fae-170">sections</span></span>|<span data-ttu-id="23fae-171">coleção [onenoteSection](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="23fae-171">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="23fae-172">As seções no grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="23fae-172">The sections in the section group.</span></span> <span data-ttu-id="23fae-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23fae-173">Read-only.</span></span> <span data-ttu-id="23fae-174">Anulável.</span><span class="sxs-lookup"><span data-stu-id="23fae-174">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="23fae-175">Métodos</span><span class="sxs-lookup"><span data-stu-id="23fae-175">Methods</span></span>

| <span data-ttu-id="23fae-176">Método</span><span class="sxs-lookup"><span data-stu-id="23fae-176">Method</span></span>           | <span data-ttu-id="23fae-177">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="23fae-177">Return Type</span></span>    |<span data-ttu-id="23fae-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="23fae-178">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="23fae-179">Obter grupo de seções</span><span class="sxs-lookup"><span data-stu-id="23fae-179">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="23fae-180">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="23fae-180">sectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="23fae-181">Leia as propriedades e as relações do grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="23fae-181">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="23fae-182">Criar grupo de seções</span><span class="sxs-lookup"><span data-stu-id="23fae-182">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="23fae-183">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="23fae-183">sectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="23fae-184">Crie um grupo de seção postando na coleção sectionGroups no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="23fae-184">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="23fae-185">List section groups</span><span class="sxs-lookup"><span data-stu-id="23fae-185">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="23fae-186">coleção de [seções](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="23fae-186">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="23fae-187">Obtém a coleção de grupos de seção no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="23fae-187">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="23fae-188">Criar seção</span><span class="sxs-lookup"><span data-stu-id="23fae-188">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="23fae-189">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="23fae-189">onenoteSection</span></span>](onenotesection.md)| <span data-ttu-id="23fae-190">Crie uma seção postando na coleção Sections no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="23fae-190">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="23fae-191">Listar seções</span><span class="sxs-lookup"><span data-stu-id="23fae-191">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="23fae-192">coleção [onenoteSection](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="23fae-192">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="23fae-193">Obter uma coleção de seções no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="23fae-193">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


