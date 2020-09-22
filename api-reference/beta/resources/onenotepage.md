---
title: tipo de recurso onenotePage
description: Uma página em um bloco de anotações do OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: 463ac02029753fcc99392fbc3db464989f5ae01a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971533"
---
# <a name="onenotepage-resource-type"></a><span data-ttu-id="b28c8-103">tipo de recurso onenotePage</span><span class="sxs-lookup"><span data-stu-id="b28c8-103">onenotePage resource type</span></span>

<span data-ttu-id="b28c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b28c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b28c8-105">Uma página em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="b28c8-105">A page in a OneNote notebook.</span></span>

## <a name="properties"></a><span data-ttu-id="b28c8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b28c8-106">Properties</span></span>
| <span data-ttu-id="b28c8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b28c8-107">Property</span></span>     | <span data-ttu-id="b28c8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b28c8-108">Type</span></span>   |<span data-ttu-id="b28c8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b28c8-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b28c8-110">conteúdo</span><span class="sxs-lookup"><span data-stu-id="b28c8-110">content</span></span>|<span data-ttu-id="b28c8-111">Fluxo</span><span class="sxs-lookup"><span data-stu-id="b28c8-111">Stream</span></span>|<span data-ttu-id="b28c8-112">O conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="b28c8-112">The page's HTML content.</span></span>|
|<span data-ttu-id="b28c8-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="b28c8-113">contentUrl</span></span>|<span data-ttu-id="b28c8-114">String</span><span class="sxs-lookup"><span data-stu-id="b28c8-114">String</span></span>|<span data-ttu-id="b28c8-115">A URL do conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="b28c8-115">The URL for the page's HTML content.</span></span>  <span data-ttu-id="b28c8-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b28c8-116">Read-only.</span></span>|
|<span data-ttu-id="b28c8-117">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="b28c8-117">createdByAppId</span></span>|<span data-ttu-id="b28c8-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b28c8-118">String</span></span>|<span data-ttu-id="b28c8-119">O identificador exclusivo do aplicativo que criou a página.</span><span class="sxs-lookup"><span data-stu-id="b28c8-119">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="b28c8-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b28c8-120">Read-only.</span></span>|
|<span data-ttu-id="b28c8-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b28c8-121">createdDateTime</span></span>|<span data-ttu-id="b28c8-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b28c8-122">DateTimeOffset</span></span>|<span data-ttu-id="b28c8-123">A data e a hora em que a página foi criada.</span><span class="sxs-lookup"><span data-stu-id="b28c8-123">The date and time when the page was created.</span></span> <span data-ttu-id="b28c8-124">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b28c8-124">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b28c8-125">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b28c8-125">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b28c8-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b28c8-126">Read-only.</span></span>|
|<span data-ttu-id="b28c8-127">id</span><span class="sxs-lookup"><span data-stu-id="b28c8-127">id</span></span>|<span data-ttu-id="b28c8-128">String</span><span class="sxs-lookup"><span data-stu-id="b28c8-128">String</span></span>|<span data-ttu-id="b28c8-129">O identificador exclusivo da página.</span><span class="sxs-lookup"><span data-stu-id="b28c8-129">The unique identifier of the page.</span></span>  <span data-ttu-id="b28c8-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b28c8-130">Read-only.</span></span>|
|<span data-ttu-id="b28c8-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b28c8-131">lastModifiedDateTime</span></span>|<span data-ttu-id="b28c8-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b28c8-132">DateTimeOffset</span></span>|<span data-ttu-id="b28c8-133">A data e a hora em que a página foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b28c8-133">The date and time when the page was last modified.</span></span> <span data-ttu-id="b28c8-134">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b28c8-134">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b28c8-135">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b28c8-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b28c8-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b28c8-136">Read-only.</span></span>|
|<span data-ttu-id="b28c8-137">antes</span><span class="sxs-lookup"><span data-stu-id="b28c8-137">level</span></span>|<span data-ttu-id="b28c8-138">Int32</span><span class="sxs-lookup"><span data-stu-id="b28c8-138">Int32</span></span>|<span data-ttu-id="b28c8-139">O nível de recuo da página.</span><span class="sxs-lookup"><span data-stu-id="b28c8-139">The indentation level of the page.</span></span> <span data-ttu-id="b28c8-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b28c8-140">Read-only.</span></span>|
|<span data-ttu-id="b28c8-141">links</span><span class="sxs-lookup"><span data-stu-id="b28c8-141">links</span></span>|[<span data-ttu-id="b28c8-142">pageLinks</span><span class="sxs-lookup"><span data-stu-id="b28c8-142">pageLinks</span></span>](pagelinks.md)|<span data-ttu-id="b28c8-143">Links para abrir a página.</span><span class="sxs-lookup"><span data-stu-id="b28c8-143">Links for opening the page.</span></span> <span data-ttu-id="b28c8-144">O `oneNoteClientURL` link abre a página no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="b28c8-144">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="b28c8-145">O `oneNoteWebUrl` link abre a página no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="b28c8-145">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="b28c8-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b28c8-146">Read-only.</span></span>|
|<span data-ttu-id="b28c8-147">Ordene</span><span class="sxs-lookup"><span data-stu-id="b28c8-147">order</span></span>|<span data-ttu-id="b28c8-148">Int32</span><span class="sxs-lookup"><span data-stu-id="b28c8-148">Int32</span></span>|<span data-ttu-id="b28c8-149">A ordem da página dentro da seção pai.</span><span class="sxs-lookup"><span data-stu-id="b28c8-149">The order of the page within its parent section.</span></span> <span data-ttu-id="b28c8-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b28c8-150">Read-only.</span></span>|
|<span data-ttu-id="b28c8-151">própria</span><span class="sxs-lookup"><span data-stu-id="b28c8-151">self</span></span>|<span data-ttu-id="b28c8-152">String</span><span class="sxs-lookup"><span data-stu-id="b28c8-152">String</span></span>|<span data-ttu-id="b28c8-153">O ponto de extremidade onde você pode obter detalhes sobre a página.</span><span class="sxs-lookup"><span data-stu-id="b28c8-153">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="b28c8-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b28c8-154">Read-only.</span></span>|
|<span data-ttu-id="b28c8-155">title</span><span class="sxs-lookup"><span data-stu-id="b28c8-155">title</span></span>|<span data-ttu-id="b28c8-156">String</span><span class="sxs-lookup"><span data-stu-id="b28c8-156">String</span></span>|<span data-ttu-id="b28c8-157">O título da página.</span><span class="sxs-lookup"><span data-stu-id="b28c8-157">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b28c8-158">Relações</span><span class="sxs-lookup"><span data-stu-id="b28c8-158">Relationships</span></span>
| <span data-ttu-id="b28c8-159">Relação</span><span class="sxs-lookup"><span data-stu-id="b28c8-159">Relationship</span></span> | <span data-ttu-id="b28c8-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="b28c8-160">Type</span></span>   |<span data-ttu-id="b28c8-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="b28c8-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b28c8-162">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="b28c8-162">parentNotebook</span></span>|[<span data-ttu-id="b28c8-163">bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="b28c8-163">notebook</span></span>](notebook.md)|<span data-ttu-id="b28c8-164">O bloco de anotações que contém a página.</span><span class="sxs-lookup"><span data-stu-id="b28c8-164">The notebook that contains the page.</span></span>  <span data-ttu-id="b28c8-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b28c8-165">Read-only.</span></span>|
|<span data-ttu-id="b28c8-166">parentSection</span><span class="sxs-lookup"><span data-stu-id="b28c8-166">parentSection</span></span>|[<span data-ttu-id="b28c8-167">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="b28c8-167">onenoteSection</span></span>](onenotesection.md)|<span data-ttu-id="b28c8-168">A seção que contém a página.</span><span class="sxs-lookup"><span data-stu-id="b28c8-168">The section that contains the page.</span></span> <span data-ttu-id="b28c8-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b28c8-169">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="b28c8-170">Methods</span><span class="sxs-lookup"><span data-stu-id="b28c8-170">Methods</span></span>

