---
title: tipo de recurso onenotePage
description: Uma página em um bloco de anotações do OneNote.
localization_priority: Normal
ms.openlocfilehash: 70b500180185a2b449a2ebbaddb809772486f45e
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236591"
---
# <a name="onenotepage-resource-type"></a><span data-ttu-id="74342-103">tipo de recurso onenotePage</span><span class="sxs-lookup"><span data-stu-id="74342-103">onenotePage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74342-104">Uma página em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="74342-104">A page in a OneNote notebook.</span></span>

## <a name="properties"></a><span data-ttu-id="74342-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74342-105">Properties</span></span>
| <span data-ttu-id="74342-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74342-106">Property</span></span>     | <span data-ttu-id="74342-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="74342-107">Type</span></span>   |<span data-ttu-id="74342-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="74342-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74342-109">conteúdo</span><span class="sxs-lookup"><span data-stu-id="74342-109">content</span></span>|<span data-ttu-id="74342-110">Fluxo</span><span class="sxs-lookup"><span data-stu-id="74342-110">Stream</span></span>|<span data-ttu-id="74342-111">O conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="74342-111">The page's HTML content.</span></span>|
|<span data-ttu-id="74342-112">contentUrl</span><span class="sxs-lookup"><span data-stu-id="74342-112">contentUrl</span></span>|<span data-ttu-id="74342-113">String</span><span class="sxs-lookup"><span data-stu-id="74342-113">String</span></span>|<span data-ttu-id="74342-114">A URL do conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="74342-114">The URL for the page's HTML content.</span></span>  <span data-ttu-id="74342-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74342-115">Read-only.</span></span>|
|<span data-ttu-id="74342-116">Pela createdbyappid</span><span class="sxs-lookup"><span data-stu-id="74342-116">createdByAppId</span></span>|<span data-ttu-id="74342-117">String</span><span class="sxs-lookup"><span data-stu-id="74342-117">String</span></span>|<span data-ttu-id="74342-118">O identificador exclusivo do aplicativo que criou a página.</span><span class="sxs-lookup"><span data-stu-id="74342-118">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="74342-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74342-119">Read-only.</span></span>|
|<span data-ttu-id="74342-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74342-120">createdDateTime</span></span>|<span data-ttu-id="74342-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74342-121">DateTimeOffset</span></span>|<span data-ttu-id="74342-122">A data e a hora em que a página foi criada.</span><span class="sxs-lookup"><span data-stu-id="74342-122">The date and time when the page was created.</span></span> <span data-ttu-id="74342-123">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="74342-123">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="74342-124">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="74342-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="74342-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74342-125">Read-only.</span></span>|
|<span data-ttu-id="74342-126">id</span><span class="sxs-lookup"><span data-stu-id="74342-126">id</span></span>|<span data-ttu-id="74342-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74342-127">String</span></span>|<span data-ttu-id="74342-128">O identificador exclusivo da página.</span><span class="sxs-lookup"><span data-stu-id="74342-128">The unique identifier of the page.</span></span>  <span data-ttu-id="74342-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74342-129">Read-only.</span></span>|
|<span data-ttu-id="74342-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74342-130">lastModifiedDateTime</span></span>|<span data-ttu-id="74342-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74342-131">DateTimeOffset</span></span>|<span data-ttu-id="74342-132">A data e a hora em que a página foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="74342-132">The date and time when the page was last modified.</span></span> <span data-ttu-id="74342-133">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="74342-133">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="74342-134">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="74342-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="74342-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74342-135">Read-only.</span></span>|
|<span data-ttu-id="74342-136">antes</span><span class="sxs-lookup"><span data-stu-id="74342-136">level</span></span>|<span data-ttu-id="74342-137">Int32</span><span class="sxs-lookup"><span data-stu-id="74342-137">Int32</span></span>|<span data-ttu-id="74342-138">O nível de recuo da página.</span><span class="sxs-lookup"><span data-stu-id="74342-138">The indentation level of the page.</span></span> <span data-ttu-id="74342-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74342-139">Read-only.</span></span>|
|<span data-ttu-id="74342-140">links</span><span class="sxs-lookup"><span data-stu-id="74342-140">links</span></span>|[<span data-ttu-id="74342-141">pageLinks</span><span class="sxs-lookup"><span data-stu-id="74342-141">pageLinks</span></span>](pagelinks.md)|<span data-ttu-id="74342-142">Links para abrir a página.</span><span class="sxs-lookup"><span data-stu-id="74342-142">Links for opening the page.</span></span> <span data-ttu-id="74342-143">O `oneNoteClientURL` link abre a página no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="74342-143">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="74342-144">O `oneNoteWebUrl` link abre a página no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="74342-144">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="74342-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74342-145">Read-only.</span></span>|
|<span data-ttu-id="74342-146">Ordene</span><span class="sxs-lookup"><span data-stu-id="74342-146">order</span></span>|<span data-ttu-id="74342-147">Int32</span><span class="sxs-lookup"><span data-stu-id="74342-147">Int32</span></span>|<span data-ttu-id="74342-148">A ordem da página dentro da seção pai.</span><span class="sxs-lookup"><span data-stu-id="74342-148">The order of the page within its parent section.</span></span> <span data-ttu-id="74342-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74342-149">Read-only.</span></span>|
|<span data-ttu-id="74342-150">própria</span><span class="sxs-lookup"><span data-stu-id="74342-150">self</span></span>|<span data-ttu-id="74342-151">String</span><span class="sxs-lookup"><span data-stu-id="74342-151">String</span></span>|<span data-ttu-id="74342-152">O ponto de extremidade onde você pode obter detalhes sobre a página.</span><span class="sxs-lookup"><span data-stu-id="74342-152">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="74342-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74342-153">Read-only.</span></span>|
|<span data-ttu-id="74342-154">title</span><span class="sxs-lookup"><span data-stu-id="74342-154">title</span></span>|<span data-ttu-id="74342-155">String</span><span class="sxs-lookup"><span data-stu-id="74342-155">String</span></span>|<span data-ttu-id="74342-156">O título da página.</span><span class="sxs-lookup"><span data-stu-id="74342-156">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="74342-157">Relações</span><span class="sxs-lookup"><span data-stu-id="74342-157">Relationships</span></span>
| <span data-ttu-id="74342-158">Relação</span><span class="sxs-lookup"><span data-stu-id="74342-158">Relationship</span></span> | <span data-ttu-id="74342-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="74342-159">Type</span></span>   |<span data-ttu-id="74342-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="74342-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74342-161">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="74342-161">parentNotebook</span></span>|[<span data-ttu-id="74342-162">anotações</span><span class="sxs-lookup"><span data-stu-id="74342-162">notebook</span></span>](notebook.md)|<span data-ttu-id="74342-163">O bloco de anotações que contém a página.</span><span class="sxs-lookup"><span data-stu-id="74342-163">The notebook that contains the page.</span></span>  <span data-ttu-id="74342-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74342-164">Read-only.</span></span>|
|<span data-ttu-id="74342-165">parentSection</span><span class="sxs-lookup"><span data-stu-id="74342-165">parentSection</span></span>|[<span data-ttu-id="74342-166">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="74342-166">onenoteSection</span></span>](onenotesection.md)|<span data-ttu-id="74342-167">A seção que contém a página.</span><span class="sxs-lookup"><span data-stu-id="74342-167">The section that contains the page.</span></span> <span data-ttu-id="74342-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74342-168">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="74342-169">Métodos</span><span class="sxs-lookup"><span data-stu-id="74342-169">Methods</span></span>

