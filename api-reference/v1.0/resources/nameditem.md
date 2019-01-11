---
title: Tipo de recurso NamedItem
description: Representa um nome definido para um intervalo de células ou um valor. Os nomes podem ser objetos nomeados primitivos (conforme exibido no tipo abaixo), objetos de intervalo ou uma referência a um intervalo. Use esse objeto para obter um objeto de intervalo associado aos nomes.
localization_priority: Normal
ms.openlocfilehash: e413361cc42a0f8f65e23e12d36b49d2c7bcebb3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883822"
---
# <a name="nameditem-resource-type"></a><span data-ttu-id="301ee-105">Tipo de recurso NamedItem</span><span class="sxs-lookup"><span data-stu-id="301ee-105">NamedItem resource type</span></span>

<span data-ttu-id="301ee-p102">Representa um nome definido para um intervalo de células ou um valor. Os nomes podem ser objetos nomeados primitivos (conforme exibido no tipo abaixo), objetos de intervalo ou uma referência a um intervalo. Use esse objeto para obter um objeto de intervalo associado aos nomes.</span><span class="sxs-lookup"><span data-stu-id="301ee-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="301ee-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="301ee-109">Methods</span></span>

| <span data-ttu-id="301ee-110">Método</span><span class="sxs-lookup"><span data-stu-id="301ee-110">Method</span></span>           | <span data-ttu-id="301ee-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="301ee-111">Return Type</span></span>    |<span data-ttu-id="301ee-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="301ee-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="301ee-113">Add</span><span class="sxs-lookup"><span data-stu-id="301ee-113">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="301ee-114">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="301ee-114">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="301ee-115">Adiciona um novo nome à coleção do escopo fornecido.</span><span class="sxs-lookup"><span data-stu-id="301ee-115">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="301ee-116">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="301ee-116">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="301ee-117">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="301ee-117">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="301ee-118">Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.</span><span class="sxs-lookup"><span data-stu-id="301ee-118">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="301ee-119">Get NamedItem</span><span class="sxs-lookup"><span data-stu-id="301ee-119">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="301ee-120">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="301ee-120">WorkbookNamedItem</span></span>](nameditem.md) |<span data-ttu-id="301ee-121">Leia as propriedades e os relacionamentos do objeto namedItem.</span><span class="sxs-lookup"><span data-stu-id="301ee-121">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="301ee-122">Update</span><span class="sxs-lookup"><span data-stu-id="301ee-122">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="301ee-123">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="301ee-123">WorkbookNamedItem</span></span>](nameditem.md)   |<span data-ttu-id="301ee-124">Atualize o objeto NamedItem.</span><span class="sxs-lookup"><span data-stu-id="301ee-124">Update NamedItem object.</span></span> |
|[<span data-ttu-id="301ee-125">Range</span><span class="sxs-lookup"><span data-stu-id="301ee-125">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="301ee-126">Range</span><span class="sxs-lookup"><span data-stu-id="301ee-126">Range</span></span>](range.md)|<span data-ttu-id="301ee-p103">Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.</span><span class="sxs-lookup"><span data-stu-id="301ee-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="301ee-129">List</span><span class="sxs-lookup"><span data-stu-id="301ee-129">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="301ee-130">Coleção [WorkbookNamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="301ee-130">[WorkbookNamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="301ee-131">Obtenha uma coleção de objetos namedItem.</span><span class="sxs-lookup"><span data-stu-id="301ee-131">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="301ee-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="301ee-132">Properties</span></span>
| <span data-ttu-id="301ee-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="301ee-133">Property</span></span>     | <span data-ttu-id="301ee-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="301ee-134">Type</span></span>   |<span data-ttu-id="301ee-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="301ee-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="301ee-136">name</span><span class="sxs-lookup"><span data-stu-id="301ee-136">name</span></span>|<span data-ttu-id="301ee-137">string</span><span class="sxs-lookup"><span data-stu-id="301ee-137">string</span></span>|<span data-ttu-id="301ee-p104">O nome do objeto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="301ee-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="301ee-140">comment</span><span class="sxs-lookup"><span data-stu-id="301ee-140">comment</span></span>|<span data-ttu-id="301ee-141">string</span><span class="sxs-lookup"><span data-stu-id="301ee-141">string</span></span>|<span data-ttu-id="301ee-142">Representa o comentário associado a esse nome.</span><span class="sxs-lookup"><span data-stu-id="301ee-142">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="301ee-143">scope</span><span class="sxs-lookup"><span data-stu-id="301ee-143">scope</span></span>|<span data-ttu-id="301ee-144">string</span><span class="sxs-lookup"><span data-stu-id="301ee-144">string</span></span>|<span data-ttu-id="301ee-p105">Indica se o nome tem escopo para a pasta de trabalho ou uma planilha específica. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="301ee-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="301ee-147">type</span><span class="sxs-lookup"><span data-stu-id="301ee-147">type</span></span>|<span data-ttu-id="301ee-148">string</span><span class="sxs-lookup"><span data-stu-id="301ee-148">string</span></span>|<span data-ttu-id="301ee-149">Indica o tipo de referência é associado ao nome.</span><span class="sxs-lookup"><span data-stu-id="301ee-149">Indicates what type of reference is associated with the name.</span></span> <span data-ttu-id="301ee-150">Os valores possíveis são: `String`, `Integer`, `Double`, `Boolean`, `Range`.</span><span class="sxs-lookup"><span data-stu-id="301ee-150">The possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`.</span></span> <span data-ttu-id="301ee-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="301ee-151">Read-only.</span></span>|
|<span data-ttu-id="301ee-152">valor</span><span class="sxs-lookup"><span data-stu-id="301ee-152">value</span></span>|<span data-ttu-id="301ee-153">Json</span><span class="sxs-lookup"><span data-stu-id="301ee-153">Json</span></span>|<span data-ttu-id="301ee-p107">Representa a fórmula à qual o nome está definido para fazer referência. Por exemplo, =Plan14!$B$2:$H$12, =4,75, etc. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="301ee-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="301ee-157">visible</span><span class="sxs-lookup"><span data-stu-id="301ee-157">visible</span></span>|<span data-ttu-id="301ee-158">booliano</span><span class="sxs-lookup"><span data-stu-id="301ee-158">boolean</span></span>|<span data-ttu-id="301ee-159">Determina se o objeto fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="301ee-159">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="301ee-160">Relações</span><span class="sxs-lookup"><span data-stu-id="301ee-160">Relationships</span></span>
| <span data-ttu-id="301ee-161">Relação</span><span class="sxs-lookup"><span data-stu-id="301ee-161">Relationship</span></span>     | <span data-ttu-id="301ee-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="301ee-162">Type</span></span>   |<span data-ttu-id="301ee-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="301ee-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="301ee-164">planilha</span><span class="sxs-lookup"><span data-stu-id="301ee-164">worksheet</span></span>|[<span data-ttu-id="301ee-165">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="301ee-165">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="301ee-p108">Retorna a planilha em que o item nomeado está no escopo. Disponível somente se o item estiver com escopo de planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="301ee-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="301ee-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="301ee-169">JSON representation</span></span>

<span data-ttu-id="301ee-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="301ee-170">Here is a JSON representation of the resource.</span></span>

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
