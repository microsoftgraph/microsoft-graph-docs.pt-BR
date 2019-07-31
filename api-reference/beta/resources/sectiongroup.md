---
title: tipo de recurso de @ @ @ Section
description: Um grupo de seções em um bloco de anotações do OneNote. Os grupos de seções podem conter seções e grupos de seções.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 4637784ac20d92c82e7a4771c815136ddd3e175a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965268"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="22a46-104">tipo de recurso de @ @ @ Section</span><span class="sxs-lookup"><span data-stu-id="22a46-104">sectionGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22a46-105">Um grupo de seções em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="22a46-105">A section group in a OneNote notebook.</span></span> <span data-ttu-id="22a46-106">Os grupos de seções podem conter seções e grupos de seções.</span><span class="sxs-lookup"><span data-stu-id="22a46-106">Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="22a46-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22a46-107">JSON representation</span></span>

<span data-ttu-id="22a46-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="22a46-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="22a46-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22a46-109">Properties</span></span>
| <span data-ttu-id="22a46-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22a46-110">Property</span></span>     | <span data-ttu-id="22a46-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="22a46-111">Type</span></span>   |<span data-ttu-id="22a46-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="22a46-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22a46-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="22a46-113">createdBy</span></span>|[<span data-ttu-id="22a46-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="22a46-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="22a46-p103">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22a46-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="22a46-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22a46-117">createdDateTime</span></span>|<span data-ttu-id="22a46-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22a46-118">DateTimeOffset</span></span>|<span data-ttu-id="22a46-119">A data e a hora em que o grupo de seções foi criado.</span><span class="sxs-lookup"><span data-stu-id="22a46-119">The date and time when the section group was created.</span></span> <span data-ttu-id="22a46-120">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="22a46-120">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="22a46-121">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="22a46-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="22a46-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22a46-122">Read-only.</span></span>|
|<span data-ttu-id="22a46-123">id</span><span class="sxs-lookup"><span data-stu-id="22a46-123">id</span></span>|<span data-ttu-id="22a46-124">String</span><span class="sxs-lookup"><span data-stu-id="22a46-124">String</span></span>|<span data-ttu-id="22a46-125">O identificador exclusivo do grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="22a46-125">The unique identifier of the section group.</span></span> <span data-ttu-id="22a46-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22a46-126">Read-only.</span></span>|
|<span data-ttu-id="22a46-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="22a46-127">lastModifiedBy</span></span>|[<span data-ttu-id="22a46-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="22a46-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="22a46-p106">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22a46-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="22a46-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22a46-131">lastModifiedDateTime</span></span>|<span data-ttu-id="22a46-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22a46-132">DateTimeOffset</span></span>|<span data-ttu-id="22a46-133">A data e a hora em que o grupo de seções foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="22a46-133">The date and time when the section group was last modified.</span></span> <span data-ttu-id="22a46-134">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="22a46-134">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="22a46-135">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="22a46-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="22a46-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22a46-136">Read-only.</span></span>|
|<span data-ttu-id="22a46-137">displayName</span><span class="sxs-lookup"><span data-stu-id="22a46-137">displayName</span></span>|<span data-ttu-id="22a46-138">String</span><span class="sxs-lookup"><span data-stu-id="22a46-138">String</span></span>|<span data-ttu-id="22a46-139">O nome do grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="22a46-139">The name of the section group.</span></span>|
|<span data-ttu-id="22a46-140">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="22a46-140">sectionGroupsUrl</span></span>|<span data-ttu-id="22a46-141">String</span><span class="sxs-lookup"><span data-stu-id="22a46-141">String</span></span>|<span data-ttu-id="22a46-142">A URL da propriedade `sectionGroups` de navegação, que retorna todos os grupos de seção no grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="22a46-142">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group.</span></span> <span data-ttu-id="22a46-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22a46-143">Read-only.</span></span>|
|<span data-ttu-id="22a46-144">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="22a46-144">sectionsUrl</span></span>|<span data-ttu-id="22a46-145">String</span><span class="sxs-lookup"><span data-stu-id="22a46-145">String</span></span>|<span data-ttu-id="22a46-146">A URL da propriedade `sections` de navegação, que retorna todas as seções no grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="22a46-146">The URL for the `sections` navigation property, which returns all the sections in the section group.</span></span> <span data-ttu-id="22a46-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22a46-147">Read-only.</span></span>|
|<span data-ttu-id="22a46-148">própria</span><span class="sxs-lookup"><span data-stu-id="22a46-148">self</span></span>|<span data-ttu-id="22a46-149">String</span><span class="sxs-lookup"><span data-stu-id="22a46-149">String</span></span>|<span data-ttu-id="22a46-150">O ponto de extremidade onde você pode obter detalhes sobre o grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="22a46-150">The endpoint where you can get details about the section group.</span></span> <span data-ttu-id="22a46-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22a46-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22a46-152">Relações</span><span class="sxs-lookup"><span data-stu-id="22a46-152">Relationships</span></span>
| <span data-ttu-id="22a46-153">Relação</span><span class="sxs-lookup"><span data-stu-id="22a46-153">Relationship</span></span> | <span data-ttu-id="22a46-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="22a46-154">Type</span></span>   |<span data-ttu-id="22a46-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="22a46-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22a46-156">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="22a46-156">parentNotebook</span></span>|[<span data-ttu-id="22a46-157">anotações</span><span class="sxs-lookup"><span data-stu-id="22a46-157">notebook</span></span>](notebook.md)|<span data-ttu-id="22a46-158">O bloco de anotações que contém o grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="22a46-158">The notebook that contains the section group.</span></span> <span data-ttu-id="22a46-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22a46-159">Read-only.</span></span>|
|<span data-ttu-id="22a46-160">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="22a46-160">parentSectionGroup</span></span>|[<span data-ttu-id="22a46-161">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="22a46-161">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="22a46-162">O grupo de seções que contém o grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="22a46-162">The section group that contains the section group.</span></span> <span data-ttu-id="22a46-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22a46-163">Read-only.</span></span>|
|<span data-ttu-id="22a46-164">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="22a46-164">sectionGroups</span></span>|<span data-ttu-id="22a46-165">coleção de [seções](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="22a46-165">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="22a46-166">Os grupos de seção na seção.</span><span class="sxs-lookup"><span data-stu-id="22a46-166">The section groups in the section.</span></span> <span data-ttu-id="22a46-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22a46-167">Read-only.</span></span> <span data-ttu-id="22a46-168">Anulável.</span><span class="sxs-lookup"><span data-stu-id="22a46-168">Nullable.</span></span>|
|<span data-ttu-id="22a46-169">seções</span><span class="sxs-lookup"><span data-stu-id="22a46-169">sections</span></span>|<span data-ttu-id="22a46-170">coleção [onenoteSection](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="22a46-170">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="22a46-171">As seções no grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="22a46-171">The sections in the section group.</span></span> <span data-ttu-id="22a46-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22a46-172">Read-only.</span></span> <span data-ttu-id="22a46-173">Anulável.</span><span class="sxs-lookup"><span data-stu-id="22a46-173">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="22a46-174">Métodos</span><span class="sxs-lookup"><span data-stu-id="22a46-174">Methods</span></span>

| <span data-ttu-id="22a46-175">Método</span><span class="sxs-lookup"><span data-stu-id="22a46-175">Method</span></span>           | <span data-ttu-id="22a46-176">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="22a46-176">Return Type</span></span>    |<span data-ttu-id="22a46-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="22a46-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="22a46-178">Obter grupo de seções</span><span class="sxs-lookup"><span data-stu-id="22a46-178">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="22a46-179">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="22a46-179">sectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="22a46-180">Leia as propriedades e as relações do grupo de seções.</span><span class="sxs-lookup"><span data-stu-id="22a46-180">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="22a46-181">Criar grupo de seções</span><span class="sxs-lookup"><span data-stu-id="22a46-181">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="22a46-182">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="22a46-182">sectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="22a46-183">Crie um grupo de seção postando na coleção sectionGroups no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="22a46-183">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="22a46-184">List section groups</span><span class="sxs-lookup"><span data-stu-id="22a46-184">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="22a46-185">coleção de [seções](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="22a46-185">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="22a46-186">Obtém a coleção de grupos de seção no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="22a46-186">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="22a46-187">Criar seção</span><span class="sxs-lookup"><span data-stu-id="22a46-187">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="22a46-188">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="22a46-188">onenoteSection</span></span>](onenotesection.md)| <span data-ttu-id="22a46-189">Crie uma seção postando na coleção Sections no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="22a46-189">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="22a46-190">Listar seções</span><span class="sxs-lookup"><span data-stu-id="22a46-190">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="22a46-191">coleção [onenoteSection](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="22a46-191">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="22a46-192">Obter uma coleção de seções no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="22a46-192">Get a collection of sections in the specified section group.</span></span>|

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
