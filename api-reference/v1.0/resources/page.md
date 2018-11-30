---
title: Tipo de recurso page
description: Uma página em um bloco de anotações do OneNote.
ms.openlocfilehash: 19380f06ad4706f623397681a020054e65eba029
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006753"
---
# <a name="page-resource-type"></a><span data-ttu-id="e4cc7-103">Tipo de recurso page</span><span class="sxs-lookup"><span data-stu-id="e4cc7-103">page resource type</span></span>

<span data-ttu-id="e4cc7-104">Uma página em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-104">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4cc7-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e4cc7-105">JSON representation</span></span>

<span data-ttu-id="e4cc7-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="e4cc7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e4cc7-107">Properties</span></span>
| <span data-ttu-id="e4cc7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4cc7-108">Property</span></span>     | <span data-ttu-id="e4cc7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4cc7-109">Type</span></span>   |<span data-ttu-id="e4cc7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4cc7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4cc7-111">content</span><span class="sxs-lookup"><span data-stu-id="e4cc7-111">content</span></span>|<span data-ttu-id="e4cc7-112">Fluxo</span><span class="sxs-lookup"><span data-stu-id="e4cc7-112">Stream</span></span>|<span data-ttu-id="e4cc7-113">O conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-113">The page's HTML content.</span></span>|
|<span data-ttu-id="e4cc7-114">contentUrl</span><span class="sxs-lookup"><span data-stu-id="e4cc7-114">contentUrl</span></span>|<span data-ttu-id="e4cc7-115">String</span><span class="sxs-lookup"><span data-stu-id="e4cc7-115">String</span></span>|<span data-ttu-id="e4cc7-p101">A URL do conteúdo HTML da página.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-p101">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="e4cc7-118">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="e4cc7-118">createdByAppId</span></span>|<span data-ttu-id="e4cc7-119">String</span><span class="sxs-lookup"><span data-stu-id="e4cc7-119">String</span></span>|<span data-ttu-id="e4cc7-p102">O identificador exclusivo do aplicativo que criou a página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-p102">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="e4cc7-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4cc7-122">createdDateTime</span></span>|<span data-ttu-id="e4cc7-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4cc7-123">DateTimeOffset</span></span>|<span data-ttu-id="e4cc7-p103">A data e a hora da criação da página. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-p103">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="e4cc7-128">id</span><span class="sxs-lookup"><span data-stu-id="e4cc7-128">id</span></span>|<span data-ttu-id="e4cc7-129">String</span><span class="sxs-lookup"><span data-stu-id="e4cc7-129">String</span></span>|<span data-ttu-id="e4cc7-p104">O identificador exclusivo da página.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-p104">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="e4cc7-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4cc7-132">lastModifiedDateTime</span></span>|<span data-ttu-id="e4cc7-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4cc7-133">DateTimeOffset</span></span>|<span data-ttu-id="e4cc7-p105">A data e a hora da última modificação da página. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-p105">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="e4cc7-138">nível</span><span class="sxs-lookup"><span data-stu-id="e4cc7-138">level</span></span>|<span data-ttu-id="e4cc7-139">Int32</span><span class="sxs-lookup"><span data-stu-id="e4cc7-139">Int32</span></span>|<span data-ttu-id="e4cc7-p106">O nível de recuo da página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-p106">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="e4cc7-142">links</span><span class="sxs-lookup"><span data-stu-id="e4cc7-142">links</span></span>|[<span data-ttu-id="e4cc7-143">PageLinks</span><span class="sxs-lookup"><span data-stu-id="e4cc7-143">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="e4cc7-p107">Links para abrir a página. O link `oneNoteClientURL` abre a página no cliente nativo do OneNote se ele estiver instalado. O link `oneNoteWebUrl` abre a página no OneNote Online. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-p107">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="e4cc7-148">ordem</span><span class="sxs-lookup"><span data-stu-id="e4cc7-148">order</span></span>|<span data-ttu-id="e4cc7-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e4cc7-149">Int32</span></span>|<span data-ttu-id="e4cc7-p108">A ordem da página dentro da seção pai dela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-p108">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="e4cc7-152">self</span><span class="sxs-lookup"><span data-stu-id="e4cc7-152">self</span></span>|<span data-ttu-id="e4cc7-153">String</span><span class="sxs-lookup"><span data-stu-id="e4cc7-153">String</span></span>|<span data-ttu-id="e4cc7-p109">O ponto de extremidade onde você pode obter detalhes sobre a página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-p109">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="e4cc7-156">title</span><span class="sxs-lookup"><span data-stu-id="e4cc7-156">title</span></span>|<span data-ttu-id="e4cc7-157">String</span><span class="sxs-lookup"><span data-stu-id="e4cc7-157">String</span></span>|<span data-ttu-id="e4cc7-158">O título da página.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-158">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e4cc7-159">Relações</span><span class="sxs-lookup"><span data-stu-id="e4cc7-159">Relationships</span></span>
| <span data-ttu-id="e4cc7-160">Relação</span><span class="sxs-lookup"><span data-stu-id="e4cc7-160">Relationship</span></span> | <span data-ttu-id="e4cc7-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4cc7-161">Type</span></span>   |<span data-ttu-id="e4cc7-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4cc7-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4cc7-163">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="e4cc7-163">parentNotebook</span></span>|[<span data-ttu-id="e4cc7-164">Notebook</span><span class="sxs-lookup"><span data-stu-id="e4cc7-164">Notebook</span></span>](notebook.md)|<span data-ttu-id="e4cc7-p110">O bloco de anotações que contém a página.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-p110">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="e4cc7-167">parentSection</span><span class="sxs-lookup"><span data-stu-id="e4cc7-167">parentSection</span></span>|[<span data-ttu-id="e4cc7-168">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="e4cc7-168">OnenoteSection</span></span>](section.md)|<span data-ttu-id="e4cc7-p111">A seção que contém a página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-p111">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="e4cc7-171">Métodos</span><span class="sxs-lookup"><span data-stu-id="e4cc7-171">Methods</span></span>

| <span data-ttu-id="e4cc7-172">Método</span><span class="sxs-lookup"><span data-stu-id="e4cc7-172">Method</span></span>           | <span data-ttu-id="e4cc7-173">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e4cc7-173">Return Type</span></span>    |<span data-ttu-id="e4cc7-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4cc7-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e4cc7-175">Get page</span><span class="sxs-lookup"><span data-stu-id="e4cc7-175">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="e4cc7-176">Página</span><span class="sxs-lookup"><span data-stu-id="e4cc7-176">Page</span></span>](page.md) |<span data-ttu-id="e4cc7-177">Leia as propriedades e as relações da página.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-177">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="e4cc7-178">Atualizar o conteúdo da página</span><span class="sxs-lookup"><span data-stu-id="e4cc7-178">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="e4cc7-179">None</span><span class="sxs-lookup"><span data-stu-id="e4cc7-179">None</span></span> |<span data-ttu-id="e4cc7-180">Atualizar o conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-180">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="e4cc7-181">Excluir página</span><span class="sxs-lookup"><span data-stu-id="e4cc7-181">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="e4cc7-182">None</span><span class="sxs-lookup"><span data-stu-id="e4cc7-182">None</span></span> |<span data-ttu-id="e4cc7-183">Exclua a página.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-183">Delete the page.</span></span> |
|[<span data-ttu-id="e4cc7-184">copyToSection</span><span class="sxs-lookup"><span data-stu-id="e4cc7-184">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="e4cc7-185">None</span><span class="sxs-lookup"><span data-stu-id="e4cc7-185">None</span></span> |<span data-ttu-id="e4cc7-186">Copia a página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="e4cc7-186">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->