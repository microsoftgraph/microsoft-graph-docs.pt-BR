---
title: tipo de recurso de bloco de anotações
description: Um bloco de anotações do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: c52108e415388d8e4e919709fd619660c531aef8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960371"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="53344-103">tipo de recurso de bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="53344-103">notebook resource type</span></span>

<span data-ttu-id="53344-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53344-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53344-105">Um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="53344-105">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="53344-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53344-106">JSON representation</span></span>

<span data-ttu-id="53344-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="53344-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="53344-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53344-108">Properties</span></span>
| <span data-ttu-id="53344-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53344-109">Property</span></span>     | <span data-ttu-id="53344-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="53344-110">Type</span></span>   |<span data-ttu-id="53344-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="53344-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53344-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="53344-112">createdBy</span></span>|[<span data-ttu-id="53344-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="53344-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="53344-p101">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53344-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="53344-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53344-116">createdDateTime</span></span>|<span data-ttu-id="53344-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53344-117">DateTimeOffset</span></span>|<span data-ttu-id="53344-118">A data e a hora em que o bloco de anotações foi criado.</span><span class="sxs-lookup"><span data-stu-id="53344-118">The date and time when the notebook was created.</span></span> <span data-ttu-id="53344-119">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="53344-119">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="53344-120">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="53344-120">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="53344-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53344-121">Read-only.</span></span>|
|<span data-ttu-id="53344-122">id</span><span class="sxs-lookup"><span data-stu-id="53344-122">id</span></span>|<span data-ttu-id="53344-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53344-123">String</span></span>|<span data-ttu-id="53344-124">O identificador exclusivo do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="53344-124">The unique identifier of the notebook.</span></span> <span data-ttu-id="53344-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53344-125">Read-only.</span></span>|
|<span data-ttu-id="53344-126">isDefault</span><span class="sxs-lookup"><span data-stu-id="53344-126">isDefault</span></span>|<span data-ttu-id="53344-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="53344-127">Boolean</span></span>|<span data-ttu-id="53344-128">Indica se esse é o bloco de anotações padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="53344-128">Indicates whether this is the user's default notebook.</span></span> <span data-ttu-id="53344-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53344-129">Read-only.</span></span>|
|<span data-ttu-id="53344-130">isShared</span><span class="sxs-lookup"><span data-stu-id="53344-130">isShared</span></span>|<span data-ttu-id="53344-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="53344-131">Boolean</span></span>|<span data-ttu-id="53344-132">Indica se o bloco de anotações é compartilhado.</span><span class="sxs-lookup"><span data-stu-id="53344-132">Indicates whether the notebook is shared.</span></span> <span data-ttu-id="53344-133">Se for verdadeiro, o conteúdo do bloco de anotações poderá ser visto por pessoas que não sejam o proprietário.</span><span class="sxs-lookup"><span data-stu-id="53344-133">If true, the contents of the notebook can be seen by people other than the owner.</span></span> <span data-ttu-id="53344-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53344-134">Read-only.</span></span>|
|<span data-ttu-id="53344-135">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="53344-135">lastModifiedBy</span></span>|[<span data-ttu-id="53344-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="53344-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="53344-p106">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53344-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="53344-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53344-139">lastModifiedDateTime</span></span>|<span data-ttu-id="53344-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53344-140">DateTimeOffset</span></span>|<span data-ttu-id="53344-141">A data e hora da última modificação do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="53344-141">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="53344-142">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="53344-142">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="53344-143">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="53344-143">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="53344-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53344-144">Read-only.</span></span>|
|<span data-ttu-id="53344-145">links</span><span class="sxs-lookup"><span data-stu-id="53344-145">links</span></span>|[<span data-ttu-id="53344-146">notebookLinks</span><span class="sxs-lookup"><span data-stu-id="53344-146">notebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="53344-147">Links para abrir o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="53344-147">Links for opening the notebook.</span></span> <span data-ttu-id="53344-148">O `oneNoteClientURL` link abre o bloco de anotações no cliente nativo do OneNote se estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="53344-148">The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed.</span></span> <span data-ttu-id="53344-149">O `oneNoteWebURL` link abre o bloco de anotações no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="53344-149">The `oneNoteWebURL` link opens the notebook in OneNote on the web.</span></span>|
|<span data-ttu-id="53344-150">displayName</span><span class="sxs-lookup"><span data-stu-id="53344-150">displayName</span></span>|<span data-ttu-id="53344-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53344-151">String</span></span>|<span data-ttu-id="53344-152">O nome do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="53344-152">The name of the notebook.</span></span>|
|<span data-ttu-id="53344-153">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="53344-153">sectionGroupsUrl</span></span>|<span data-ttu-id="53344-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53344-154">String</span></span>|<span data-ttu-id="53344-155">A URL da `sectionGroups` propriedade de navegação, que retorna todos os grupos de seções no bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="53344-155">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook.</span></span> <span data-ttu-id="53344-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53344-156">Read-only.</span></span>|
|<span data-ttu-id="53344-157">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="53344-157">sectionsUrl</span></span>|<span data-ttu-id="53344-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53344-158">String</span></span>|<span data-ttu-id="53344-159">A URL da `sections` propriedade de navegação, que retorna todas as seções no bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="53344-159">The URL for the `sections` navigation property, which returns all the sections in the notebook.</span></span> <span data-ttu-id="53344-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53344-160">Read-only.</span></span>|
|<span data-ttu-id="53344-161">self</span><span class="sxs-lookup"><span data-stu-id="53344-161">self</span></span>|<span data-ttu-id="53344-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53344-162">String</span></span>|<span data-ttu-id="53344-163">O ponto de extremidade onde você pode obter detalhes sobre o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="53344-163">The endpoint where you can get details about the notebook.</span></span> <span data-ttu-id="53344-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53344-164">Read-only.</span></span>|
|<span data-ttu-id="53344-165">userRole</span><span class="sxs-lookup"><span data-stu-id="53344-165">userRole</span></span>|<span data-ttu-id="53344-166">onenoteUserRole</span><span class="sxs-lookup"><span data-stu-id="53344-166">onenoteUserRole</span></span>|<span data-ttu-id="53344-167">Os valores possíveis são: `Owner`, `Contributor`, `Reader`, `None`.</span><span class="sxs-lookup"><span data-stu-id="53344-167">Possible values are: `Owner`, `Contributor`, `Reader`, `None`.</span></span> <span data-ttu-id="53344-168">O proprietário representa o acesso no nível do proprietário ao bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="53344-168">Owner represents owner-level access to the notebook.</span></span> <span data-ttu-id="53344-169">Colaborador representa o acesso de leitura/gravação ao bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="53344-169">Contributor represents read/write access to the notebook.</span></span> <span data-ttu-id="53344-170">O leitor representa o acesso somente leitura ao bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="53344-170">Reader represents read-only access to the notebook.</span></span> <span data-ttu-id="53344-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53344-171">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53344-172">Relações</span><span class="sxs-lookup"><span data-stu-id="53344-172">Relationships</span></span>
| <span data-ttu-id="53344-173">Relação</span><span class="sxs-lookup"><span data-stu-id="53344-173">Relationship</span></span> | <span data-ttu-id="53344-174">Tipo</span><span class="sxs-lookup"><span data-stu-id="53344-174">Type</span></span>   |<span data-ttu-id="53344-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="53344-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53344-176">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="53344-176">sectionGroups</span></span>|<span data-ttu-id="53344-177">[coleção sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="53344-177">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="53344-178">Obtém os grupos de seção no bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="53344-178">The section groups in the notebook.</span></span> <span data-ttu-id="53344-179">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53344-179">Read-only.</span></span> <span data-ttu-id="53344-180">Anulável.</span><span class="sxs-lookup"><span data-stu-id="53344-180">Nullable.</span></span>|
|<span data-ttu-id="53344-181">seções</span><span class="sxs-lookup"><span data-stu-id="53344-181">sections</span></span>|<span data-ttu-id="53344-182">[Coleção onenoteSection](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="53344-182">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="53344-183">As seções no bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="53344-183">The sections in the notebook.</span></span> <span data-ttu-id="53344-184">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53344-184">Read-only.</span></span> <span data-ttu-id="53344-185">Anulável.</span><span class="sxs-lookup"><span data-stu-id="53344-185">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="53344-186">Métodos</span><span class="sxs-lookup"><span data-stu-id="53344-186">Methods</span></span>

| <span data-ttu-id="53344-187">Método</span><span class="sxs-lookup"><span data-stu-id="53344-187">Method</span></span>           | <span data-ttu-id="53344-188">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="53344-188">Return Type</span></span>    |<span data-ttu-id="53344-189">Descrição</span><span class="sxs-lookup"><span data-stu-id="53344-189">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="53344-190">Obter bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="53344-190">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="53344-191">bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="53344-191">notebook</span></span>](notebook.md) |<span data-ttu-id="53344-192">Leia as propriedades e as relações do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="53344-192">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="53344-193">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="53344-193">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="53344-194">[coleção recentNotebook](recentnotebook.md)</span><span class="sxs-lookup"><span data-stu-id="53344-194">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="53344-195">Obtenha uma coleção de blocos de anotações acessados mais recentemente para o usuário.</span><span class="sxs-lookup"><span data-stu-id="53344-195">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="53344-196">getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="53344-196">getNotebookFromWebUrl</span></span>](../api/notebook-getnotebookfromweburl.md) | [<span data-ttu-id="53344-197">bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="53344-197">notebook</span></span>](notebook.md) | <span data-ttu-id="53344-198">Recupere as propriedades e as relações de um objeto de bloco de anotações usando seu caminho de URL.</span><span class="sxs-lookup"><span data-stu-id="53344-198">Retrieve the properties and relationships of a notebook object using its URL path.</span></span> |
|[<span data-ttu-id="53344-199">Criar grupo de seções</span><span class="sxs-lookup"><span data-stu-id="53344-199">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="53344-200">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="53344-200">sectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="53344-201">Crie um grupo de seções postando na coleção sectionGroups no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="53344-201">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="53344-202">List section groups</span><span class="sxs-lookup"><span data-stu-id="53344-202">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="53344-203">[coleção sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="53344-203">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="53344-204">Obter uma coleção de grupos de seções no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="53344-204">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="53344-205">Criar seção</span><span class="sxs-lookup"><span data-stu-id="53344-205">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="53344-206">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="53344-206">onenoteSection</span></span>](onenotesection.md)| <span data-ttu-id="53344-207">Crie uma seção postando na coleção sections no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="53344-207">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="53344-208">Listar seções</span><span class="sxs-lookup"><span data-stu-id="53344-208">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="53344-209">[Coleção onenoteSection](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="53344-209">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="53344-210">Obter uma coleção de seções no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="53344-210">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="53344-211">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="53344-211">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="53344-212">Nenhum</span><span class="sxs-lookup"><span data-stu-id="53344-212">None</span></span> | <span data-ttu-id="53344-213">Copia um bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="53344-213">Copies a notebook.</span></span>|

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


