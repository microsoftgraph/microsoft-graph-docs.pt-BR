---
title: tipo de recurso onenoteSection
description: Uma seção em um bloco de anotações do OneNote. As seções podem conter páginas.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: 98a878ae10eb4756c631aa0031d0342aa90e6e8c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968359"
---
# <a name="onenotesection-resource-type"></a><span data-ttu-id="7eca3-104">tipo de recurso onenoteSection</span><span class="sxs-lookup"><span data-stu-id="7eca3-104">onenoteSection resource type</span></span>

<span data-ttu-id="7eca3-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7eca3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7eca3-106">Uma seção em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="7eca3-106">A section in a OneNote notebook.</span></span> <span data-ttu-id="7eca3-107">As seções podem conter páginas.</span><span class="sxs-lookup"><span data-stu-id="7eca3-107">Sections can contain pages.</span></span>

## <a name="properties"></a><span data-ttu-id="7eca3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7eca3-108">Properties</span></span>
| <span data-ttu-id="7eca3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7eca3-109">Property</span></span>     | <span data-ttu-id="7eca3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7eca3-110">Type</span></span>   |<span data-ttu-id="7eca3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7eca3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7eca3-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="7eca3-112">createdBy</span></span>|[<span data-ttu-id="7eca3-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="7eca3-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="7eca3-p103">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7eca3-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="7eca3-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7eca3-116">createdDateTime</span></span>|<span data-ttu-id="7eca3-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7eca3-117">DateTimeOffset</span></span>|<span data-ttu-id="7eca3-118">A data e a hora em que a seção foi criada.</span><span class="sxs-lookup"><span data-stu-id="7eca3-118">The date and time when the section was created.</span></span> <span data-ttu-id="7eca3-119">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7eca3-119">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7eca3-120">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7eca3-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="7eca3-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7eca3-121">Read-only.</span></span>|
|<span data-ttu-id="7eca3-122">id</span><span class="sxs-lookup"><span data-stu-id="7eca3-122">id</span></span>|<span data-ttu-id="7eca3-123">String</span><span class="sxs-lookup"><span data-stu-id="7eca3-123">String</span></span>|<span data-ttu-id="7eca3-124">O identificador exclusivo da seção.</span><span class="sxs-lookup"><span data-stu-id="7eca3-124">The unique identifier of the section.</span></span>  <span data-ttu-id="7eca3-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7eca3-125">Read-only.</span></span>|
|<span data-ttu-id="7eca3-126">isDefault</span><span class="sxs-lookup"><span data-stu-id="7eca3-126">isDefault</span></span>|<span data-ttu-id="7eca3-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="7eca3-127">Boolean</span></span>|<span data-ttu-id="7eca3-128">Indica se esta é a seção padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="7eca3-128">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="7eca3-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7eca3-129">Read-only.</span></span>|
|<span data-ttu-id="7eca3-130">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="7eca3-130">lastModifiedBy</span></span>|[<span data-ttu-id="7eca3-131">identitySet</span><span class="sxs-lookup"><span data-stu-id="7eca3-131">identitySet</span></span>](identityset.md)|<span data-ttu-id="7eca3-p107">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7eca3-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="7eca3-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7eca3-134">lastModifiedDateTime</span></span>|<span data-ttu-id="7eca3-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7eca3-135">DateTimeOffset</span></span>|<span data-ttu-id="7eca3-136">A data e a hora em que a seção foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7eca3-136">The date and time when the section was last modified.</span></span> <span data-ttu-id="7eca3-137">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7eca3-137">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7eca3-138">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7eca3-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="7eca3-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7eca3-139">Read-only.</span></span>|
|<span data-ttu-id="7eca3-140">links</span><span class="sxs-lookup"><span data-stu-id="7eca3-140">links</span></span>|[<span data-ttu-id="7eca3-141">sectionLinks</span><span class="sxs-lookup"><span data-stu-id="7eca3-141">sectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="7eca3-142">Links para abrir a seção.</span><span class="sxs-lookup"><span data-stu-id="7eca3-142">Links for opening the section.</span></span> <span data-ttu-id="7eca3-143">O `oneNoteClientURL` link abre a seção no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="7eca3-143">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="7eca3-144">O `oneNoteWebURL` link abre a seção no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="7eca3-144">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="7eca3-145">displayName</span><span class="sxs-lookup"><span data-stu-id="7eca3-145">displayName</span></span>|<span data-ttu-id="7eca3-146">String</span><span class="sxs-lookup"><span data-stu-id="7eca3-146">String</span></span>|<span data-ttu-id="7eca3-147">O nome da seção.</span><span class="sxs-lookup"><span data-stu-id="7eca3-147">The name of the section.</span></span> |
|<span data-ttu-id="7eca3-148">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="7eca3-148">pagesUrl</span></span>|<span data-ttu-id="7eca3-149">String</span><span class="sxs-lookup"><span data-stu-id="7eca3-149">String</span></span>|<span data-ttu-id="7eca3-150">O `pages` ponto de extremidade onde você pode obter detalhes de todas as páginas da seção.</span><span class="sxs-lookup"><span data-stu-id="7eca3-150">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="7eca3-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7eca3-151">Read-only.</span></span>|
|<span data-ttu-id="7eca3-152">própria</span><span class="sxs-lookup"><span data-stu-id="7eca3-152">self</span></span>|<span data-ttu-id="7eca3-153">String</span><span class="sxs-lookup"><span data-stu-id="7eca3-153">String</span></span>|<span data-ttu-id="7eca3-154">O ponto de extremidade onde você pode obter detalhes sobre a seção.</span><span class="sxs-lookup"><span data-stu-id="7eca3-154">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="7eca3-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7eca3-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7eca3-156">Relações</span><span class="sxs-lookup"><span data-stu-id="7eca3-156">Relationships</span></span>
| <span data-ttu-id="7eca3-157">Relação</span><span class="sxs-lookup"><span data-stu-id="7eca3-157">Relationship</span></span> | <span data-ttu-id="7eca3-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="7eca3-158">Type</span></span>   |<span data-ttu-id="7eca3-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="7eca3-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7eca3-160">páginas</span><span class="sxs-lookup"><span data-stu-id="7eca3-160">pages</span></span>|<span data-ttu-id="7eca3-161">coleção [onenotePage](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="7eca3-161">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="7eca3-162">Obtém o conjunto de páginas da seção.</span><span class="sxs-lookup"><span data-stu-id="7eca3-162">The collection of pages in the section.</span></span>  <span data-ttu-id="7eca3-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7eca3-163">Read-only.</span></span> <span data-ttu-id="7eca3-164">Anulável.</span><span class="sxs-lookup"><span data-stu-id="7eca3-164">Nullable.</span></span>|
|<span data-ttu-id="7eca3-165">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="7eca3-165">parentNotebook</span></span>|[<span data-ttu-id="7eca3-166">bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="7eca3-166">notebook</span></span>](notebook.md)|<span data-ttu-id="7eca3-167">O bloco de anotações que contém a seção.</span><span class="sxs-lookup"><span data-stu-id="7eca3-167">The notebook that contains the section.</span></span>  <span data-ttu-id="7eca3-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7eca3-168">Read-only.</span></span>|
|<span data-ttu-id="7eca3-169">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="7eca3-169">parentSectionGroup</span></span>|[<span data-ttu-id="7eca3-170">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="7eca3-170">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="7eca3-171">O grupo de seções que contém a seção.</span><span class="sxs-lookup"><span data-stu-id="7eca3-171">The section group that contains the section.</span></span>  <span data-ttu-id="7eca3-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7eca3-172">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="7eca3-173">Methods</span><span class="sxs-lookup"><span data-stu-id="7eca3-173">Methods</span></span>

| <span data-ttu-id="7eca3-174">Método</span><span class="sxs-lookup"><span data-stu-id="7eca3-174">Method</span></span>           | <span data-ttu-id="7eca3-175">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7eca3-175">Return Type</span></span>    |<span data-ttu-id="7eca3-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="7eca3-176">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7eca3-177">Obter seção</span><span class="sxs-lookup"><span data-stu-id="7eca3-177">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="7eca3-178">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="7eca3-178">onenoteSection</span></span>](onenotesection.md) |<span data-ttu-id="7eca3-179">Leia as propriedades e as relações da seção.</span><span class="sxs-lookup"><span data-stu-id="7eca3-179">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="7eca3-180">Create page</span><span class="sxs-lookup"><span data-stu-id="7eca3-180">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="7eca3-181">onenotePage</span><span class="sxs-lookup"><span data-stu-id="7eca3-181">onenotePage</span></span>](onenotepage.md)| <span data-ttu-id="7eca3-182">Crie uma página postando na coleção Pages na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="7eca3-182">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="7eca3-183">List pages</span><span class="sxs-lookup"><span data-stu-id="7eca3-183">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="7eca3-184">coleção [onenotePage](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="7eca3-184">[onenotePage](onenotepage.md) collection</span></span>| <span data-ttu-id="7eca3-185">Obtém uma coleção de páginas na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="7eca3-185">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="7eca3-186">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="7eca3-186">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="7eca3-187">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7eca3-187">None</span></span>|<span data-ttu-id="7eca3-188">Copie a seção para um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="7eca3-188">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="7eca3-189">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="7eca3-189">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="7eca3-190">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7eca3-190">None</span></span>|<span data-ttu-id="7eca3-191">Copie a seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="7eca3-191">Copy the section to a specific section group.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7eca3-192">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7eca3-192">JSON representation</span></span>

<span data-ttu-id="7eca3-193">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7eca3-193">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


