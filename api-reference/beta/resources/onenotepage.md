---
title: tipo de recurso onenotePage
description: Uma página em um bloco de anotações do OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: d219677c70be566b5039a39c5421c91a9ab11c8c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809366"
---
# <a name="onenotepage-resource-type"></a><span data-ttu-id="1f85e-103">tipo de recurso onenotePage</span><span class="sxs-lookup"><span data-stu-id="1f85e-103">onenotePage resource type</span></span>

<span data-ttu-id="1f85e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f85e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f85e-105">Uma página em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="1f85e-105">A page in a OneNote notebook.</span></span>

## <a name="properties"></a><span data-ttu-id="1f85e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f85e-106">Properties</span></span>
| <span data-ttu-id="1f85e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f85e-107">Property</span></span>     | <span data-ttu-id="1f85e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f85e-108">Type</span></span>   |<span data-ttu-id="1f85e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f85e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f85e-110">conteúdo</span><span class="sxs-lookup"><span data-stu-id="1f85e-110">content</span></span>|<span data-ttu-id="1f85e-111">Fluxo</span><span class="sxs-lookup"><span data-stu-id="1f85e-111">Stream</span></span>|<span data-ttu-id="1f85e-112">O conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="1f85e-112">The page's HTML content.</span></span>|
|<span data-ttu-id="1f85e-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="1f85e-113">contentUrl</span></span>|<span data-ttu-id="1f85e-114">String</span><span class="sxs-lookup"><span data-stu-id="1f85e-114">String</span></span>|<span data-ttu-id="1f85e-115">A URL do conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="1f85e-115">The URL for the page's HTML content.</span></span>  <span data-ttu-id="1f85e-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f85e-116">Read-only.</span></span>|
|<span data-ttu-id="1f85e-117">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="1f85e-117">createdByAppId</span></span>|<span data-ttu-id="1f85e-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f85e-118">String</span></span>|<span data-ttu-id="1f85e-119">O identificador exclusivo do aplicativo que criou a página.</span><span class="sxs-lookup"><span data-stu-id="1f85e-119">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="1f85e-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f85e-120">Read-only.</span></span>|
|<span data-ttu-id="1f85e-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f85e-121">createdDateTime</span></span>|<span data-ttu-id="1f85e-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f85e-122">DateTimeOffset</span></span>|<span data-ttu-id="1f85e-123">A data e a hora em que a página foi criada.</span><span class="sxs-lookup"><span data-stu-id="1f85e-123">The date and time when the page was created.</span></span> <span data-ttu-id="1f85e-124">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1f85e-124">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1f85e-125">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1f85e-125">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="1f85e-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f85e-126">Read-only.</span></span>|
|<span data-ttu-id="1f85e-127">id</span><span class="sxs-lookup"><span data-stu-id="1f85e-127">id</span></span>|<span data-ttu-id="1f85e-128">String</span><span class="sxs-lookup"><span data-stu-id="1f85e-128">String</span></span>|<span data-ttu-id="1f85e-129">O identificador exclusivo da página.</span><span class="sxs-lookup"><span data-stu-id="1f85e-129">The unique identifier of the page.</span></span>  <span data-ttu-id="1f85e-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f85e-130">Read-only.</span></span>|
|<span data-ttu-id="1f85e-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f85e-131">lastModifiedDateTime</span></span>|<span data-ttu-id="1f85e-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f85e-132">DateTimeOffset</span></span>|<span data-ttu-id="1f85e-133">A data e a hora em que a página foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1f85e-133">The date and time when the page was last modified.</span></span> <span data-ttu-id="1f85e-134">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1f85e-134">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1f85e-135">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1f85e-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="1f85e-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f85e-136">Read-only.</span></span>|
|<span data-ttu-id="1f85e-137">antes</span><span class="sxs-lookup"><span data-stu-id="1f85e-137">level</span></span>|<span data-ttu-id="1f85e-138">Int32</span><span class="sxs-lookup"><span data-stu-id="1f85e-138">Int32</span></span>|<span data-ttu-id="1f85e-139">O nível de recuo da página.</span><span class="sxs-lookup"><span data-stu-id="1f85e-139">The indentation level of the page.</span></span> <span data-ttu-id="1f85e-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f85e-140">Read-only.</span></span>|
|<span data-ttu-id="1f85e-141">links</span><span class="sxs-lookup"><span data-stu-id="1f85e-141">links</span></span>|[<span data-ttu-id="1f85e-142">pageLinks</span><span class="sxs-lookup"><span data-stu-id="1f85e-142">pageLinks</span></span>](pagelinks.md)|<span data-ttu-id="1f85e-143">Links para abrir a página.</span><span class="sxs-lookup"><span data-stu-id="1f85e-143">Links for opening the page.</span></span> <span data-ttu-id="1f85e-144">O `oneNoteClientURL` link abre a página no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="1f85e-144">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="1f85e-145">O `oneNoteWebUrl` link abre a página no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="1f85e-145">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="1f85e-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f85e-146">Read-only.</span></span>|
|<span data-ttu-id="1f85e-147">Ordene</span><span class="sxs-lookup"><span data-stu-id="1f85e-147">order</span></span>|<span data-ttu-id="1f85e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="1f85e-148">Int32</span></span>|<span data-ttu-id="1f85e-149">A ordem da página dentro da seção pai.</span><span class="sxs-lookup"><span data-stu-id="1f85e-149">The order of the page within its parent section.</span></span> <span data-ttu-id="1f85e-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f85e-150">Read-only.</span></span>|
|<span data-ttu-id="1f85e-151">própria</span><span class="sxs-lookup"><span data-stu-id="1f85e-151">self</span></span>|<span data-ttu-id="1f85e-152">String</span><span class="sxs-lookup"><span data-stu-id="1f85e-152">String</span></span>|<span data-ttu-id="1f85e-153">O ponto de extremidade onde você pode obter detalhes sobre a página.</span><span class="sxs-lookup"><span data-stu-id="1f85e-153">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="1f85e-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f85e-154">Read-only.</span></span>|
|<span data-ttu-id="1f85e-155">title</span><span class="sxs-lookup"><span data-stu-id="1f85e-155">title</span></span>|<span data-ttu-id="1f85e-156">String</span><span class="sxs-lookup"><span data-stu-id="1f85e-156">String</span></span>|<span data-ttu-id="1f85e-157">O título da página.</span><span class="sxs-lookup"><span data-stu-id="1f85e-157">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1f85e-158">Relações</span><span class="sxs-lookup"><span data-stu-id="1f85e-158">Relationships</span></span>
| <span data-ttu-id="1f85e-159">Relação</span><span class="sxs-lookup"><span data-stu-id="1f85e-159">Relationship</span></span> | <span data-ttu-id="1f85e-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f85e-160">Type</span></span>   |<span data-ttu-id="1f85e-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f85e-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f85e-162">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="1f85e-162">parentNotebook</span></span>|[<span data-ttu-id="1f85e-163">bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="1f85e-163">notebook</span></span>](notebook.md)|<span data-ttu-id="1f85e-164">O bloco de anotações que contém a página.</span><span class="sxs-lookup"><span data-stu-id="1f85e-164">The notebook that contains the page.</span></span>  <span data-ttu-id="1f85e-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f85e-165">Read-only.</span></span>|
|<span data-ttu-id="1f85e-166">parentSection</span><span class="sxs-lookup"><span data-stu-id="1f85e-166">parentSection</span></span>|[<span data-ttu-id="1f85e-167">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="1f85e-167">onenoteSection</span></span>](onenotesection.md)|<span data-ttu-id="1f85e-168">A seção que contém a página.</span><span class="sxs-lookup"><span data-stu-id="1f85e-168">The section that contains the page.</span></span> <span data-ttu-id="1f85e-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f85e-169">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="1f85e-170">Métodos</span><span class="sxs-lookup"><span data-stu-id="1f85e-170">Methods</span></span>

