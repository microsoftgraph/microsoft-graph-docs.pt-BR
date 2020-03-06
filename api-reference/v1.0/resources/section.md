---
title: tipo de recurso Section
description: Uma seção em um bloco de anotações do OneNote. As seções podem conter páginas.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a701fbe2cea27db97bb7d95911c0c0ee1140b55c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533782"
---
# <a name="section-resource-type"></a><span data-ttu-id="acb6e-104">tipo de recurso Section</span><span class="sxs-lookup"><span data-stu-id="acb6e-104">section resource type</span></span>

<span data-ttu-id="acb6e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acb6e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="acb6e-106">Uma seção em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="acb6e-106">A section in a OneNote notebook.</span></span> <span data-ttu-id="acb6e-107">As seções podem conter páginas.</span><span class="sxs-lookup"><span data-stu-id="acb6e-107">Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="acb6e-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="acb6e-108">JSON representation</span></span>

<span data-ttu-id="acb6e-109">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="acb6e-109">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
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
## <a name="properties"></a><span data-ttu-id="acb6e-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="acb6e-110">Properties</span></span>
| <span data-ttu-id="acb6e-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acb6e-111">Property</span></span>     | <span data-ttu-id="acb6e-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="acb6e-112">Type</span></span>   |<span data-ttu-id="acb6e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="acb6e-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acb6e-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="acb6e-114">createdBy</span></span>|[<span data-ttu-id="acb6e-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="acb6e-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="acb6e-p103">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6e-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="acb6e-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="acb6e-118">createdDateTime</span></span>|<span data-ttu-id="acb6e-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acb6e-119">DateTimeOffset</span></span>|<span data-ttu-id="acb6e-120">A data e a hora em que a seção foi criada.</span><span class="sxs-lookup"><span data-stu-id="acb6e-120">The date and time when the section was created.</span></span> <span data-ttu-id="acb6e-121">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="acb6e-121">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="acb6e-122">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="acb6e-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="acb6e-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6e-123">Read-only.</span></span>|
|<span data-ttu-id="acb6e-124">id</span><span class="sxs-lookup"><span data-stu-id="acb6e-124">id</span></span>|<span data-ttu-id="acb6e-125">String</span><span class="sxs-lookup"><span data-stu-id="acb6e-125">String</span></span>|<span data-ttu-id="acb6e-126">O identificador exclusivo da seção.</span><span class="sxs-lookup"><span data-stu-id="acb6e-126">The unique identifier of the section.</span></span>  <span data-ttu-id="acb6e-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6e-127">Read-only.</span></span>|
|<span data-ttu-id="acb6e-128">isDefault</span><span class="sxs-lookup"><span data-stu-id="acb6e-128">isDefault</span></span>|<span data-ttu-id="acb6e-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="acb6e-129">Boolean</span></span>|<span data-ttu-id="acb6e-130">Indica se esta é a seção padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="acb6e-130">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="acb6e-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6e-131">Read-only.</span></span>|
|<span data-ttu-id="acb6e-132">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="acb6e-132">lastModifiedBy</span></span>|[<span data-ttu-id="acb6e-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="acb6e-133">identitySet</span></span>](identityset.md)|<span data-ttu-id="acb6e-p107">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6e-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="acb6e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="acb6e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="acb6e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acb6e-137">DateTimeOffset</span></span>|<span data-ttu-id="acb6e-138">A data e a hora em que a seção foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="acb6e-138">The date and time when the section was last modified.</span></span> <span data-ttu-id="acb6e-139">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="acb6e-139">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="acb6e-140">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="acb6e-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="acb6e-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6e-141">Read-only.</span></span>|
|<span data-ttu-id="acb6e-142">links</span><span class="sxs-lookup"><span data-stu-id="acb6e-142">links</span></span>|[<span data-ttu-id="acb6e-143">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="acb6e-143">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="acb6e-144">Links para abrir a seção.</span><span class="sxs-lookup"><span data-stu-id="acb6e-144">Links for opening the section.</span></span> <span data-ttu-id="acb6e-145">O `oneNoteClientURL` link abre a seção no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="acb6e-145">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="acb6e-146">O `oneNoteWebURL` link abre a seção no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="acb6e-146">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="acb6e-147">displayName</span><span class="sxs-lookup"><span data-stu-id="acb6e-147">displayName</span></span>|<span data-ttu-id="acb6e-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="acb6e-148">String</span></span>|<span data-ttu-id="acb6e-149">O nome da seção.</span><span class="sxs-lookup"><span data-stu-id="acb6e-149">The name of the section.</span></span> |
|<span data-ttu-id="acb6e-150">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="acb6e-150">pagesUrl</span></span>|<span data-ttu-id="acb6e-151">String</span><span class="sxs-lookup"><span data-stu-id="acb6e-151">String</span></span>|<span data-ttu-id="acb6e-152">O `pages` ponto de extremidade onde você pode obter detalhes de todas as páginas da seção.</span><span class="sxs-lookup"><span data-stu-id="acb6e-152">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="acb6e-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6e-153">Read-only.</span></span>|
|<span data-ttu-id="acb6e-154">própria</span><span class="sxs-lookup"><span data-stu-id="acb6e-154">self</span></span>|<span data-ttu-id="acb6e-155">String</span><span class="sxs-lookup"><span data-stu-id="acb6e-155">String</span></span>|<span data-ttu-id="acb6e-156">O ponto de extremidade onde você pode obter detalhes sobre a seção.</span><span class="sxs-lookup"><span data-stu-id="acb6e-156">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="acb6e-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6e-157">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="acb6e-158">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="acb6e-158">Relationships</span></span>
| <span data-ttu-id="acb6e-159">Relação</span><span class="sxs-lookup"><span data-stu-id="acb6e-159">Relationship</span></span> | <span data-ttu-id="acb6e-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="acb6e-160">Type</span></span>   |<span data-ttu-id="acb6e-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="acb6e-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acb6e-162">páginas</span><span class="sxs-lookup"><span data-stu-id="acb6e-162">pages</span></span>|<span data-ttu-id="acb6e-163">Coleção [OnenotePage](page.md) </span><span class="sxs-lookup"><span data-stu-id="acb6e-163">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="acb6e-164">Obtém o conjunto de páginas da seção.</span><span class="sxs-lookup"><span data-stu-id="acb6e-164">The collection of pages in the section.</span></span>  <span data-ttu-id="acb6e-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6e-165">Read-only.</span></span> <span data-ttu-id="acb6e-166">Anulável.</span><span class="sxs-lookup"><span data-stu-id="acb6e-166">Nullable.</span></span>|
|<span data-ttu-id="acb6e-167">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="acb6e-167">parentNotebook</span></span>|[<span data-ttu-id="acb6e-168">Notebook</span><span class="sxs-lookup"><span data-stu-id="acb6e-168">Notebook</span></span>](notebook.md)|<span data-ttu-id="acb6e-169">O bloco de anotações que contém a seção.</span><span class="sxs-lookup"><span data-stu-id="acb6e-169">The notebook that contains the section.</span></span>  <span data-ttu-id="acb6e-170">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6e-170">Read-only.</span></span>|
|<span data-ttu-id="acb6e-171">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="acb6e-171">parentSectionGroup</span></span>|[<span data-ttu-id="acb6e-172">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="acb6e-172">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="acb6e-173">O grupo de seções que contém a seção.</span><span class="sxs-lookup"><span data-stu-id="acb6e-173">The section group that contains the section.</span></span>  <span data-ttu-id="acb6e-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6e-174">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="acb6e-175">Métodos</span><span class="sxs-lookup"><span data-stu-id="acb6e-175">Methods</span></span>

| <span data-ttu-id="acb6e-176">Método</span><span class="sxs-lookup"><span data-stu-id="acb6e-176">Method</span></span>           | <span data-ttu-id="acb6e-177">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="acb6e-177">Return Type</span></span>    |<span data-ttu-id="acb6e-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="acb6e-178">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="acb6e-179">Obter seção</span><span class="sxs-lookup"><span data-stu-id="acb6e-179">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="acb6e-180">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="acb6e-180">OnenoteSection</span></span>](section.md) |<span data-ttu-id="acb6e-181">Leia as propriedades e as relações da seção.</span><span class="sxs-lookup"><span data-stu-id="acb6e-181">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="acb6e-182">Create page</span><span class="sxs-lookup"><span data-stu-id="acb6e-182">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="acb6e-183">Page</span><span class="sxs-lookup"><span data-stu-id="acb6e-183">Page</span></span>](page.md)| <span data-ttu-id="acb6e-184">Crie uma página postando na coleção Pages na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="acb6e-184">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="acb6e-185">List pages</span><span class="sxs-lookup"><span data-stu-id="acb6e-185">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="acb6e-186">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="acb6e-186">[Page](page.md) collection</span></span>| <span data-ttu-id="acb6e-187">Obtém uma coleção de páginas na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="acb6e-187">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="acb6e-188">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="acb6e-188">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="acb6e-189">Nenhum</span><span class="sxs-lookup"><span data-stu-id="acb6e-189">None</span></span>|<span data-ttu-id="acb6e-190">Copie a seção para um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="acb6e-190">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="acb6e-191">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="acb6e-191">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="acb6e-192">Nenhum</span><span class="sxs-lookup"><span data-stu-id="acb6e-192">None</span></span>|<span data-ttu-id="acb6e-193">Copie a seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="acb6e-193">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