| <span data-ttu-id="74342-170">Método</span><span class="sxs-lookup"><span data-stu-id="74342-170">Method</span></span>           | <span data-ttu-id="74342-171">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="74342-171">Return Type</span></span>    |<span data-ttu-id="74342-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="74342-172">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74342-173">Obter página</span><span class="sxs-lookup"><span data-stu-id="74342-173">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="74342-174">onenotePage</span><span class="sxs-lookup"><span data-stu-id="74342-174">onenotePage</span></span>](onenotepage.md) |<span data-ttu-id="74342-175">Leia as propriedades e as relações da página.</span><span class="sxs-lookup"><span data-stu-id="74342-175">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="74342-176">Atualizar conteúdo da página</span><span class="sxs-lookup"><span data-stu-id="74342-176">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="74342-177">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74342-177">None</span></span> |<span data-ttu-id="74342-178">Atualize o conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="74342-178">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="74342-179">Excluir página</span><span class="sxs-lookup"><span data-stu-id="74342-179">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="74342-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74342-180">None</span></span> |<span data-ttu-id="74342-181">Exclua a página.</span><span class="sxs-lookup"><span data-stu-id="74342-181">Delete the page.</span></span> |
|[<span data-ttu-id="74342-182">copyToSection</span><span class="sxs-lookup"><span data-stu-id="74342-182">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="74342-183">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74342-183">None</span></span> |<span data-ttu-id="74342-184">Copia a página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="74342-184">Copies the page to a specific section.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74342-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74342-185">JSON representation</span></span>

<span data-ttu-id="74342-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74342-186">Here is a JSON representation of the resource.</span></span>

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
