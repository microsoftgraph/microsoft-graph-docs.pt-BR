---
title: tipo de recurso Section
description: Uma seção em um bloco de anotações do OneNote. As seções podem conter páginas.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6cc87845b14b45dbe84377f1be917fe4b9f873ff
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812243"
---
# <a name="section-resource-type"></a><span data-ttu-id="14f3e-104">tipo de recurso Section</span><span class="sxs-lookup"><span data-stu-id="14f3e-104">section resource type</span></span>

<span data-ttu-id="14f3e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14f3e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="14f3e-106">Uma seção em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="14f3e-106">A section in a OneNote notebook.</span></span> <span data-ttu-id="14f3e-107">As seções podem conter páginas.</span><span class="sxs-lookup"><span data-stu-id="14f3e-107">Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="14f3e-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14f3e-108">JSON representation</span></span>

<span data-ttu-id="14f3e-109">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="14f3e-109">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="14f3e-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14f3e-110">Properties</span></span>
| <span data-ttu-id="14f3e-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14f3e-111">Property</span></span>     | <span data-ttu-id="14f3e-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="14f3e-112">Type</span></span>   |<span data-ttu-id="14f3e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="14f3e-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14f3e-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="14f3e-114">createdBy</span></span>|[<span data-ttu-id="14f3e-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="14f3e-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="14f3e-p103">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14f3e-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="14f3e-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14f3e-118">createdDateTime</span></span>|<span data-ttu-id="14f3e-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14f3e-119">DateTimeOffset</span></span>|<span data-ttu-id="14f3e-120">A data e a hora em que a seção foi criada.</span><span class="sxs-lookup"><span data-stu-id="14f3e-120">The date and time when the section was created.</span></span> <span data-ttu-id="14f3e-121">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="14f3e-121">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="14f3e-122">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="14f3e-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="14f3e-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14f3e-123">Read-only.</span></span>|
|<span data-ttu-id="14f3e-124">id</span><span class="sxs-lookup"><span data-stu-id="14f3e-124">id</span></span>|<span data-ttu-id="14f3e-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14f3e-125">String</span></span>|<span data-ttu-id="14f3e-126">O identificador exclusivo da seção.</span><span class="sxs-lookup"><span data-stu-id="14f3e-126">The unique identifier of the section.</span></span>  <span data-ttu-id="14f3e-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14f3e-127">Read-only.</span></span>|
|<span data-ttu-id="14f3e-128">isDefault</span><span class="sxs-lookup"><span data-stu-id="14f3e-128">isDefault</span></span>|<span data-ttu-id="14f3e-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="14f3e-129">Boolean</span></span>|<span data-ttu-id="14f3e-130">Indica se esta é a seção padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="14f3e-130">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="14f3e-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14f3e-131">Read-only.</span></span>|
|<span data-ttu-id="14f3e-132">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="14f3e-132">lastModifiedBy</span></span>|[<span data-ttu-id="14f3e-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="14f3e-133">identitySet</span></span>](identityset.md)|<span data-ttu-id="14f3e-p107">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14f3e-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="14f3e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14f3e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="14f3e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14f3e-137">DateTimeOffset</span></span>|<span data-ttu-id="14f3e-138">A data e a hora em que a seção foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="14f3e-138">The date and time when the section was last modified.</span></span> <span data-ttu-id="14f3e-139">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="14f3e-139">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="14f3e-140">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="14f3e-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="14f3e-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14f3e-141">Read-only.</span></span>|
|<span data-ttu-id="14f3e-142">links</span><span class="sxs-lookup"><span data-stu-id="14f3e-142">links</span></span>|[<span data-ttu-id="14f3e-143">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="14f3e-143">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="14f3e-144">Links para abrir a seção.</span><span class="sxs-lookup"><span data-stu-id="14f3e-144">Links for opening the section.</span></span> <span data-ttu-id="14f3e-145">O `oneNoteClientURL` link abre a seção no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="14f3e-145">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="14f3e-146">O `oneNoteWebURL` link abre a seção no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="14f3e-146">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="14f3e-147">displayName</span><span class="sxs-lookup"><span data-stu-id="14f3e-147">displayName</span></span>|<span data-ttu-id="14f3e-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14f3e-148">String</span></span>|<span data-ttu-id="14f3e-149">O nome da seção.</span><span class="sxs-lookup"><span data-stu-id="14f3e-149">The name of the section.</span></span> |
|<span data-ttu-id="14f3e-150">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="14f3e-150">pagesUrl</span></span>|<span data-ttu-id="14f3e-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14f3e-151">String</span></span>|<span data-ttu-id="14f3e-152">O `pages` ponto de extremidade onde você pode obter detalhes de todas as páginas da seção.</span><span class="sxs-lookup"><span data-stu-id="14f3e-152">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="14f3e-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14f3e-153">Read-only.</span></span>|
|<span data-ttu-id="14f3e-154">própria</span><span class="sxs-lookup"><span data-stu-id="14f3e-154">self</span></span>|<span data-ttu-id="14f3e-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14f3e-155">String</span></span>|<span data-ttu-id="14f3e-156">O ponto de extremidade onde você pode obter detalhes sobre a seção.</span><span class="sxs-lookup"><span data-stu-id="14f3e-156">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="14f3e-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14f3e-157">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14f3e-158">Relações</span><span class="sxs-lookup"><span data-stu-id="14f3e-158">Relationships</span></span>
| <span data-ttu-id="14f3e-159">Relação</span><span class="sxs-lookup"><span data-stu-id="14f3e-159">Relationship</span></span> | <span data-ttu-id="14f3e-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="14f3e-160">Type</span></span>   |<span data-ttu-id="14f3e-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="14f3e-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14f3e-162">páginas</span><span class="sxs-lookup"><span data-stu-id="14f3e-162">pages</span></span>|<span data-ttu-id="14f3e-163">Coleção [OnenotePage](page.md) </span><span class="sxs-lookup"><span data-stu-id="14f3e-163">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="14f3e-164">Obtém o conjunto de páginas da seção.</span><span class="sxs-lookup"><span data-stu-id="14f3e-164">The collection of pages in the section.</span></span>  <span data-ttu-id="14f3e-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14f3e-165">Read-only.</span></span> <span data-ttu-id="14f3e-166">Anulável.</span><span class="sxs-lookup"><span data-stu-id="14f3e-166">Nullable.</span></span>|
|<span data-ttu-id="14f3e-167">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="14f3e-167">parentNotebook</span></span>|[<span data-ttu-id="14f3e-168">Notebook</span><span class="sxs-lookup"><span data-stu-id="14f3e-168">Notebook</span></span>](notebook.md)|<span data-ttu-id="14f3e-169">O bloco de anotações que contém a seção.</span><span class="sxs-lookup"><span data-stu-id="14f3e-169">The notebook that contains the section.</span></span>  <span data-ttu-id="14f3e-170">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14f3e-170">Read-only.</span></span>|
|<span data-ttu-id="14f3e-171">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="14f3e-171">parentSectionGroup</span></span>|[<span data-ttu-id="14f3e-172">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="14f3e-172">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="14f3e-173">O grupo de seções que contém a seção.</span><span class="sxs-lookup"><span data-stu-id="14f3e-173">The section group that contains the section.</span></span>  <span data-ttu-id="14f3e-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14f3e-174">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="14f3e-175">Métodos</span><span class="sxs-lookup"><span data-stu-id="14f3e-175">Methods</span></span>

| <span data-ttu-id="14f3e-176">Método</span><span class="sxs-lookup"><span data-stu-id="14f3e-176">Method</span></span>           | <span data-ttu-id="14f3e-177">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="14f3e-177">Return Type</span></span>    |<span data-ttu-id="14f3e-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="14f3e-178">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="14f3e-179">Obter seção</span><span class="sxs-lookup"><span data-stu-id="14f3e-179">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="14f3e-180">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="14f3e-180">OnenoteSection</span></span>](section.md) |<span data-ttu-id="14f3e-181">Leia as propriedades e as relações da seção.</span><span class="sxs-lookup"><span data-stu-id="14f3e-181">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="14f3e-182">Create page</span><span class="sxs-lookup"><span data-stu-id="14f3e-182">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="14f3e-183">Page</span><span class="sxs-lookup"><span data-stu-id="14f3e-183">Page</span></span>](page.md)| <span data-ttu-id="14f3e-184">Crie uma página postando na coleção Pages na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="14f3e-184">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="14f3e-185">List pages</span><span class="sxs-lookup"><span data-stu-id="14f3e-185">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="14f3e-186">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="14f3e-186">[Page](page.md) collection</span></span>| <span data-ttu-id="14f3e-187">Obtém uma coleção de páginas na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="14f3e-187">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="14f3e-188">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="14f3e-188">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="14f3e-189">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="14f3e-189">None</span></span>|<span data-ttu-id="14f3e-190">Copie a seção para um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="14f3e-190">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="14f3e-191">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="14f3e-191">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="14f3e-192">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="14f3e-192">None</span></span>|<span data-ttu-id="14f3e-193">Copie a seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="14f3e-193">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