| <span data-ttu-id="b28c8-171">Método</span><span class="sxs-lookup"><span data-stu-id="b28c8-171">Method</span></span>           | <span data-ttu-id="b28c8-172">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b28c8-172">Return Type</span></span>    |<span data-ttu-id="b28c8-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="b28c8-173">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b28c8-174">Obter página</span><span class="sxs-lookup"><span data-stu-id="b28c8-174">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="b28c8-175">onenotePage</span><span class="sxs-lookup"><span data-stu-id="b28c8-175">onenotePage</span></span>](onenotepage.md) |<span data-ttu-id="b28c8-176">Leia as propriedades e as relações da página.</span><span class="sxs-lookup"><span data-stu-id="b28c8-176">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="b28c8-177">Atualizar conteúdo da página</span><span class="sxs-lookup"><span data-stu-id="b28c8-177">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="b28c8-178">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b28c8-178">None</span></span> |<span data-ttu-id="b28c8-179">Atualize o conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="b28c8-179">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="b28c8-180">Excluir página</span><span class="sxs-lookup"><span data-stu-id="b28c8-180">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="b28c8-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b28c8-181">None</span></span> |<span data-ttu-id="b28c8-182">Exclua a página.</span><span class="sxs-lookup"><span data-stu-id="b28c8-182">Delete the page.</span></span> |
|[<span data-ttu-id="b28c8-183">copyToSection</span><span class="sxs-lookup"><span data-stu-id="b28c8-183">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="b28c8-184">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b28c8-184">None</span></span> |<span data-ttu-id="b28c8-185">Copia a página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="b28c8-185">Copies the page to a specific section.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b28c8-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b28c8-186">JSON representation</span></span>

<span data-ttu-id="b28c8-187">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b28c8-187">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


