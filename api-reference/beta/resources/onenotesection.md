---
title: tipo de recurso onenoteSection
description: Uma seção em um bloco de anotações do OneNote. As seções podem conter páginas.
localization_priority: Normal
ms.openlocfilehash: d262065f46052c1cae55b42babaa91a2e065d3ef
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348469"
---
# <a name="onenotesection-resource-type"></a><span data-ttu-id="52886-104">tipo de recurso onenoteSection</span><span class="sxs-lookup"><span data-stu-id="52886-104">onenoteSection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52886-105">Uma seção em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="52886-105">A section in a OneNote notebook.</span></span> <span data-ttu-id="52886-106">As seções podem conter páginas.</span><span class="sxs-lookup"><span data-stu-id="52886-106">Sections can contain pages.</span></span>

## <a name="properties"></a><span data-ttu-id="52886-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52886-107">Properties</span></span>
| <span data-ttu-id="52886-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52886-108">Property</span></span>     | <span data-ttu-id="52886-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="52886-109">Type</span></span>   |<span data-ttu-id="52886-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="52886-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52886-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="52886-111">createdBy</span></span>|[<span data-ttu-id="52886-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="52886-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="52886-p103">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52886-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="52886-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="52886-115">createdDateTime</span></span>|<span data-ttu-id="52886-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52886-116">DateTimeOffset</span></span>|<span data-ttu-id="52886-117">A data e a hora em que a seção foi criada.</span><span class="sxs-lookup"><span data-stu-id="52886-117">The date and time when the section was created.</span></span> <span data-ttu-id="52886-118">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="52886-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="52886-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="52886-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="52886-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52886-120">Read-only.</span></span>|
|<span data-ttu-id="52886-121">id</span><span class="sxs-lookup"><span data-stu-id="52886-121">id</span></span>|<span data-ttu-id="52886-122">String</span><span class="sxs-lookup"><span data-stu-id="52886-122">String</span></span>|<span data-ttu-id="52886-123">O identificador exclusivo da seção.</span><span class="sxs-lookup"><span data-stu-id="52886-123">The unique identifier of the section.</span></span>  <span data-ttu-id="52886-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52886-124">Read-only.</span></span>|
|<span data-ttu-id="52886-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="52886-125">isDefault</span></span>|<span data-ttu-id="52886-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="52886-126">Boolean</span></span>|<span data-ttu-id="52886-127">Indica se esta é a seção padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="52886-127">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="52886-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52886-128">Read-only.</span></span>|
|<span data-ttu-id="52886-129">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="52886-129">lastModifiedBy</span></span>|[<span data-ttu-id="52886-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="52886-130">identitySet</span></span>](identityset.md)|<span data-ttu-id="52886-p107">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52886-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="52886-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="52886-133">lastModifiedDateTime</span></span>|<span data-ttu-id="52886-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52886-134">DateTimeOffset</span></span>|<span data-ttu-id="52886-135">A data e a hora em que a seção foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="52886-135">The date and time when the section was last modified.</span></span> <span data-ttu-id="52886-136">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="52886-136">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="52886-137">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="52886-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="52886-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52886-138">Read-only.</span></span>|
|<span data-ttu-id="52886-139">links</span><span class="sxs-lookup"><span data-stu-id="52886-139">links</span></span>|[<span data-ttu-id="52886-140">sectionLinks</span><span class="sxs-lookup"><span data-stu-id="52886-140">sectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="52886-141">Links para abrir a seção.</span><span class="sxs-lookup"><span data-stu-id="52886-141">Links for opening the section.</span></span> <span data-ttu-id="52886-142">O `oneNoteClientURL` link abre a seção no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="52886-142">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="52886-143">O `oneNoteWebURL` link abre a seção no OneNote online.</span><span class="sxs-lookup"><span data-stu-id="52886-143">The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="52886-144">displayName</span><span class="sxs-lookup"><span data-stu-id="52886-144">displayName</span></span>|<span data-ttu-id="52886-145">String</span><span class="sxs-lookup"><span data-stu-id="52886-145">String</span></span>|<span data-ttu-id="52886-146">O nome da seção.</span><span class="sxs-lookup"><span data-stu-id="52886-146">The name of the section.</span></span> |
|<span data-ttu-id="52886-147">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="52886-147">pagesUrl</span></span>|<span data-ttu-id="52886-148">String</span><span class="sxs-lookup"><span data-stu-id="52886-148">String</span></span>|<span data-ttu-id="52886-149">O `pages` ponto de extremidade onde você pode obter detalhes de todas as páginas da seção.</span><span class="sxs-lookup"><span data-stu-id="52886-149">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="52886-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52886-150">Read-only.</span></span>|
|<span data-ttu-id="52886-151">própria</span><span class="sxs-lookup"><span data-stu-id="52886-151">self</span></span>|<span data-ttu-id="52886-152">String</span><span class="sxs-lookup"><span data-stu-id="52886-152">String</span></span>|<span data-ttu-id="52886-153">O ponto de extremidade onde você pode obter detalhes sobre a seção.</span><span class="sxs-lookup"><span data-stu-id="52886-153">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="52886-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52886-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52886-155">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="52886-155">Relationships</span></span>
| <span data-ttu-id="52886-156">Relação</span><span class="sxs-lookup"><span data-stu-id="52886-156">Relationship</span></span> | <span data-ttu-id="52886-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="52886-157">Type</span></span>   |<span data-ttu-id="52886-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="52886-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52886-159">páginas</span><span class="sxs-lookup"><span data-stu-id="52886-159">pages</span></span>|<span data-ttu-id="52886-160">coleção [onenotePage](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="52886-160">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="52886-161">Obtém o conjunto de páginas da seção.</span><span class="sxs-lookup"><span data-stu-id="52886-161">The collection of pages in the section.</span></span>  <span data-ttu-id="52886-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52886-162">Read-only.</span></span> <span data-ttu-id="52886-163">Anulável.</span><span class="sxs-lookup"><span data-stu-id="52886-163">Nullable.</span></span>|
|<span data-ttu-id="52886-164">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="52886-164">parentNotebook</span></span>|[<span data-ttu-id="52886-165">anotações</span><span class="sxs-lookup"><span data-stu-id="52886-165">notebook</span></span>](notebook.md)|<span data-ttu-id="52886-166">O bloco de anotações que contém a seção.</span><span class="sxs-lookup"><span data-stu-id="52886-166">The notebook that contains the section.</span></span>  <span data-ttu-id="52886-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52886-167">Read-only.</span></span>|
|<span data-ttu-id="52886-168">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="52886-168">parentSectionGroup</span></span>|[<span data-ttu-id="52886-169">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="52886-169">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="52886-170">O grupo de seções que contém a seção.</span><span class="sxs-lookup"><span data-stu-id="52886-170">The section group that contains the section.</span></span>  <span data-ttu-id="52886-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52886-171">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="52886-172">Métodos</span><span class="sxs-lookup"><span data-stu-id="52886-172">Methods</span></span>

| <span data-ttu-id="52886-173">Método</span><span class="sxs-lookup"><span data-stu-id="52886-173">Method</span></span>           | <span data-ttu-id="52886-174">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="52886-174">Return Type</span></span>    |<span data-ttu-id="52886-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="52886-175">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52886-176">Obter seção</span><span class="sxs-lookup"><span data-stu-id="52886-176">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="52886-177">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="52886-177">onenoteSection</span></span>](onenotesection.md) |<span data-ttu-id="52886-178">Leia as propriedades e as relações da seção.</span><span class="sxs-lookup"><span data-stu-id="52886-178">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="52886-179">Create page</span><span class="sxs-lookup"><span data-stu-id="52886-179">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="52886-180">onenotePage</span><span class="sxs-lookup"><span data-stu-id="52886-180">onenotePage</span></span>](onenotepage.md)| <span data-ttu-id="52886-181">Crie uma página postando na coleção Pages na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="52886-181">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="52886-182">Listar páginas</span><span class="sxs-lookup"><span data-stu-id="52886-182">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="52886-183">coleção [onenotePage](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="52886-183">[onenotePage](onenotepage.md) collection</span></span>| <span data-ttu-id="52886-184">Obtém uma coleção de páginas na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="52886-184">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="52886-185">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="52886-185">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="52886-186">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52886-186">None</span></span>|<span data-ttu-id="52886-187">Copie a seção para um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="52886-187">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="52886-188">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="52886-188">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="52886-189">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52886-189">None</span></span>|<span data-ttu-id="52886-190">Copie a seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="52886-190">Copy the section to a specific section group.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="52886-191">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52886-191">JSON representation</span></span>

<span data-ttu-id="52886-192">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52886-192">Here is a JSON representation of the resource.</span></span>

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
