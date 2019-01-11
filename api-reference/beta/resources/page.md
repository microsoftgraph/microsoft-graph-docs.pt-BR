---
title: Tipo de recurso page
description: Uma página em um bloco de anotações do OneNote.
localization_priority: Normal
ms.openlocfilehash: 5928f430fcbfe9f41c6aa83e99d7dfe737e8e1c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850131"
---
# <a name="page-resource-type"></a><span data-ttu-id="5b69f-103">Tipo de recurso page</span><span class="sxs-lookup"><span data-stu-id="5b69f-103">page resource type</span></span>

> <span data-ttu-id="5b69f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5b69f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b69f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5b69f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b69f-106">Uma página em um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="5b69f-106">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b69f-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b69f-107">JSON representation</span></span>

<span data-ttu-id="5b69f-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b69f-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="5b69f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b69f-109">Properties</span></span>
| <span data-ttu-id="5b69f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b69f-110">Property</span></span>     | <span data-ttu-id="5b69f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b69f-111">Type</span></span>   |<span data-ttu-id="5b69f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b69f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b69f-113">content</span><span class="sxs-lookup"><span data-stu-id="5b69f-113">content</span></span>|<span data-ttu-id="5b69f-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="5b69f-114">Stream</span></span>|<span data-ttu-id="5b69f-115">O conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="5b69f-115">The page's HTML content.</span></span>|
|<span data-ttu-id="5b69f-116">contentUrl</span><span class="sxs-lookup"><span data-stu-id="5b69f-116">contentUrl</span></span>|<span data-ttu-id="5b69f-117">String</span><span class="sxs-lookup"><span data-stu-id="5b69f-117">String</span></span>|<span data-ttu-id="5b69f-p102">A URL do conteúdo HTML da página.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b69f-p102">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="5b69f-120">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="5b69f-120">createdByAppId</span></span>|<span data-ttu-id="5b69f-121">String</span><span class="sxs-lookup"><span data-stu-id="5b69f-121">String</span></span>|<span data-ttu-id="5b69f-p103">O identificador exclusivo do aplicativo que criou a página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b69f-p103">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="5b69f-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b69f-124">createdDateTime</span></span>|<span data-ttu-id="5b69f-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b69f-125">DateTimeOffset</span></span>|<span data-ttu-id="5b69f-p104">A data e a hora da criação da página. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b69f-p104">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="5b69f-130">id</span><span class="sxs-lookup"><span data-stu-id="5b69f-130">id</span></span>|<span data-ttu-id="5b69f-131">String</span><span class="sxs-lookup"><span data-stu-id="5b69f-131">String</span></span>|<span data-ttu-id="5b69f-p105">O identificador exclusivo da página.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b69f-p105">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="5b69f-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b69f-134">lastModifiedDateTime</span></span>|<span data-ttu-id="5b69f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b69f-135">DateTimeOffset</span></span>|<span data-ttu-id="5b69f-p106">A data e a hora da última modificação da página. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b69f-p106">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="5b69f-140">nível</span><span class="sxs-lookup"><span data-stu-id="5b69f-140">level</span></span>|<span data-ttu-id="5b69f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="5b69f-141">Int32</span></span>|<span data-ttu-id="5b69f-p107">O nível de recuo da página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b69f-p107">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="5b69f-144">links</span><span class="sxs-lookup"><span data-stu-id="5b69f-144">links</span></span>|[<span data-ttu-id="5b69f-145">PageLinks</span><span class="sxs-lookup"><span data-stu-id="5b69f-145">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="5b69f-p108">Links para abrir a página. O link `oneNoteClientURL` abre a página no cliente nativo do OneNote se ele estiver instalado. O link `oneNoteWebUrl` abre a página no OneNote Online. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b69f-p108">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="5b69f-150">ordem</span><span class="sxs-lookup"><span data-stu-id="5b69f-150">order</span></span>|<span data-ttu-id="5b69f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="5b69f-151">Int32</span></span>|<span data-ttu-id="5b69f-p109">A ordem da página dentro da seção pai dela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b69f-p109">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="5b69f-154">self</span><span class="sxs-lookup"><span data-stu-id="5b69f-154">self</span></span>|<span data-ttu-id="5b69f-155">String</span><span class="sxs-lookup"><span data-stu-id="5b69f-155">String</span></span>|<span data-ttu-id="5b69f-p110">O ponto de extremidade onde você pode obter detalhes sobre a página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b69f-p110">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="5b69f-158">title</span><span class="sxs-lookup"><span data-stu-id="5b69f-158">title</span></span>|<span data-ttu-id="5b69f-159">String</span><span class="sxs-lookup"><span data-stu-id="5b69f-159">String</span></span>|<span data-ttu-id="5b69f-160">O título da página.</span><span class="sxs-lookup"><span data-stu-id="5b69f-160">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5b69f-161">Relações</span><span class="sxs-lookup"><span data-stu-id="5b69f-161">Relationships</span></span>
| <span data-ttu-id="5b69f-162">Relação</span><span class="sxs-lookup"><span data-stu-id="5b69f-162">Relationship</span></span> | <span data-ttu-id="5b69f-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b69f-163">Type</span></span>   |<span data-ttu-id="5b69f-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b69f-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b69f-165">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="5b69f-165">parentNotebook</span></span>|[<span data-ttu-id="5b69f-166">Notebook</span><span class="sxs-lookup"><span data-stu-id="5b69f-166">Notebook</span></span>](notebook.md)|<span data-ttu-id="5b69f-p111">O bloco de anotações que contém a página.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b69f-p111">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="5b69f-169">parentSection</span><span class="sxs-lookup"><span data-stu-id="5b69f-169">parentSection</span></span>|[<span data-ttu-id="5b69f-170">Section</span><span class="sxs-lookup"><span data-stu-id="5b69f-170">Section</span></span>](section.md)|<span data-ttu-id="5b69f-p112">A seção que contém a página. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b69f-p112">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="5b69f-173">Métodos</span><span class="sxs-lookup"><span data-stu-id="5b69f-173">Methods</span></span>

