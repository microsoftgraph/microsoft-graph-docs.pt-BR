---
title: tipo de recurso Page
description: Uma página em um bloco de anotações do OneNote.
localization_priority: Normal
ms.openlocfilehash: d8c27cdc144e9b192bd0205f256653ff7f04df5f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568546"
---
# <a name="page-resource-type"></a><span data-ttu-id="8877a-103">tipo de recurso Page</span><span class="sxs-lookup"><span data-stu-id="8877a-103">page resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8877a-104">Uma página em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="8877a-104">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8877a-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8877a-105">JSON representation</span></span>

<span data-ttu-id="8877a-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8877a-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "@odata.type": "microsoft.graph.onenotePage"
}-->

```json
{
  "content": "stream",
  "contentUrl": "string",
  "createdByAppId": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "level": 1024,
  "links": {"@odata.type": "microsoft.graph.pageLinks"},
  "order": 1024,
  "self": "string",
  "title": "string"
}

```
## <a name="properties"></a><span data-ttu-id="8877a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8877a-107">Properties</span></span>
| <span data-ttu-id="8877a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8877a-108">Property</span></span>     | <span data-ttu-id="8877a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8877a-109">Type</span></span>   |<span data-ttu-id="8877a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8877a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8877a-111">conteúdo</span><span class="sxs-lookup"><span data-stu-id="8877a-111">content</span></span>|<span data-ttu-id="8877a-112">Fluxo</span><span class="sxs-lookup"><span data-stu-id="8877a-112">Stream</span></span>|<span data-ttu-id="8877a-113">O conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="8877a-113">The page's HTML content.</span></span>|
|<span data-ttu-id="8877a-114">contentUrl</span><span class="sxs-lookup"><span data-stu-id="8877a-114">contentUrl</span></span>|<span data-ttu-id="8877a-115">String</span><span class="sxs-lookup"><span data-stu-id="8877a-115">String</span></span>|<span data-ttu-id="8877a-116">A URL do conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="8877a-116">The URL for the page's HTML content.</span></span>  <span data-ttu-id="8877a-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8877a-117">Read-only.</span></span>|
|<span data-ttu-id="8877a-118">Pela createdbyappid</span><span class="sxs-lookup"><span data-stu-id="8877a-118">createdByAppId</span></span>|<span data-ttu-id="8877a-119">String</span><span class="sxs-lookup"><span data-stu-id="8877a-119">String</span></span>|<span data-ttu-id="8877a-120">O identificador exclusivo do aplicativo que criou a página.</span><span class="sxs-lookup"><span data-stu-id="8877a-120">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="8877a-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8877a-121">Read-only.</span></span>|
|<span data-ttu-id="8877a-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8877a-122">createdDateTime</span></span>|<span data-ttu-id="8877a-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8877a-123">DateTimeOffset</span></span>|<span data-ttu-id="8877a-124">A data e a hora em que a página foi criada.</span><span class="sxs-lookup"><span data-stu-id="8877a-124">The date and time when the page was created.</span></span> <span data-ttu-id="8877a-125">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8877a-125">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8877a-126">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8877a-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="8877a-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8877a-127">Read-only.</span></span>|
|<span data-ttu-id="8877a-128">id</span><span class="sxs-lookup"><span data-stu-id="8877a-128">id</span></span>|<span data-ttu-id="8877a-129">String</span><span class="sxs-lookup"><span data-stu-id="8877a-129">String</span></span>|<span data-ttu-id="8877a-130">O identificador exclusivo da página.</span><span class="sxs-lookup"><span data-stu-id="8877a-130">The unique identifier of the page.</span></span>  <span data-ttu-id="8877a-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8877a-131">Read-only.</span></span>|
|<span data-ttu-id="8877a-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8877a-132">lastModifiedDateTime</span></span>|<span data-ttu-id="8877a-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8877a-133">DateTimeOffset</span></span>|<span data-ttu-id="8877a-134">A data e a hora em que a página foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8877a-134">The date and time when the page was last modified.</span></span> <span data-ttu-id="8877a-135">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8877a-135">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8877a-136">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8877a-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="8877a-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8877a-137">Read-only.</span></span>|
|<span data-ttu-id="8877a-138">level</span><span class="sxs-lookup"><span data-stu-id="8877a-138">level</span></span>|<span data-ttu-id="8877a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8877a-139">Int32</span></span>|<span data-ttu-id="8877a-140">O nível de recuo da página.</span><span class="sxs-lookup"><span data-stu-id="8877a-140">The indentation level of the page.</span></span> <span data-ttu-id="8877a-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8877a-141">Read-only.</span></span>|
|<span data-ttu-id="8877a-142">links</span><span class="sxs-lookup"><span data-stu-id="8877a-142">links</span></span>|[<span data-ttu-id="8877a-143">PageLinks</span><span class="sxs-lookup"><span data-stu-id="8877a-143">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="8877a-144">Links para abrir a página.</span><span class="sxs-lookup"><span data-stu-id="8877a-144">Links for opening the page.</span></span> <span data-ttu-id="8877a-145">O `oneNoteClientURL` link abre a página no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="8877a-145">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="8877a-146">O `oneNoteWebUrl` link abre a página no OneNote online.</span><span class="sxs-lookup"><span data-stu-id="8877a-146">The `oneNoteWebUrl` link opens the page in OneNote Online.</span></span> <span data-ttu-id="8877a-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8877a-147">Read-only.</span></span>|
|<span data-ttu-id="8877a-148">Ordene</span><span class="sxs-lookup"><span data-stu-id="8877a-148">order</span></span>|<span data-ttu-id="8877a-149">Int32</span><span class="sxs-lookup"><span data-stu-id="8877a-149">Int32</span></span>|<span data-ttu-id="8877a-150">A ordem da página dentro da seção pai.</span><span class="sxs-lookup"><span data-stu-id="8877a-150">The order of the page within its parent section.</span></span> <span data-ttu-id="8877a-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8877a-151">Read-only.</span></span>|
|<span data-ttu-id="8877a-152">própria</span><span class="sxs-lookup"><span data-stu-id="8877a-152">self</span></span>|<span data-ttu-id="8877a-153">String</span><span class="sxs-lookup"><span data-stu-id="8877a-153">String</span></span>|<span data-ttu-id="8877a-154">O ponto de extremidade onde você pode obter detalhes sobre a página.</span><span class="sxs-lookup"><span data-stu-id="8877a-154">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="8877a-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8877a-155">Read-only.</span></span>|
|<span data-ttu-id="8877a-156">title</span><span class="sxs-lookup"><span data-stu-id="8877a-156">title</span></span>|<span data-ttu-id="8877a-157">String</span><span class="sxs-lookup"><span data-stu-id="8877a-157">String</span></span>|<span data-ttu-id="8877a-158">O título da página.</span><span class="sxs-lookup"><span data-stu-id="8877a-158">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8877a-159">Relações</span><span class="sxs-lookup"><span data-stu-id="8877a-159">Relationships</span></span>
| <span data-ttu-id="8877a-160">Relação</span><span class="sxs-lookup"><span data-stu-id="8877a-160">Relationship</span></span> | <span data-ttu-id="8877a-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="8877a-161">Type</span></span>   |<span data-ttu-id="8877a-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="8877a-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8877a-163">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="8877a-163">parentNotebook</span></span>|[<span data-ttu-id="8877a-164">Bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="8877a-164">Notebook</span></span>](notebook.md)|<span data-ttu-id="8877a-165">O bloco de anotações que contém a página.</span><span class="sxs-lookup"><span data-stu-id="8877a-165">The notebook that contains the page.</span></span>  <span data-ttu-id="8877a-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8877a-166">Read-only.</span></span>|
|<span data-ttu-id="8877a-167">parentSection</span><span class="sxs-lookup"><span data-stu-id="8877a-167">parentSection</span></span>|[<span data-ttu-id="8877a-168">Section</span><span class="sxs-lookup"><span data-stu-id="8877a-168">Section</span></span>](section.md)|<span data-ttu-id="8877a-169">A seção que contém a página.</span><span class="sxs-lookup"><span data-stu-id="8877a-169">The section that contains the page.</span></span> <span data-ttu-id="8877a-170">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8877a-170">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="8877a-171">Métodos</span><span class="sxs-lookup"><span data-stu-id="8877a-171">Methods</span></span>

| <span data-ttu-id="8877a-172">Método</span><span class="sxs-lookup"><span data-stu-id="8877a-172">Method</span></span>           | <span data-ttu-id="8877a-173">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8877a-173">Return Type</span></span>    |<span data-ttu-id="8877a-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="8877a-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8877a-175">Obter página</span><span class="sxs-lookup"><span data-stu-id="8877a-175">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="8877a-176">Page</span><span class="sxs-lookup"><span data-stu-id="8877a-176">Page</span></span>](page.md) |<span data-ttu-id="8877a-177">Leia as propriedades e as relações da página.</span><span class="sxs-lookup"><span data-stu-id="8877a-177">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="8877a-178">Atualizar conteúdo da página</span><span class="sxs-lookup"><span data-stu-id="8877a-178">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="8877a-179">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8877a-179">None</span></span> |<span data-ttu-id="8877a-180">Atualize o conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="8877a-180">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="8877a-181">Excluir página</span><span class="sxs-lookup"><span data-stu-id="8877a-181">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="8877a-182">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8877a-182">None</span></span> |<span data-ttu-id="8877a-183">Exclua a página.</span><span class="sxs-lookup"><span data-stu-id="8877a-183">Delete the page.</span></span> |
|[<span data-ttu-id="8877a-184">copyToSection</span><span class="sxs-lookup"><span data-stu-id="8877a-184">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="8877a-185">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8877a-185">None</span></span> |<span data-ttu-id="8877a-186">Copia a página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="8877a-186">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/page.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
