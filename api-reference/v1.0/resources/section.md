---
title: tipo de recurso de seção
description: Uma seção em um bloco de anotações do OneNote. As seções podem conter páginas.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 421d910a79dd04403f09b455417d5ad97eac5691
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722011"
---
# <a name="section-resource-type"></a><span data-ttu-id="accea-104">tipo de recurso de seção</span><span class="sxs-lookup"><span data-stu-id="accea-104">section resource type</span></span>

<span data-ttu-id="accea-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="accea-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="accea-106">Uma seção em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="accea-106">A section in a OneNote notebook.</span></span> <span data-ttu-id="accea-107">As seções podem conter páginas.</span><span class="sxs-lookup"><span data-stu-id="accea-107">Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="accea-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="accea-108">JSON representation</span></span>

<span data-ttu-id="accea-109">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="accea-109">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="accea-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="accea-110">Properties</span></span>
| <span data-ttu-id="accea-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="accea-111">Property</span></span>     | <span data-ttu-id="accea-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="accea-112">Type</span></span>   |<span data-ttu-id="accea-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="accea-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="accea-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="accea-114">createdBy</span></span>|[<span data-ttu-id="accea-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="accea-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="accea-p103">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="accea-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="accea-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="accea-118">createdDateTime</span></span>|<span data-ttu-id="accea-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="accea-119">DateTimeOffset</span></span>|<span data-ttu-id="accea-120">A data e a hora em que a seção foi criada.</span><span class="sxs-lookup"><span data-stu-id="accea-120">The date and time when the section was created.</span></span> <span data-ttu-id="accea-121">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="accea-121">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="accea-122">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="accea-122">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="accea-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="accea-123">Read-only.</span></span>|
|<span data-ttu-id="accea-124">id</span><span class="sxs-lookup"><span data-stu-id="accea-124">id</span></span>|<span data-ttu-id="accea-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="accea-125">String</span></span>|<span data-ttu-id="accea-126">O identificador exclusivo da seção.</span><span class="sxs-lookup"><span data-stu-id="accea-126">The unique identifier of the section.</span></span>  <span data-ttu-id="accea-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="accea-127">Read-only.</span></span>|
|<span data-ttu-id="accea-128">isDefault</span><span class="sxs-lookup"><span data-stu-id="accea-128">isDefault</span></span>|<span data-ttu-id="accea-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="accea-129">Boolean</span></span>|<span data-ttu-id="accea-130">Indica se essa é a seção padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="accea-130">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="accea-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="accea-131">Read-only.</span></span>|
|<span data-ttu-id="accea-132">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="accea-132">lastModifiedBy</span></span>|[<span data-ttu-id="accea-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="accea-133">identitySet</span></span>](identityset.md)|<span data-ttu-id="accea-p107">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="accea-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="accea-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="accea-136">lastModifiedDateTime</span></span>|<span data-ttu-id="accea-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="accea-137">DateTimeOffset</span></span>|<span data-ttu-id="accea-138">A data e a hora em que a seção foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="accea-138">The date and time when the section was last modified.</span></span> <span data-ttu-id="accea-139">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="accea-139">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="accea-140">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="accea-140">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="accea-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="accea-141">Read-only.</span></span>|
|<span data-ttu-id="accea-142">links</span><span class="sxs-lookup"><span data-stu-id="accea-142">links</span></span>|[<span data-ttu-id="accea-143">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="accea-143">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="accea-144">Links para abrir a seção.</span><span class="sxs-lookup"><span data-stu-id="accea-144">Links for opening the section.</span></span> <span data-ttu-id="accea-145">O `oneNoteClientURL` link abre a seção no cliente nativo do OneNote se estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="accea-145">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="accea-146">O `oneNoteWebURL` link abre a seção no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="accea-146">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="accea-147">displayName</span><span class="sxs-lookup"><span data-stu-id="accea-147">displayName</span></span>|<span data-ttu-id="accea-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="accea-148">String</span></span>|<span data-ttu-id="accea-149">O nome da seção.</span><span class="sxs-lookup"><span data-stu-id="accea-149">The name of the section.</span></span> |
|<span data-ttu-id="accea-150">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="accea-150">pagesUrl</span></span>|<span data-ttu-id="accea-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="accea-151">String</span></span>|<span data-ttu-id="accea-152">O `pages` ponto de extremidade onde você pode obter detalhes para todas as páginas da seção.</span><span class="sxs-lookup"><span data-stu-id="accea-152">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="accea-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="accea-153">Read-only.</span></span>|
|<span data-ttu-id="accea-154">self</span><span class="sxs-lookup"><span data-stu-id="accea-154">self</span></span>|<span data-ttu-id="accea-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="accea-155">String</span></span>|<span data-ttu-id="accea-156">O ponto de extremidade onde você pode obter detalhes sobre a seção.</span><span class="sxs-lookup"><span data-stu-id="accea-156">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="accea-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="accea-157">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="accea-158">Relações</span><span class="sxs-lookup"><span data-stu-id="accea-158">Relationships</span></span>
| <span data-ttu-id="accea-159">Relação</span><span class="sxs-lookup"><span data-stu-id="accea-159">Relationship</span></span> | <span data-ttu-id="accea-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="accea-160">Type</span></span>   |<span data-ttu-id="accea-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="accea-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="accea-162">páginas</span><span class="sxs-lookup"><span data-stu-id="accea-162">pages</span></span>|<span data-ttu-id="accea-163">Coleção [OnenotePage](page.md) </span><span class="sxs-lookup"><span data-stu-id="accea-163">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="accea-164">Obtém o conjunto de páginas da seção.</span><span class="sxs-lookup"><span data-stu-id="accea-164">The collection of pages in the section.</span></span>  <span data-ttu-id="accea-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="accea-165">Read-only.</span></span> <span data-ttu-id="accea-166">Anulável.</span><span class="sxs-lookup"><span data-stu-id="accea-166">Nullable.</span></span>|
|<span data-ttu-id="accea-167">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="accea-167">parentNotebook</span></span>|[<span data-ttu-id="accea-168">Notebook</span><span class="sxs-lookup"><span data-stu-id="accea-168">Notebook</span></span>](notebook.md)|<span data-ttu-id="accea-169">O bloco de anotações que contém a seção.</span><span class="sxs-lookup"><span data-stu-id="accea-169">The notebook that contains the section.</span></span>  <span data-ttu-id="accea-170">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="accea-170">Read-only.</span></span>|
|<span data-ttu-id="accea-171">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="accea-171">parentSectionGroup</span></span>|[<span data-ttu-id="accea-172">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="accea-172">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="accea-173">O grupo de seções que contém a seção.</span><span class="sxs-lookup"><span data-stu-id="accea-173">The section group that contains the section.</span></span>  <span data-ttu-id="accea-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="accea-174">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="accea-175">Methods</span><span class="sxs-lookup"><span data-stu-id="accea-175">Methods</span></span>

| <span data-ttu-id="accea-176">Método</span><span class="sxs-lookup"><span data-stu-id="accea-176">Method</span></span>           | <span data-ttu-id="accea-177">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="accea-177">Return Type</span></span>    |<span data-ttu-id="accea-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="accea-178">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="accea-179">Obter seção</span><span class="sxs-lookup"><span data-stu-id="accea-179">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="accea-180">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="accea-180">OnenoteSection</span></span>](section.md) |<span data-ttu-id="accea-181">Leia as propriedades e as relações da seção.</span><span class="sxs-lookup"><span data-stu-id="accea-181">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="accea-182">Create page</span><span class="sxs-lookup"><span data-stu-id="accea-182">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="accea-183">Page</span><span class="sxs-lookup"><span data-stu-id="accea-183">Page</span></span>](page.md)| <span data-ttu-id="accea-184">Crie uma página postando na coleção pages na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="accea-184">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="accea-185">List pages</span><span class="sxs-lookup"><span data-stu-id="accea-185">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="accea-186">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="accea-186">[Page](page.md) collection</span></span>| <span data-ttu-id="accea-187">Obter uma coleção de páginas na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="accea-187">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="accea-188">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="accea-188">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="accea-189">Nenhum</span><span class="sxs-lookup"><span data-stu-id="accea-189">None</span></span>|<span data-ttu-id="accea-190">Copie a seção para um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="accea-190">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="accea-191">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="accea-191">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="accea-192">Nenhum</span><span class="sxs-lookup"><span data-stu-id="accea-192">None</span></span>|<span data-ttu-id="accea-193">Copie a seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="accea-193">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

