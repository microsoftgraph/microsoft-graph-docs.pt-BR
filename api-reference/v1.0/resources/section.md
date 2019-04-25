---
title: tipo de recurso Section
description: Uma seção em um bloco de anotações do OneNote. As seções podem conter páginas.
localization_priority: Normal
ms.openlocfilehash: f9cb5a8e3ddf9cf4a045103e4ecc7909653d797c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579153"
---
# <a name="section-resource-type"></a><span data-ttu-id="46747-104">tipo de recurso Section</span><span class="sxs-lookup"><span data-stu-id="46747-104">section resource type</span></span>

<span data-ttu-id="46747-105">Uma seção em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="46747-105">A section in a OneNote notebook.</span></span> <span data-ttu-id="46747-106">As seções podem conter páginas.</span><span class="sxs-lookup"><span data-stu-id="46747-106">Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="46747-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46747-107">JSON representation</span></span>

<span data-ttu-id="46747-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="46747-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="46747-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46747-109">Properties</span></span>
| <span data-ttu-id="46747-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46747-110">Property</span></span>     | <span data-ttu-id="46747-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="46747-111">Type</span></span>   |<span data-ttu-id="46747-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="46747-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46747-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="46747-113">createdBy</span></span>|[<span data-ttu-id="46747-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="46747-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="46747-p103">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46747-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="46747-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="46747-117">createdDateTime</span></span>|<span data-ttu-id="46747-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46747-118">DateTimeOffset</span></span>|<span data-ttu-id="46747-119">A data e a hora em que a seção foi criada.</span><span class="sxs-lookup"><span data-stu-id="46747-119">The date and time when the section was created.</span></span> <span data-ttu-id="46747-120">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="46747-120">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="46747-121">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="46747-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="46747-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46747-122">Read-only.</span></span>|
|<span data-ttu-id="46747-123">id</span><span class="sxs-lookup"><span data-stu-id="46747-123">id</span></span>|<span data-ttu-id="46747-124">String</span><span class="sxs-lookup"><span data-stu-id="46747-124">String</span></span>|<span data-ttu-id="46747-125">O identificador exclusivo da seção.</span><span class="sxs-lookup"><span data-stu-id="46747-125">The unique identifier of the section.</span></span>  <span data-ttu-id="46747-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46747-126">Read-only.</span></span>|
|<span data-ttu-id="46747-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="46747-127">isDefault</span></span>|<span data-ttu-id="46747-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="46747-128">Boolean</span></span>|<span data-ttu-id="46747-129">Indica se esta é a seção padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="46747-129">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="46747-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46747-130">Read-only.</span></span>|
|<span data-ttu-id="46747-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="46747-131">lastModifiedBy</span></span>|[<span data-ttu-id="46747-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="46747-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="46747-p107">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46747-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="46747-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="46747-135">lastModifiedDateTime</span></span>|<span data-ttu-id="46747-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46747-136">DateTimeOffset</span></span>|<span data-ttu-id="46747-137">A data e a hora em que a seção foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="46747-137">The date and time when the section was last modified.</span></span> <span data-ttu-id="46747-138">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="46747-138">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="46747-139">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="46747-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="46747-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46747-140">Read-only.</span></span>|
|<span data-ttu-id="46747-141">links</span><span class="sxs-lookup"><span data-stu-id="46747-141">links</span></span>|[<span data-ttu-id="46747-142">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="46747-142">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="46747-143">Links para abrir a seção.</span><span class="sxs-lookup"><span data-stu-id="46747-143">Links for opening the section.</span></span> <span data-ttu-id="46747-144">O `oneNoteClientURL` link abre a seção no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="46747-144">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="46747-145">O `oneNoteWebURL` link abre a seção no OneNote online.</span><span class="sxs-lookup"><span data-stu-id="46747-145">The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="46747-146">displayName</span><span class="sxs-lookup"><span data-stu-id="46747-146">displayName</span></span>|<span data-ttu-id="46747-147">String</span><span class="sxs-lookup"><span data-stu-id="46747-147">String</span></span>|<span data-ttu-id="46747-148">O nome da seção.</span><span class="sxs-lookup"><span data-stu-id="46747-148">The name of the section.</span></span> |
|<span data-ttu-id="46747-149">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="46747-149">pagesUrl</span></span>|<span data-ttu-id="46747-150">String</span><span class="sxs-lookup"><span data-stu-id="46747-150">String</span></span>|<span data-ttu-id="46747-151">O `pages` ponto de extremidade onde você pode obter detalhes de todas as páginas da seção.</span><span class="sxs-lookup"><span data-stu-id="46747-151">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="46747-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46747-152">Read-only.</span></span>|
|<span data-ttu-id="46747-153">própria</span><span class="sxs-lookup"><span data-stu-id="46747-153">self</span></span>|<span data-ttu-id="46747-154">String</span><span class="sxs-lookup"><span data-stu-id="46747-154">String</span></span>|<span data-ttu-id="46747-155">O ponto de extremidade onde você pode obter detalhes sobre a seção.</span><span class="sxs-lookup"><span data-stu-id="46747-155">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="46747-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46747-156">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46747-157">Relações</span><span class="sxs-lookup"><span data-stu-id="46747-157">Relationships</span></span>
| <span data-ttu-id="46747-158">Relação</span><span class="sxs-lookup"><span data-stu-id="46747-158">Relationship</span></span> | <span data-ttu-id="46747-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="46747-159">Type</span></span>   |<span data-ttu-id="46747-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="46747-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46747-161">páginas</span><span class="sxs-lookup"><span data-stu-id="46747-161">pages</span></span>|<span data-ttu-id="46747-162">Coleção [OnenotePage](page.md)</span><span class="sxs-lookup"><span data-stu-id="46747-162">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="46747-163">Obtém o conjunto de páginas da seção.</span><span class="sxs-lookup"><span data-stu-id="46747-163">The collection of pages in the section.</span></span>  <span data-ttu-id="46747-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46747-164">Read-only.</span></span> <span data-ttu-id="46747-165">Anulável.</span><span class="sxs-lookup"><span data-stu-id="46747-165">Nullable.</span></span>|
|<span data-ttu-id="46747-166">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="46747-166">parentNotebook</span></span>|[<span data-ttu-id="46747-167">Bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="46747-167">Notebook</span></span>](notebook.md)|<span data-ttu-id="46747-168">O bloco de anotações que contém a seção.</span><span class="sxs-lookup"><span data-stu-id="46747-168">The notebook that contains the section.</span></span>  <span data-ttu-id="46747-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46747-169">Read-only.</span></span>|
|<span data-ttu-id="46747-170">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="46747-170">parentSectionGroup</span></span>|[<span data-ttu-id="46747-171">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="46747-171">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="46747-172">O grupo de seções que contém a seção.</span><span class="sxs-lookup"><span data-stu-id="46747-172">The section group that contains the section.</span></span>  <span data-ttu-id="46747-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46747-173">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="46747-174">Métodos</span><span class="sxs-lookup"><span data-stu-id="46747-174">Methods</span></span>

| <span data-ttu-id="46747-175">Método</span><span class="sxs-lookup"><span data-stu-id="46747-175">Method</span></span>           | <span data-ttu-id="46747-176">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="46747-176">Return Type</span></span>    |<span data-ttu-id="46747-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="46747-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="46747-178">Obter seção</span><span class="sxs-lookup"><span data-stu-id="46747-178">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="46747-179">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="46747-179">OnenoteSection</span></span>](section.md) |<span data-ttu-id="46747-180">Leia as propriedades e as relações da seção.</span><span class="sxs-lookup"><span data-stu-id="46747-180">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="46747-181">Criar página</span><span class="sxs-lookup"><span data-stu-id="46747-181">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="46747-182">Page</span><span class="sxs-lookup"><span data-stu-id="46747-182">Page</span></span>](page.md)| <span data-ttu-id="46747-183">Crie uma página postando na coleção Pages na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="46747-183">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="46747-184">Listar páginas</span><span class="sxs-lookup"><span data-stu-id="46747-184">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="46747-185">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="46747-185">[Page](page.md) collection</span></span>| <span data-ttu-id="46747-186">Obtém uma coleção de páginas na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="46747-186">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="46747-187">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="46747-187">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="46747-188">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46747-188">None</span></span>|<span data-ttu-id="46747-189">Copie a seção para um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="46747-189">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="46747-190">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="46747-190">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="46747-191">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46747-191">None</span></span>|<span data-ttu-id="46747-192">Copie a seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="46747-192">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
