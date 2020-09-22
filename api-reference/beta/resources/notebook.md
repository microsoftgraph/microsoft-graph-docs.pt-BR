---
title: tipo de recurso Notebook
description: Um bloco de anotações do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 1fff6f16c111d8036eae5fcb1705d7e5b59d7893
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078322"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="966c2-103">tipo de recurso Notebook</span><span class="sxs-lookup"><span data-stu-id="966c2-103">notebook resource type</span></span>

<span data-ttu-id="966c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="966c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="966c2-105">Um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="966c2-105">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="966c2-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="966c2-106">JSON representation</span></span>

<span data-ttu-id="966c2-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="966c2-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
## <a name="properties"></a><span data-ttu-id="966c2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="966c2-108">Properties</span></span>
| <span data-ttu-id="966c2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="966c2-109">Property</span></span>     | <span data-ttu-id="966c2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="966c2-110">Type</span></span>   |<span data-ttu-id="966c2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="966c2-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="966c2-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="966c2-112">createdBy</span></span>|[<span data-ttu-id="966c2-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="966c2-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="966c2-p101">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="966c2-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="966c2-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="966c2-116">createdDateTime</span></span>|<span data-ttu-id="966c2-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="966c2-117">DateTimeOffset</span></span>|<span data-ttu-id="966c2-118">A data e a hora em que o bloco de anotações foi criado.</span><span class="sxs-lookup"><span data-stu-id="966c2-118">The date and time when the notebook was created.</span></span> <span data-ttu-id="966c2-119">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="966c2-119">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="966c2-120">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="966c2-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="966c2-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="966c2-121">Read-only.</span></span>|
|<span data-ttu-id="966c2-122">id</span><span class="sxs-lookup"><span data-stu-id="966c2-122">id</span></span>|<span data-ttu-id="966c2-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="966c2-123">String</span></span>|<span data-ttu-id="966c2-124">O identificador exclusivo do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="966c2-124">The unique identifier of the notebook.</span></span> <span data-ttu-id="966c2-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="966c2-125">Read-only.</span></span>|
|<span data-ttu-id="966c2-126">isDefault</span><span class="sxs-lookup"><span data-stu-id="966c2-126">isDefault</span></span>|<span data-ttu-id="966c2-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="966c2-127">Boolean</span></span>|<span data-ttu-id="966c2-128">Indica se este é o bloco de anotações padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="966c2-128">Indicates whether this is the user's default notebook.</span></span> <span data-ttu-id="966c2-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="966c2-129">Read-only.</span></span>|
|<span data-ttu-id="966c2-130">isShared</span><span class="sxs-lookup"><span data-stu-id="966c2-130">isShared</span></span>|<span data-ttu-id="966c2-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="966c2-131">Boolean</span></span>|<span data-ttu-id="966c2-132">Indica se o bloco de anotações é compartilhado.</span><span class="sxs-lookup"><span data-stu-id="966c2-132">Indicates whether the notebook is shared.</span></span> <span data-ttu-id="966c2-133">Se for true, o conteúdo do bloco de anotações poderá ser visto por pessoas que não o proprietário.</span><span class="sxs-lookup"><span data-stu-id="966c2-133">If true, the contents of the notebook can be seen by people other than the owner.</span></span> <span data-ttu-id="966c2-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="966c2-134">Read-only.</span></span>|
|<span data-ttu-id="966c2-135">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="966c2-135">lastModifiedBy</span></span>|[<span data-ttu-id="966c2-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="966c2-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="966c2-p106">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="966c2-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="966c2-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="966c2-139">lastModifiedDateTime</span></span>|<span data-ttu-id="966c2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="966c2-140">DateTimeOffset</span></span>|<span data-ttu-id="966c2-141">A data e hora da última modificação do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="966c2-141">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="966c2-142">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="966c2-142">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="966c2-143">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="966c2-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="966c2-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="966c2-144">Read-only.</span></span>|
|<span data-ttu-id="966c2-145">links</span><span class="sxs-lookup"><span data-stu-id="966c2-145">links</span></span>|[<span data-ttu-id="966c2-146">notebookLinks</span><span class="sxs-lookup"><span data-stu-id="966c2-146">notebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="966c2-147">Links para abrir o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="966c2-147">Links for opening the notebook.</span></span> <span data-ttu-id="966c2-148">O `oneNoteClientURL` link abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="966c2-148">The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed.</span></span> <span data-ttu-id="966c2-149">O `oneNoteWebURL` link abre o bloco de anotações no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="966c2-149">The `oneNoteWebURL` link opens the notebook in OneNote on the web.</span></span>|
|<span data-ttu-id="966c2-150">displayName</span><span class="sxs-lookup"><span data-stu-id="966c2-150">displayName</span></span>|<span data-ttu-id="966c2-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="966c2-151">String</span></span>|<span data-ttu-id="966c2-152">O nome do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="966c2-152">The name of the notebook.</span></span>|
|<span data-ttu-id="966c2-153">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="966c2-153">sectionGroupsUrl</span></span>|<span data-ttu-id="966c2-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="966c2-154">String</span></span>|<span data-ttu-id="966c2-155">A URL da `sectionGroups` propriedade de navegação, que retorna todos os grupos de seção no bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="966c2-155">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook.</span></span> <span data-ttu-id="966c2-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="966c2-156">Read-only.</span></span>|
|<span data-ttu-id="966c2-157">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="966c2-157">sectionsUrl</span></span>|<span data-ttu-id="966c2-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="966c2-158">String</span></span>|<span data-ttu-id="966c2-159">A URL da `sections` propriedade de navegação, que retorna todas as seções do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="966c2-159">The URL for the `sections` navigation property, which returns all the sections in the notebook.</span></span> <span data-ttu-id="966c2-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="966c2-160">Read-only.</span></span>|
|<span data-ttu-id="966c2-161">própria</span><span class="sxs-lookup"><span data-stu-id="966c2-161">self</span></span>|<span data-ttu-id="966c2-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="966c2-162">String</span></span>|<span data-ttu-id="966c2-163">O ponto de extremidade onde você pode obter detalhes sobre o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="966c2-163">The endpoint where you can get details about the notebook.</span></span> <span data-ttu-id="966c2-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="966c2-164">Read-only.</span></span>|
|<span data-ttu-id="966c2-165">userRole</span><span class="sxs-lookup"><span data-stu-id="966c2-165">userRole</span></span>|<span data-ttu-id="966c2-166">String</span><span class="sxs-lookup"><span data-stu-id="966c2-166">String</span></span>|<span data-ttu-id="966c2-167">Os valores possíveis são: `Owner`, `Contributor`, `Reader`, `None`.</span><span class="sxs-lookup"><span data-stu-id="966c2-167">Possible values are: `Owner`, `Contributor`, `Reader`, `None`.</span></span> <span data-ttu-id="966c2-168">O proprietário representa o acesso no nível do proprietário ao bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="966c2-168">Owner represents owner-level access to the notebook.</span></span> <span data-ttu-id="966c2-169">O colaborador representa acesso de leitura/gravação ao bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="966c2-169">Contributor represents read/write access to the notebook.</span></span> <span data-ttu-id="966c2-170">O leitor representa acesso somente leitura ao bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="966c2-170">Reader represents read-only access to the notebook.</span></span> <span data-ttu-id="966c2-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="966c2-171">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="966c2-172">Relações</span><span class="sxs-lookup"><span data-stu-id="966c2-172">Relationships</span></span>
| <span data-ttu-id="966c2-173">Relação</span><span class="sxs-lookup"><span data-stu-id="966c2-173">Relationship</span></span> | <span data-ttu-id="966c2-174">Tipo</span><span class="sxs-lookup"><span data-stu-id="966c2-174">Type</span></span>   |<span data-ttu-id="966c2-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="966c2-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="966c2-176">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="966c2-176">sectionGroups</span></span>|<span data-ttu-id="966c2-177">coleção de [seções](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="966c2-177">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="966c2-178">Obtém os grupos de seção no bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="966c2-178">The section groups in the notebook.</span></span> <span data-ttu-id="966c2-179">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="966c2-179">Read-only.</span></span> <span data-ttu-id="966c2-180">Anulável.</span><span class="sxs-lookup"><span data-stu-id="966c2-180">Nullable.</span></span>|
|<span data-ttu-id="966c2-181">seções</span><span class="sxs-lookup"><span data-stu-id="966c2-181">sections</span></span>|<span data-ttu-id="966c2-182">coleção [onenoteSection](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="966c2-182">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="966c2-183">As seções no bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="966c2-183">The sections in the notebook.</span></span> <span data-ttu-id="966c2-184">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="966c2-184">Read-only.</span></span> <span data-ttu-id="966c2-185">Anulável.</span><span class="sxs-lookup"><span data-stu-id="966c2-185">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="966c2-186">Métodos</span><span class="sxs-lookup"><span data-stu-id="966c2-186">Methods</span></span>

| <span data-ttu-id="966c2-187">Método</span><span class="sxs-lookup"><span data-stu-id="966c2-187">Method</span></span>           | <span data-ttu-id="966c2-188">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="966c2-188">Return Type</span></span>    |<span data-ttu-id="966c2-189">Descrição</span><span class="sxs-lookup"><span data-stu-id="966c2-189">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="966c2-190">Obter bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="966c2-190">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="966c2-191">bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="966c2-191">notebook</span></span>](notebook.md) |<span data-ttu-id="966c2-192">Leia as propriedades e as relações do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="966c2-192">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="966c2-193">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="966c2-193">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="966c2-194">coleção [recentNotebook](recentnotebook.md)</span><span class="sxs-lookup"><span data-stu-id="966c2-194">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="966c2-195">Obtenha uma coleção de blocos de anotações acessados mais recentemente para o usuário.</span><span class="sxs-lookup"><span data-stu-id="966c2-195">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="966c2-196">getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="966c2-196">getNotebookFromWebUrl</span></span>](../api/notebook-getnotebookfromweburl.md) | [<span data-ttu-id="966c2-197">bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="966c2-197">notebook</span></span>](notebook.md) | <span data-ttu-id="966c2-198">Recupere as propriedades e os relacionamentos de um objeto Notebook usando seu caminho de URL.</span><span class="sxs-lookup"><span data-stu-id="966c2-198">Retrieve the properties and relationships of a notebook object using its URL path.</span></span> |
|[<span data-ttu-id="966c2-199">Criar grupo de seções</span><span class="sxs-lookup"><span data-stu-id="966c2-199">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="966c2-200">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="966c2-200">sectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="966c2-201">Criar um grupo de seção postando na coleção sectionGroups no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="966c2-201">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="966c2-202">List section groups</span><span class="sxs-lookup"><span data-stu-id="966c2-202">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="966c2-203">coleção de [seções](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="966c2-203">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="966c2-204">Obtém uma coleção de grupos de seções no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="966c2-204">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="966c2-205">Criar seção</span><span class="sxs-lookup"><span data-stu-id="966c2-205">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="966c2-206">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="966c2-206">onenoteSection</span></span>](onenotesection.md)| <span data-ttu-id="966c2-207">Criar uma seção postando na coleção Sections no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="966c2-207">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="966c2-208">Listar seções</span><span class="sxs-lookup"><span data-stu-id="966c2-208">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="966c2-209">coleção [onenoteSection](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="966c2-209">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="966c2-210">Obtém uma coleção de seções no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="966c2-210">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="966c2-211">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="966c2-211">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="966c2-212">Nenhum</span><span class="sxs-lookup"><span data-stu-id="966c2-212">None</span></span> | <span data-ttu-id="966c2-213">Copia um bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="966c2-213">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


