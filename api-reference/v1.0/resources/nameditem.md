---
title: Tipo de recurso NamedItem
description: Representa um nome definido para um intervalo de células ou um valor. Os nomes podem ser objetos nomeados primitivos (conforme exibido no tipo abaixo), objetos de intervalo ou uma referência a um intervalo. Use esse objeto para obter um objeto de intervalo associado aos nomes.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3be31cd34f1fe880c079bba50e7e612dfa26da45
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808211"
---
# <a name="nameditem-resource-type"></a><span data-ttu-id="8dc37-105">Tipo de recurso NamedItem</span><span class="sxs-lookup"><span data-stu-id="8dc37-105">NamedItem resource type</span></span>

<span data-ttu-id="8dc37-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dc37-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8dc37-p102">Representa um nome definido para um intervalo de células ou um valor. Os nomes podem ser objetos nomeados primitivos (conforme exibido no tipo abaixo), objetos de intervalo ou uma referência a um intervalo. Use esse objeto para obter um objeto de intervalo associado aos nomes.</span><span class="sxs-lookup"><span data-stu-id="8dc37-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="8dc37-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="8dc37-110">Methods</span></span>

| <span data-ttu-id="8dc37-111">Método</span><span class="sxs-lookup"><span data-stu-id="8dc37-111">Method</span></span>           | <span data-ttu-id="8dc37-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8dc37-112">Return Type</span></span>    |<span data-ttu-id="8dc37-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dc37-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8dc37-114">Add</span><span class="sxs-lookup"><span data-stu-id="8dc37-114">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="8dc37-115">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="8dc37-115">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="8dc37-116">Adiciona um novo nome à coleção do escopo fornecido.</span><span class="sxs-lookup"><span data-stu-id="8dc37-116">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="8dc37-117">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="8dc37-117">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="8dc37-118">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="8dc37-118">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="8dc37-119">Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.</span><span class="sxs-lookup"><span data-stu-id="8dc37-119">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="8dc37-120">Get NamedItem</span><span class="sxs-lookup"><span data-stu-id="8dc37-120">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="8dc37-121">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="8dc37-121">WorkbookNamedItem</span></span>](nameditem.md) |<span data-ttu-id="8dc37-122">Leia as propriedades e os relacionamentos do objeto namedItem.</span><span class="sxs-lookup"><span data-stu-id="8dc37-122">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="8dc37-123">Update</span><span class="sxs-lookup"><span data-stu-id="8dc37-123">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="8dc37-124">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="8dc37-124">WorkbookNamedItem</span></span>](nameditem.md)   |<span data-ttu-id="8dc37-125">Atualize o objeto NamedItem.</span><span class="sxs-lookup"><span data-stu-id="8dc37-125">Update NamedItem object.</span></span> |
|[<span data-ttu-id="8dc37-126">Range</span><span class="sxs-lookup"><span data-stu-id="8dc37-126">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="8dc37-127">Range</span><span class="sxs-lookup"><span data-stu-id="8dc37-127">Range</span></span>](range.md)|<span data-ttu-id="8dc37-p103">Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.</span><span class="sxs-lookup"><span data-stu-id="8dc37-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="8dc37-130">List</span><span class="sxs-lookup"><span data-stu-id="8dc37-130">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="8dc37-131">Coleção [WorkbookNamedItem](nameditem.md) </span><span class="sxs-lookup"><span data-stu-id="8dc37-131">[WorkbookNamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="8dc37-132">Obtenha uma coleção de objetos namedItem.</span><span class="sxs-lookup"><span data-stu-id="8dc37-132">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="8dc37-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8dc37-133">Properties</span></span>
| <span data-ttu-id="8dc37-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8dc37-134">Property</span></span>     | <span data-ttu-id="8dc37-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="8dc37-135">Type</span></span>   |<span data-ttu-id="8dc37-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dc37-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8dc37-137">nome</span><span class="sxs-lookup"><span data-stu-id="8dc37-137">name</span></span>|<span data-ttu-id="8dc37-138">string</span><span class="sxs-lookup"><span data-stu-id="8dc37-138">string</span></span>|<span data-ttu-id="8dc37-p104">O nome do objeto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8dc37-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="8dc37-141">comment</span><span class="sxs-lookup"><span data-stu-id="8dc37-141">comment</span></span>|<span data-ttu-id="8dc37-142">string</span><span class="sxs-lookup"><span data-stu-id="8dc37-142">string</span></span>|<span data-ttu-id="8dc37-143">Representa o comentário associado a esse nome.</span><span class="sxs-lookup"><span data-stu-id="8dc37-143">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="8dc37-144">scope</span><span class="sxs-lookup"><span data-stu-id="8dc37-144">scope</span></span>|<span data-ttu-id="8dc37-145">string</span><span class="sxs-lookup"><span data-stu-id="8dc37-145">string</span></span>|<span data-ttu-id="8dc37-p105">Indica se o nome tem escopo para a pasta de trabalho ou uma planilha específica. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8dc37-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="8dc37-148">type</span><span class="sxs-lookup"><span data-stu-id="8dc37-148">type</span></span>|<span data-ttu-id="8dc37-149">string</span><span class="sxs-lookup"><span data-stu-id="8dc37-149">string</span></span>|<span data-ttu-id="8dc37-150">Indica o tipo de referência que está associado ao nome.</span><span class="sxs-lookup"><span data-stu-id="8dc37-150">Indicates what type of reference is associated with the name.</span></span> <span data-ttu-id="8dc37-151">Os valores possíveis são: `String`, `Integer`, `Double`, `Boolean`, `Range`.</span><span class="sxs-lookup"><span data-stu-id="8dc37-151">The possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`.</span></span> <span data-ttu-id="8dc37-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8dc37-152">Read-only.</span></span>|
|<span data-ttu-id="8dc37-153">value</span><span class="sxs-lookup"><span data-stu-id="8dc37-153">value</span></span>|<span data-ttu-id="8dc37-154">Json</span><span class="sxs-lookup"><span data-stu-id="8dc37-154">Json</span></span>|<span data-ttu-id="8dc37-p107">Representa a fórmula à qual o nome está definido para fazer referência. Por exemplo, =Plan14!$B$2:$H$12, =4,75, etc. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8dc37-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="8dc37-158">visible</span><span class="sxs-lookup"><span data-stu-id="8dc37-158">visible</span></span>|<span data-ttu-id="8dc37-159">booliano</span><span class="sxs-lookup"><span data-stu-id="8dc37-159">boolean</span></span>|<span data-ttu-id="8dc37-160">Determina se o objeto fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="8dc37-160">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8dc37-161">Relações</span><span class="sxs-lookup"><span data-stu-id="8dc37-161">Relationships</span></span>
| <span data-ttu-id="8dc37-162">Relação</span><span class="sxs-lookup"><span data-stu-id="8dc37-162">Relationship</span></span>     | <span data-ttu-id="8dc37-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="8dc37-163">Type</span></span>   |<span data-ttu-id="8dc37-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dc37-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8dc37-165">planilha</span><span class="sxs-lookup"><span data-stu-id="8dc37-165">worksheet</span></span>|[<span data-ttu-id="8dc37-166">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="8dc37-166">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="8dc37-p108">Retorna a planilha em que o item nomeado está no escopo. Disponível somente se o item estiver com escopo de planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8dc37-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8dc37-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8dc37-170">JSON representation</span></span>

<span data-ttu-id="8dc37-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8dc37-171">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookNamedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.Json"},
  "visible": true

}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
