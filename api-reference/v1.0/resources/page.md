---
title: tipo de recurso de página
description: Uma página em um bloco de anotações do OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6adb0197b5e8fbcaa71e88f66481ca18a11bbfeb
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721527"
---
# <a name="page-resource-type"></a><span data-ttu-id="251b1-103">tipo de recurso de página</span><span class="sxs-lookup"><span data-stu-id="251b1-103">page resource type</span></span>

<span data-ttu-id="251b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="251b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="251b1-105">Uma página em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="251b1-105">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="251b1-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="251b1-106">JSON representation</span></span>

<span data-ttu-id="251b1-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="251b1-107">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "isMediaEntity": true,
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
## <a name="properties"></a><span data-ttu-id="251b1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="251b1-108">Properties</span></span>
| <span data-ttu-id="251b1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="251b1-109">Property</span></span>     | <span data-ttu-id="251b1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="251b1-110">Type</span></span>   |<span data-ttu-id="251b1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="251b1-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="251b1-112">conteúdo</span><span class="sxs-lookup"><span data-stu-id="251b1-112">content</span></span>|<span data-ttu-id="251b1-113">Fluxo</span><span class="sxs-lookup"><span data-stu-id="251b1-113">Stream</span></span>|<span data-ttu-id="251b1-114">Conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="251b1-114">The page's HTML content.</span></span>|
|<span data-ttu-id="251b1-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="251b1-115">contentUrl</span></span>|<span data-ttu-id="251b1-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="251b1-116">String</span></span>|<span data-ttu-id="251b1-117">A URL do conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="251b1-117">The URL for the page's HTML content.</span></span>  <span data-ttu-id="251b1-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="251b1-118">Read-only.</span></span>|
|<span data-ttu-id="251b1-119">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="251b1-119">createdByAppId</span></span>|<span data-ttu-id="251b1-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="251b1-120">String</span></span>|<span data-ttu-id="251b1-121">O identificador exclusivo do aplicativo que criou a página.</span><span class="sxs-lookup"><span data-stu-id="251b1-121">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="251b1-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="251b1-122">Read-only.</span></span>|
|<span data-ttu-id="251b1-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="251b1-123">createdDateTime</span></span>|<span data-ttu-id="251b1-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="251b1-124">DateTimeOffset</span></span>|<span data-ttu-id="251b1-125">A data e a hora em que a página foi criada.</span><span class="sxs-lookup"><span data-stu-id="251b1-125">The date and time when the page was created.</span></span> <span data-ttu-id="251b1-126">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="251b1-126">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="251b1-127">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="251b1-127">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="251b1-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="251b1-128">Read-only.</span></span>|
|<span data-ttu-id="251b1-129">id</span><span class="sxs-lookup"><span data-stu-id="251b1-129">id</span></span>|<span data-ttu-id="251b1-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="251b1-130">String</span></span>|<span data-ttu-id="251b1-131">O identificador exclusivo da página.</span><span class="sxs-lookup"><span data-stu-id="251b1-131">The unique identifier of the page.</span></span>  <span data-ttu-id="251b1-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="251b1-132">Read-only.</span></span>|
|<span data-ttu-id="251b1-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="251b1-133">lastModifiedDateTime</span></span>|<span data-ttu-id="251b1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="251b1-134">DateTimeOffset</span></span>|<span data-ttu-id="251b1-135">A data e a hora em que a página foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="251b1-135">The date and time when the page was last modified.</span></span> <span data-ttu-id="251b1-136">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="251b1-136">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="251b1-137">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="251b1-137">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="251b1-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="251b1-138">Read-only.</span></span>|
|<span data-ttu-id="251b1-139">level</span><span class="sxs-lookup"><span data-stu-id="251b1-139">level</span></span>|<span data-ttu-id="251b1-140">Int32</span><span class="sxs-lookup"><span data-stu-id="251b1-140">Int32</span></span>|<span data-ttu-id="251b1-141">O nível de recuo da página.</span><span class="sxs-lookup"><span data-stu-id="251b1-141">The indentation level of the page.</span></span> <span data-ttu-id="251b1-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="251b1-142">Read-only.</span></span>|
|<span data-ttu-id="251b1-143">links</span><span class="sxs-lookup"><span data-stu-id="251b1-143">links</span></span>|[<span data-ttu-id="251b1-144">PageLinks</span><span class="sxs-lookup"><span data-stu-id="251b1-144">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="251b1-145">Links para abrir a página.</span><span class="sxs-lookup"><span data-stu-id="251b1-145">Links for opening the page.</span></span> <span data-ttu-id="251b1-146">O `oneNoteClientURL` link abre a página no cliente nativo do OneNote se estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="251b1-146">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="251b1-147">O `oneNoteWebUrl` link abre a página no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="251b1-147">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="251b1-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="251b1-148">Read-only.</span></span>|
|<span data-ttu-id="251b1-149">order</span><span class="sxs-lookup"><span data-stu-id="251b1-149">order</span></span>|<span data-ttu-id="251b1-150">Int32</span><span class="sxs-lookup"><span data-stu-id="251b1-150">Int32</span></span>|<span data-ttu-id="251b1-151">A ordem da página em sua seção pai.</span><span class="sxs-lookup"><span data-stu-id="251b1-151">The order of the page within its parent section.</span></span> <span data-ttu-id="251b1-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="251b1-152">Read-only.</span></span>|
|<span data-ttu-id="251b1-153">self</span><span class="sxs-lookup"><span data-stu-id="251b1-153">self</span></span>|<span data-ttu-id="251b1-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="251b1-154">String</span></span>|<span data-ttu-id="251b1-155">O ponto de extremidade onde você pode obter detalhes sobre a página.</span><span class="sxs-lookup"><span data-stu-id="251b1-155">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="251b1-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="251b1-156">Read-only.</span></span>|
|<span data-ttu-id="251b1-157">title</span><span class="sxs-lookup"><span data-stu-id="251b1-157">title</span></span>|<span data-ttu-id="251b1-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="251b1-158">String</span></span>|<span data-ttu-id="251b1-159">O título da página.</span><span class="sxs-lookup"><span data-stu-id="251b1-159">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="251b1-160">Relações</span><span class="sxs-lookup"><span data-stu-id="251b1-160">Relationships</span></span>
| <span data-ttu-id="251b1-161">Relação</span><span class="sxs-lookup"><span data-stu-id="251b1-161">Relationship</span></span> | <span data-ttu-id="251b1-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="251b1-162">Type</span></span>   |<span data-ttu-id="251b1-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="251b1-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="251b1-164">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="251b1-164">parentNotebook</span></span>|[<span data-ttu-id="251b1-165">Notebook</span><span class="sxs-lookup"><span data-stu-id="251b1-165">Notebook</span></span>](notebook.md)|<span data-ttu-id="251b1-166">O bloco de anotações que contém a página.</span><span class="sxs-lookup"><span data-stu-id="251b1-166">The notebook that contains the page.</span></span>  <span data-ttu-id="251b1-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="251b1-167">Read-only.</span></span>|
|<span data-ttu-id="251b1-168">parentSection</span><span class="sxs-lookup"><span data-stu-id="251b1-168">parentSection</span></span>|[<span data-ttu-id="251b1-169">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="251b1-169">OnenoteSection</span></span>](section.md)|<span data-ttu-id="251b1-170">A seção que contém a página.</span><span class="sxs-lookup"><span data-stu-id="251b1-170">The section that contains the page.</span></span> <span data-ttu-id="251b1-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="251b1-171">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="251b1-172">Methods</span><span class="sxs-lookup"><span data-stu-id="251b1-172">Methods</span></span>

| <span data-ttu-id="251b1-173">Método</span><span class="sxs-lookup"><span data-stu-id="251b1-173">Method</span></span>           | <span data-ttu-id="251b1-174">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="251b1-174">Return Type</span></span>    |<span data-ttu-id="251b1-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="251b1-175">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="251b1-176">Obter página</span><span class="sxs-lookup"><span data-stu-id="251b1-176">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="251b1-177">Page</span><span class="sxs-lookup"><span data-stu-id="251b1-177">Page</span></span>](page.md) |<span data-ttu-id="251b1-178">Leia as propriedades e as relações da página.</span><span class="sxs-lookup"><span data-stu-id="251b1-178">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="251b1-179">Atualizar conteúdo da página</span><span class="sxs-lookup"><span data-stu-id="251b1-179">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="251b1-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="251b1-180">None</span></span> |<span data-ttu-id="251b1-181">Atualize o conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="251b1-181">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="251b1-182">Excluir página</span><span class="sxs-lookup"><span data-stu-id="251b1-182">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="251b1-183">Nenhum</span><span class="sxs-lookup"><span data-stu-id="251b1-183">None</span></span> |<span data-ttu-id="251b1-184">Exclua a página.</span><span class="sxs-lookup"><span data-stu-id="251b1-184">Delete the page.</span></span> |
|[<span data-ttu-id="251b1-185">copyToSection</span><span class="sxs-lookup"><span data-stu-id="251b1-185">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="251b1-186">Nenhum</span><span class="sxs-lookup"><span data-stu-id="251b1-186">None</span></span> |<span data-ttu-id="251b1-187">Copia a página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="251b1-187">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