| <span data-ttu-id="5b69f-174">Método</span><span class="sxs-lookup"><span data-stu-id="5b69f-174">Method</span></span>           | <span data-ttu-id="5b69f-175">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5b69f-175">Return Type</span></span>    |<span data-ttu-id="5b69f-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b69f-176">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5b69f-177">Get page</span><span class="sxs-lookup"><span data-stu-id="5b69f-177">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="5b69f-178">Página</span><span class="sxs-lookup"><span data-stu-id="5b69f-178">Page</span></span>](page.md) |<span data-ttu-id="5b69f-179">Leia as propriedades e as relações da página.</span><span class="sxs-lookup"><span data-stu-id="5b69f-179">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="5b69f-180">Atualizar o conteúdo da página</span><span class="sxs-lookup"><span data-stu-id="5b69f-180">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="5b69f-181">None</span><span class="sxs-lookup"><span data-stu-id="5b69f-181">None</span></span> |<span data-ttu-id="5b69f-182">Atualizar o conteúdo HTML da página.</span><span class="sxs-lookup"><span data-stu-id="5b69f-182">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="5b69f-183">Excluir página</span><span class="sxs-lookup"><span data-stu-id="5b69f-183">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="5b69f-184">None</span><span class="sxs-lookup"><span data-stu-id="5b69f-184">None</span></span> |<span data-ttu-id="5b69f-185">Exclua a página.</span><span class="sxs-lookup"><span data-stu-id="5b69f-185">Delete the page.</span></span> |
|[<span data-ttu-id="5b69f-186">copyToSection</span><span class="sxs-lookup"><span data-stu-id="5b69f-186">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="5b69f-187">None</span><span class="sxs-lookup"><span data-stu-id="5b69f-187">None</span></span> |<span data-ttu-id="5b69f-188">Copia a página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="5b69f-188">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
