---
title: Tipo de recurso page
description: Uma página em um bloco de anotações do OneNote.
ms.openlocfilehash: 82b9ca00cb4488c33e73daa94844b11f8de301cd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038650"
---
# <a name="page-resource-type"></a><span data-ttu-id="9f81d-103">Tipo de recurso page</span><span class="sxs-lookup"><span data-stu-id="9f81d-103">page resource type</span></span>

> <span data-ttu-id="9f81d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9f81d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f81d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9f81d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f81d-106">Uma página em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="9f81d-106">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f81d-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f81d-107">JSON representation</span></span>

<span data-ttu-id="9f81d-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f81d-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="9f81d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f81d-109">Properties</span></span>
| <span data-ttu-id="9f81d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f81d-110">Property</span></span>     | <span data-ttu-id="9f81d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f81d-111">Type</span></span>   |<span data-ttu-id="9f81d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f81d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f81d-113">content</span><span class="sxs-lookup"><span data-stu-id="9f81d-113">content</span></span>|<span data-ttu-id="9f81d-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="9f81d-114">Stream</span></span>|<span data-ttu-id="9f81d-115">O conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="9f81d-115">The page's HTML content.</span></span>|
|<span data-ttu-id="9f81d-116">contentUrl</span><span class="sxs-lookup"><span data-stu-id="9f81d-116">contentUrl</span></span>|<span data-ttu-id="9f81d-117">String</span><span class="sxs-lookup"><span data-stu-id="9f81d-117">String</span></span>|<span data-ttu-id="9f81d-p102">A URL do conteúdo HTML da página.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f81d-p102">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="9f81d-120">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="9f81d-120">createdByAppId</span></span>|<span data-ttu-id="9f81d-121">String</span><span class="sxs-lookup"><span data-stu-id="9f81d-121">String</span></span>|<span data-ttu-id="9f81d-p103">O identificador exclusivo do aplicativo que criou a página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f81d-p103">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="9f81d-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f81d-124">createdDateTime</span></span>|<span data-ttu-id="9f81d-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f81d-125">DateTimeOffset</span></span>|<span data-ttu-id="9f81d-p104">A data e a hora da criação da página. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f81d-p104">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="9f81d-130">id</span><span class="sxs-lookup"><span data-stu-id="9f81d-130">id</span></span>|<span data-ttu-id="9f81d-131">String</span><span class="sxs-lookup"><span data-stu-id="9f81d-131">String</span></span>|<span data-ttu-id="9f81d-p105">O identificador exclusivo da página.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f81d-p105">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="9f81d-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f81d-134">lastModifiedDateTime</span></span>|<span data-ttu-id="9f81d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f81d-135">DateTimeOffset</span></span>|<span data-ttu-id="9f81d-p106">A data e a hora da última modificação da página. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f81d-p106">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="9f81d-140">nível</span><span class="sxs-lookup"><span data-stu-id="9f81d-140">level</span></span>|<span data-ttu-id="9f81d-141">Int32</span><span class="sxs-lookup"><span data-stu-id="9f81d-141">Int32</span></span>|<span data-ttu-id="9f81d-p107">O nível de recuo da página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f81d-p107">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="9f81d-144">links</span><span class="sxs-lookup"><span data-stu-id="9f81d-144">links</span></span>|[<span data-ttu-id="9f81d-145">PageLinks</span><span class="sxs-lookup"><span data-stu-id="9f81d-145">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="9f81d-p108">Links para abrir a página. O link `oneNoteClientURL` abre a página no cliente nativo do OneNote se ele estiver instalado. O link `oneNoteWebUrl` abre a página no OneNote Online. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f81d-p108">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="9f81d-150">ordem</span><span class="sxs-lookup"><span data-stu-id="9f81d-150">order</span></span>|<span data-ttu-id="9f81d-151">Int32</span><span class="sxs-lookup"><span data-stu-id="9f81d-151">Int32</span></span>|<span data-ttu-id="9f81d-p109">A ordem da página dentro da seção pai dela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f81d-p109">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="9f81d-154">self</span><span class="sxs-lookup"><span data-stu-id="9f81d-154">self</span></span>|<span data-ttu-id="9f81d-155">String</span><span class="sxs-lookup"><span data-stu-id="9f81d-155">String</span></span>|<span data-ttu-id="9f81d-p110">O ponto de extremidade onde você pode obter detalhes sobre a página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f81d-p110">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="9f81d-158">title</span><span class="sxs-lookup"><span data-stu-id="9f81d-158">title</span></span>|<span data-ttu-id="9f81d-159">String</span><span class="sxs-lookup"><span data-stu-id="9f81d-159">String</span></span>|<span data-ttu-id="9f81d-160">O título da página.</span><span class="sxs-lookup"><span data-stu-id="9f81d-160">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9f81d-161">Relações</span><span class="sxs-lookup"><span data-stu-id="9f81d-161">Relationships</span></span>
| <span data-ttu-id="9f81d-162">Relação</span><span class="sxs-lookup"><span data-stu-id="9f81d-162">Relationship</span></span> | <span data-ttu-id="9f81d-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f81d-163">Type</span></span>   |<span data-ttu-id="9f81d-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f81d-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f81d-165">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="9f81d-165">parentNotebook</span></span>|[<span data-ttu-id="9f81d-166">Notebook</span><span class="sxs-lookup"><span data-stu-id="9f81d-166">Notebook</span></span>](notebook.md)|<span data-ttu-id="9f81d-p111">O bloco de anotações que contém a página.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f81d-p111">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="9f81d-169">parentSection</span><span class="sxs-lookup"><span data-stu-id="9f81d-169">parentSection</span></span>|[<span data-ttu-id="9f81d-170">Section</span><span class="sxs-lookup"><span data-stu-id="9f81d-170">Section</span></span>](section.md)|<span data-ttu-id="9f81d-p112">A seção que contém a página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f81d-p112">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="9f81d-173">Métodos</span><span class="sxs-lookup"><span data-stu-id="9f81d-173">Methods</span></span>

| <span data-ttu-id="9f81d-174">Método</span><span class="sxs-lookup"><span data-stu-id="9f81d-174">Method</span></span>           | <span data-ttu-id="9f81d-175">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9f81d-175">Return Type</span></span>    |<span data-ttu-id="9f81d-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f81d-176">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9f81d-177">Get page</span><span class="sxs-lookup"><span data-stu-id="9f81d-177">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="9f81d-178">Página</span><span class="sxs-lookup"><span data-stu-id="9f81d-178">Page</span></span>](page.md) |<span data-ttu-id="9f81d-179">Leia as propriedades e as relações da página.</span><span class="sxs-lookup"><span data-stu-id="9f81d-179">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="9f81d-180">Atualizar o conteúdo da página</span><span class="sxs-lookup"><span data-stu-id="9f81d-180">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="9f81d-181">None</span><span class="sxs-lookup"><span data-stu-id="9f81d-181">None</span></span> |<span data-ttu-id="9f81d-182">Atualizar o conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="9f81d-182">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="9f81d-183">Excluir página</span><span class="sxs-lookup"><span data-stu-id="9f81d-183">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="9f81d-184">None</span><span class="sxs-lookup"><span data-stu-id="9f81d-184">None</span></span> |<span data-ttu-id="9f81d-185">Exclua a página.</span><span class="sxs-lookup"><span data-stu-id="9f81d-185">Delete the page.</span></span> |
|[<span data-ttu-id="9f81d-186">copyToSection</span><span class="sxs-lookup"><span data-stu-id="9f81d-186">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="9f81d-187">None</span><span class="sxs-lookup"><span data-stu-id="9f81d-187">None</span></span> |<span data-ttu-id="9f81d-188">Copia a página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="9f81d-188">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->