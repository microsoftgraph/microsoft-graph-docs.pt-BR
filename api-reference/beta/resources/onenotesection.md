---
title: tipo de recurso onenoteSection
description: Uma seção em um bloco de anotações do OneNote. As seções podem conter páginas.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ed90d29e0441544bffd2576a255acf17e6cb3996
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966396"
---
# <a name="onenotesection-resource-type"></a><span data-ttu-id="11484-104">tipo de recurso onenoteSection</span><span class="sxs-lookup"><span data-stu-id="11484-104">onenoteSection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11484-105">Uma seção em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="11484-105">A section in a OneNote notebook.</span></span> <span data-ttu-id="11484-106">As seções podem conter páginas.</span><span class="sxs-lookup"><span data-stu-id="11484-106">Sections can contain pages.</span></span>

## <a name="properties"></a><span data-ttu-id="11484-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11484-107">Properties</span></span>
| <span data-ttu-id="11484-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11484-108">Property</span></span>     | <span data-ttu-id="11484-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="11484-109">Type</span></span>   |<span data-ttu-id="11484-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="11484-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11484-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="11484-111">createdBy</span></span>|[<span data-ttu-id="11484-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="11484-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="11484-p103">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11484-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="11484-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11484-115">createdDateTime</span></span>|<span data-ttu-id="11484-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11484-116">DateTimeOffset</span></span>|<span data-ttu-id="11484-117">A data e a hora em que a seção foi criada.</span><span class="sxs-lookup"><span data-stu-id="11484-117">The date and time when the section was created.</span></span> <span data-ttu-id="11484-118">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="11484-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="11484-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="11484-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="11484-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11484-120">Read-only.</span></span>|
|<span data-ttu-id="11484-121">id</span><span class="sxs-lookup"><span data-stu-id="11484-121">id</span></span>|<span data-ttu-id="11484-122">String</span><span class="sxs-lookup"><span data-stu-id="11484-122">String</span></span>|<span data-ttu-id="11484-123">O identificador exclusivo da seção.</span><span class="sxs-lookup"><span data-stu-id="11484-123">The unique identifier of the section.</span></span>  <span data-ttu-id="11484-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11484-124">Read-only.</span></span>|
|<span data-ttu-id="11484-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="11484-125">isDefault</span></span>|<span data-ttu-id="11484-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="11484-126">Boolean</span></span>|<span data-ttu-id="11484-127">Indica se esta é a seção padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="11484-127">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="11484-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11484-128">Read-only.</span></span>|
|<span data-ttu-id="11484-129">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="11484-129">lastModifiedBy</span></span>|[<span data-ttu-id="11484-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="11484-130">identitySet</span></span>](identityset.md)|<span data-ttu-id="11484-p107">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11484-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="11484-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11484-133">lastModifiedDateTime</span></span>|<span data-ttu-id="11484-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11484-134">DateTimeOffset</span></span>|<span data-ttu-id="11484-135">A data e a hora em que a seção foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="11484-135">The date and time when the section was last modified.</span></span> <span data-ttu-id="11484-136">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="11484-136">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="11484-137">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="11484-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="11484-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11484-138">Read-only.</span></span>|
|<span data-ttu-id="11484-139">links</span><span class="sxs-lookup"><span data-stu-id="11484-139">links</span></span>|[<span data-ttu-id="11484-140">sectionLinks</span><span class="sxs-lookup"><span data-stu-id="11484-140">sectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="11484-141">Links para abrir a seção.</span><span class="sxs-lookup"><span data-stu-id="11484-141">Links for opening the section.</span></span> <span data-ttu-id="11484-142">O `oneNoteClientURL` link abre a seção no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="11484-142">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="11484-143">O `oneNoteWebURL` link abre a seção no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="11484-143">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="11484-144">displayName</span><span class="sxs-lookup"><span data-stu-id="11484-144">displayName</span></span>|<span data-ttu-id="11484-145">String</span><span class="sxs-lookup"><span data-stu-id="11484-145">String</span></span>|<span data-ttu-id="11484-146">O nome da seção.</span><span class="sxs-lookup"><span data-stu-id="11484-146">The name of the section.</span></span> |
|<span data-ttu-id="11484-147">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="11484-147">pagesUrl</span></span>|<span data-ttu-id="11484-148">String</span><span class="sxs-lookup"><span data-stu-id="11484-148">String</span></span>|<span data-ttu-id="11484-149">O `pages` ponto de extremidade onde você pode obter detalhes de todas as páginas da seção.</span><span class="sxs-lookup"><span data-stu-id="11484-149">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="11484-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11484-150">Read-only.</span></span>|
|<span data-ttu-id="11484-151">própria</span><span class="sxs-lookup"><span data-stu-id="11484-151">self</span></span>|<span data-ttu-id="11484-152">String</span><span class="sxs-lookup"><span data-stu-id="11484-152">String</span></span>|<span data-ttu-id="11484-153">O ponto de extremidade onde você pode obter detalhes sobre a seção.</span><span class="sxs-lookup"><span data-stu-id="11484-153">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="11484-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11484-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11484-155">Relações</span><span class="sxs-lookup"><span data-stu-id="11484-155">Relationships</span></span>
| <span data-ttu-id="11484-156">Relação</span><span class="sxs-lookup"><span data-stu-id="11484-156">Relationship</span></span> | <span data-ttu-id="11484-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="11484-157">Type</span></span>   |<span data-ttu-id="11484-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="11484-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11484-159">páginas</span><span class="sxs-lookup"><span data-stu-id="11484-159">pages</span></span>|<span data-ttu-id="11484-160">coleção [onenotePage](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="11484-160">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="11484-161">Obtém o conjunto de páginas da seção.</span><span class="sxs-lookup"><span data-stu-id="11484-161">The collection of pages in the section.</span></span>  <span data-ttu-id="11484-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11484-162">Read-only.</span></span> <span data-ttu-id="11484-163">Anulável.</span><span class="sxs-lookup"><span data-stu-id="11484-163">Nullable.</span></span>|
|<span data-ttu-id="11484-164">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="11484-164">parentNotebook</span></span>|[<span data-ttu-id="11484-165">anotações</span><span class="sxs-lookup"><span data-stu-id="11484-165">notebook</span></span>](notebook.md)|<span data-ttu-id="11484-166">O bloco de anotações que contém a seção.</span><span class="sxs-lookup"><span data-stu-id="11484-166">The notebook that contains the section.</span></span>  <span data-ttu-id="11484-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11484-167">Read-only.</span></span>|
|<span data-ttu-id="11484-168">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="11484-168">parentSectionGroup</span></span>|[<span data-ttu-id="11484-169">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="11484-169">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="11484-170">O grupo de seções que contém a seção.</span><span class="sxs-lookup"><span data-stu-id="11484-170">The section group that contains the section.</span></span>  <span data-ttu-id="11484-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11484-171">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="11484-172">Métodos</span><span class="sxs-lookup"><span data-stu-id="11484-172">Methods</span></span>

| <span data-ttu-id="11484-173">Método</span><span class="sxs-lookup"><span data-stu-id="11484-173">Method</span></span>           | <span data-ttu-id="11484-174">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="11484-174">Return Type</span></span>    |<span data-ttu-id="11484-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="11484-175">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="11484-176">Obter seção</span><span class="sxs-lookup"><span data-stu-id="11484-176">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="11484-177">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="11484-177">onenoteSection</span></span>](onenotesection.md) |<span data-ttu-id="11484-178">Leia as propriedades e as relações da seção.</span><span class="sxs-lookup"><span data-stu-id="11484-178">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="11484-179">Create page</span><span class="sxs-lookup"><span data-stu-id="11484-179">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="11484-180">onenotePage</span><span class="sxs-lookup"><span data-stu-id="11484-180">onenotePage</span></span>](onenotepage.md)| <span data-ttu-id="11484-181">Crie uma página postando na coleção Pages na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="11484-181">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="11484-182">Listar páginas</span><span class="sxs-lookup"><span data-stu-id="11484-182">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="11484-183">coleção [onenotePage](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="11484-183">[onenotePage](onenotepage.md) collection</span></span>| <span data-ttu-id="11484-184">Obtém uma coleção de páginas na seção especificada.</span><span class="sxs-lookup"><span data-stu-id="11484-184">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="11484-185">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="11484-185">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="11484-186">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11484-186">None</span></span>|<span data-ttu-id="11484-187">Copie a seção para um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="11484-187">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="11484-188">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="11484-188">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="11484-189">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11484-189">None</span></span>|<span data-ttu-id="11484-190">Copie a seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="11484-190">Copy the section to a specific section group.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="11484-191">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11484-191">JSON representation</span></span>

<span data-ttu-id="11484-192">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11484-192">Here is a JSON representation of the resource.</span></span>

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