| <span data-ttu-id="1f85e-171">Método</span><span class="sxs-lookup"><span data-stu-id="1f85e-171">Method</span></span>           | <span data-ttu-id="1f85e-172">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1f85e-172">Return Type</span></span>    |<span data-ttu-id="1f85e-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f85e-173">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1f85e-174">Obter página</span><span class="sxs-lookup"><span data-stu-id="1f85e-174">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="1f85e-175">onenotePage</span><span class="sxs-lookup"><span data-stu-id="1f85e-175">onenotePage</span></span>](onenotepage.md) |<span data-ttu-id="1f85e-176">Leia as propriedades e as relações da página.</span><span class="sxs-lookup"><span data-stu-id="1f85e-176">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="1f85e-177">Atualizar conteúdo da página</span><span class="sxs-lookup"><span data-stu-id="1f85e-177">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="1f85e-178">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f85e-178">None</span></span> |<span data-ttu-id="1f85e-179">Atualize o conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="1f85e-179">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="1f85e-180">Excluir página</span><span class="sxs-lookup"><span data-stu-id="1f85e-180">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="1f85e-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f85e-181">None</span></span> |<span data-ttu-id="1f85e-182">Exclua a página.</span><span class="sxs-lookup"><span data-stu-id="1f85e-182">Delete the page.</span></span> |
|[<span data-ttu-id="1f85e-183">copyToSection</span><span class="sxs-lookup"><span data-stu-id="1f85e-183">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="1f85e-184">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f85e-184">None</span></span> |<span data-ttu-id="1f85e-185">Copia a página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="1f85e-185">Copies the page to a specific section.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1f85e-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f85e-186">JSON representation</span></span>

<span data-ttu-id="1f85e-187">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f85e-187">Here is a JSON representation of the resource.</span></span>

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
