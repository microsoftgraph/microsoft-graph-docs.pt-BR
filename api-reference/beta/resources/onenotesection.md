---
title: tipo de recurso onenoteSection
description: Uma seção em um bloco de anotações do OneNote. As seções podem conter páginas.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f23017506208c1c0ff4f5a190eafe12079626d23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522313"
---
# <a name="onenotesection-resource-type"></a><span data-ttu-id="f0cba-104">tipo de recurso onenoteSection</span><span class="sxs-lookup"><span data-stu-id="f0cba-104">onenoteSection resource type</span></span>

<span data-ttu-id="f0cba-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f0cba-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0cba-106">Uma seção em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f0cba-106">A section in a OneNote notebook.</span></span> <span data-ttu-id="f0cba-107">As seções podem conter páginas.</span><span class="sxs-lookup"><span data-stu-id="f0cba-107">Sections can contain pages.</span></span>

## <a name="properties"></a><span data-ttu-id="f0cba-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0cba-108">Properties</span></span>
| <span data-ttu-id="f0cba-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0cba-109">Property</span></span>     | <span data-ttu-id="f0cba-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0cba-110">Type</span></span>   |<span data-ttu-id="f0cba-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0cba-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0cba-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="f0cba-112">createdBy</span></span>|[<span data-ttu-id="f0cba-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="f0cba-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="f0cba-p103">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0cba-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="f0cba-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0cba-116">createdDateTime</span></span>|<span data-ttu-id="f0cba-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0cba-117">DateTimeOffset</span></span>|<span data-ttu-id="f0cba-118">A data e a hora em que a seção foi criada.</span><span class="sxs-lookup"><span data-stu-id="f0cba-118">The date and time when the section was created.</span></span> <span data-ttu-id="f0cba-119">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f0cba-119">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f0cba-120">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f0cba-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f0cba-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0cba-121">Read-only.</span></span>|
|<span data-ttu-id="f0cba-122">id</span><span class="sxs-lookup"><span data-stu-id="f0cba-122">id</span></span>|<span data-ttu-id="f0cba-123">String</span><span class="sxs-lookup"><span data-stu-id="f0cba-123">String</span></span>|<span data-ttu-id="f0cba-124">O identificador exclusivo da seção.</span><span class="sxs-lookup"><span data-stu-id="f0cba-124">The unique identifier of the section.</span></span>  <span data-ttu-id="f0cba-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0cba-125">Read-only.</span></span>|
|<span data-ttu-id="f0cba-126">isDefault</span><span class="sxs-lookup"><span data-stu-id="f0cba-126">isDefault</span></span>|<span data-ttu-id="f0cba-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0cba-127">Boolean</span></span>|<span data-ttu-id="f0cba-128">Indica se esta é a seção padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="f0cba-128">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="f0cba-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0cba-129">Read-only.</span></span>|
|<span data-ttu-id="f0cba-130">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f0cba-130">lastModifiedBy</span></span>|[<span data-ttu-id="f0cba-131">identitySet</span><span class="sxs-lookup"><span data-stu-id="f0cba-131">identitySet</span></span>](identityset.md)|<span data-ttu-id="f0cba-p107">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0cba-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="f0cba-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0cba-134">lastModifiedDateTime</span></span>|<span data-ttu-id="f0cba-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0cba-135">DateTimeOffset</span></span>|<span data-ttu-id="f0cba-136">A data e a hora em que a seção foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f0cba-136">The date and time when the section was last modified.</span></span> <span data-ttu-id="f0cba-137">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f0cba-137">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f0cba-138">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f0cba-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f0cba-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0cba-139">Read-only.</span></span>|
|<span data-ttu-id="f0cba-140">links</span><span class="sxs-lookup"><span data-stu-id="f0cba-140">links</span></span>|[<span data-ttu-id="f0cba-141">sectionLinks</span><span class="sxs-lookup"><span data-stu-id="f0cba-141">sectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="f0cba-142">Links para abrir a seção.</span><span class="sxs-lookup"><span data-stu-id="f0cba-142">Links for opening the section.</span></span> <span data-ttu-id="f0cba-143">O `oneNoteClientURL` link abre a seção no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="f0cba-143">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="f0cba-144">O `oneNoteWebURL` link abre a seção no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="f0cba-144">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="f0cba-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f0cba-145">displayName</span></span>|<span data-ttu-id="f0cba-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0cba-146">String</span></span>|<span data-ttu-id="f0cba-147">O nome da seção.</span><span class="sxs-lookup"><span data-stu-id="f0cba-147">The name of the section.</span></span> |
|<span data-ttu-id="f0cba-148">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="f0cba-148">pagesUrl</span></span>|<span data-ttu-id="f0cba-149">String</span><span class="sxs-lookup"><span data-stu-id="f0cba-149">String</span></span>|<span data-ttu-id="f0cba-150">O `pages` ponto de extremidade onde você pode obter detalhes de todas as páginas da seção.</span><span class="sxs-lookup"><span data-stu-id="f0cba-150">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="f0cba-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0cba-151">Read-only.</span></span>|
|<span data-ttu-id="f0cba-152">própria</span><span class="sxs-lookup"><span data-stu-id="f0cba-152">self</span></span>|<span data-ttu-id="f0cba-153">String</span><span class="sxs-lookup"><span data-stu-id="f0cba-153">String</span></span>|<span data-ttu-id="f0cba-154">O ponto de extremidade onde você pode obter detalhes sobre a seção.</span><span class="sxs-lookup"><span data-stu-id="f0cba-154">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="f0cba-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0cba-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0cba-156">Relações</span><span class="sxs-lookup"><span data-stu-id="f0cba-156">Relationships</span></span>
| <span data-ttu-id="f0cba-157">Relação</span><span class="sxs-lookup"><span data-stu-id="f0cba-157">Relationship</span></span> | <span data-ttu-id="f0cba-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0cba-158">Type</span></span>   |<span data-ttu-id="f0cba-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0cba-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0cba-160">páginas</span><span class="sxs-lookup"><span data-stu-id="f0cba-160">pages</span></span>|<span data-ttu-id="f0cba-161">coleção [onenotePage](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="f0cba-161">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="f0cba-162">Obtém o conjunto de páginas da seção.</span><span class="sxs-lookup"><span data-stu-id="f0cba-162">The collection of pages in the section.</span></span>  <span data-ttu-id="f0cba-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0cba-163">Read-only.</span></span> <span data-ttu-id="f0cba-164">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f0cba-164">Nullable.</span></span>|
|<span data-ttu-id="f0cba-165">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="f0cba-165">parentNotebook</span></span>|[<span data-ttu-id="f0cba-166">bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="f0cba-166">notebook</span></span>](notebook.md)|<span data-ttu-id="f0cba-167">O bloco de anotações que contém a seção.</span><span class="sxs-lookup"><span data-stu-id="f0cba-167">The notebook that contains the section.</span></span>  <span data-ttu-id="f0cba-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0cba-168">Read-only.</span></span>|
|<span data-ttu-id="f0cba-169">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="f0cba-169">parentSectionGroup</span></span>|[<span data-ttu-id="f0cba-170">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="f0cba-170">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="f0cba-171">O grupo de seções que contém a seção.</span><span class="sxs-lookup"><span data-stu-id="f0cba-171">The section group that contains the section.</span></span>  <span data-ttu-id="f0cba-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0cba-172">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="f0cba-173">Métodos</span><span class="sxs-lookup"><span data-stu-id="f0cba-173">Methods</span></span>

| <span data-ttu-id="f0cba-174">Método</span><span class="sxs-lookup"><span data-stu-id="f0cba-174">Method</span></span>           | <span data-ttu-id="f0cba-175">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f0cba-175">Return Type</span></span>    |<span data-ttu-id="f0cba-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0cba-176">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f0cba-177">Obter seção</span><span class="sxs-lookup"><span data-stu-id="f0cba-177">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="f0cba-178">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="f0cba-178">onenoteSection</span></span>](onenotesection.md) |<span data-ttu-id="f0cba-179">Leia as propriedades e as relações da seção.</span><span class="sxs-lookup"><span data-stu-id="f0cba-179">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="f0cba-180">Create page</span><span class="sxs-lookup"><span data-stu-id="f0cba-180">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="f0cba-181">onenotePage</span><span class="sxs-lookup"><span data-stu-id="f0cba-181">onenotePage</span></span>](onenotepage.md)| <span data-ttu-id="f0cba-182">Crie uma página postando na coleção Pages na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="f0cba-182">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="f0cba-183">List pages</span><span class="sxs-lookup"><span data-stu-id="f0cba-183">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="f0cba-184">coleção [onenotePage](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="f0cba-184">[onenotePage](onenotepage.md) collection</span></span>| <span data-ttu-id="f0cba-185">Obtém uma coleção de páginas na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="f0cba-185">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="f0cba-186">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="f0cba-186">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="f0cba-187">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0cba-187">None</span></span>|<span data-ttu-id="f0cba-188">Copie a seção para um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="f0cba-188">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="f0cba-189">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="f0cba-189">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="f0cba-190">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0cba-190">None</span></span>|<span data-ttu-id="f0cba-191">Copie a seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="f0cba-191">Copy the section to a specific section group.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f0cba-192">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0cba-192">JSON representation</span></span>

<span data-ttu-id="f0cba-193">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0cba-193">Here is a JSON representation of the resource.</span></span>

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
