---
title: tipo de recurso workbookNamedItem
description: Representa um nome definido para um intervalo de células ou um valor. Os nomes podem ser objetos nomeados primitivos (conforme exibido no tipo abaixo), objetos de intervalo ou uma referência a um intervalo. Use esse objeto para obter um objeto de intervalo associado aos nomes.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: 17b9e7a04a2524febcb949829b626bc6efe6b779
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519208"
---
# <a name="workbooknameditem-resource-type"></a><span data-ttu-id="bff4c-105">tipo de recurso workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="bff4c-105">workbookNamedItem resource type</span></span>

<span data-ttu-id="bff4c-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bff4c-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bff4c-p102">Representa um nome definido para um intervalo de células ou um valor. Os nomes podem ser objetos nomeados primitivos (conforme exibido no tipo abaixo), objetos de intervalo ou uma referência a um intervalo. Use esse objeto para obter um objeto de intervalo associado aos nomes.</span><span class="sxs-lookup"><span data-stu-id="bff4c-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="bff4c-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="bff4c-110">Methods</span></span>

| <span data-ttu-id="bff4c-111">Método</span><span class="sxs-lookup"><span data-stu-id="bff4c-111">Method</span></span>           | <span data-ttu-id="bff4c-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bff4c-112">Return Type</span></span>    |<span data-ttu-id="bff4c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="bff4c-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bff4c-114">Add</span><span class="sxs-lookup"><span data-stu-id="bff4c-114">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="bff4c-115">workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="bff4c-115">workbookNamedItem</span></span>](workbooknameditem.md)|<span data-ttu-id="bff4c-116">Adiciona um novo nome à coleção do escopo fornecido.</span><span class="sxs-lookup"><span data-stu-id="bff4c-116">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="bff4c-117">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="bff4c-117">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="bff4c-118">workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="bff4c-118">workbookNamedItem</span></span>](workbooknameditem.md)|<span data-ttu-id="bff4c-119">Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.</span><span class="sxs-lookup"><span data-stu-id="bff4c-119">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="bff4c-120">Get NamedItem</span><span class="sxs-lookup"><span data-stu-id="bff4c-120">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="bff4c-121">workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="bff4c-121">workbookNamedItem</span></span>](workbooknameditem.md) |<span data-ttu-id="bff4c-122">Leia as propriedades e os relacionamentos do objeto namedItem.</span><span class="sxs-lookup"><span data-stu-id="bff4c-122">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="bff4c-123">Update</span><span class="sxs-lookup"><span data-stu-id="bff4c-123">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="bff4c-124">workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="bff4c-124">workbookNamedItem</span></span>](workbooknameditem.md)   |<span data-ttu-id="bff4c-125">Atualize o objeto NamedItem.</span><span class="sxs-lookup"><span data-stu-id="bff4c-125">Update NamedItem object.</span></span> |
|[<span data-ttu-id="bff4c-126">Range</span><span class="sxs-lookup"><span data-stu-id="bff4c-126">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="bff4c-127">workbookRange</span><span class="sxs-lookup"><span data-stu-id="bff4c-127">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="bff4c-p103">Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.</span><span class="sxs-lookup"><span data-stu-id="bff4c-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="bff4c-130">List</span><span class="sxs-lookup"><span data-stu-id="bff4c-130">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="bff4c-131">coleção [workbookNamedItem](workbooknameditem.md)</span><span class="sxs-lookup"><span data-stu-id="bff4c-131">[workbookNamedItem](workbooknameditem.md) collection</span></span> |<span data-ttu-id="bff4c-132">Obtenha uma coleção de objetos namedItem.</span><span class="sxs-lookup"><span data-stu-id="bff4c-132">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="bff4c-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bff4c-133">Properties</span></span>
| <span data-ttu-id="bff4c-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bff4c-134">Property</span></span>     | <span data-ttu-id="bff4c-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="bff4c-135">Type</span></span>   |<span data-ttu-id="bff4c-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="bff4c-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bff4c-137">nome</span><span class="sxs-lookup"><span data-stu-id="bff4c-137">name</span></span>|<span data-ttu-id="bff4c-138">string</span><span class="sxs-lookup"><span data-stu-id="bff4c-138">string</span></span>|<span data-ttu-id="bff4c-p104">O nome do objeto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bff4c-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="bff4c-141">comment</span><span class="sxs-lookup"><span data-stu-id="bff4c-141">comment</span></span>|<span data-ttu-id="bff4c-142">string</span><span class="sxs-lookup"><span data-stu-id="bff4c-142">string</span></span>|<span data-ttu-id="bff4c-143">Representa o comentário associado a esse nome.</span><span class="sxs-lookup"><span data-stu-id="bff4c-143">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="bff4c-144">scope</span><span class="sxs-lookup"><span data-stu-id="bff4c-144">scope</span></span>|<span data-ttu-id="bff4c-145">string</span><span class="sxs-lookup"><span data-stu-id="bff4c-145">string</span></span>|<span data-ttu-id="bff4c-p105">Indica se o nome tem escopo para a pasta de trabalho ou uma planilha específica. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bff4c-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="bff4c-148">type</span><span class="sxs-lookup"><span data-stu-id="bff4c-148">type</span></span>|<span data-ttu-id="bff4c-149">string</span><span class="sxs-lookup"><span data-stu-id="bff4c-149">string</span></span>|<span data-ttu-id="bff4c-p106">Indica o tipo de referência associado ao nome. Os valores possíveis são: `String`, `Integer`, `Double`, `Boolean` e `Range`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bff4c-p106">Indicates what type of reference is associated with the name. Possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`. Read-only.</span></span>|
|<span data-ttu-id="bff4c-153">value</span><span class="sxs-lookup"><span data-stu-id="bff4c-153">value</span></span>|<span data-ttu-id="bff4c-154">string</span><span class="sxs-lookup"><span data-stu-id="bff4c-154">string</span></span>|<span data-ttu-id="bff4c-p107">Representa a fórmula à qual o nome está definido para fazer referência. Por exemplo, =Plan14!$B$2:$H$12, =4,75, etc. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bff4c-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="bff4c-158">visible</span><span class="sxs-lookup"><span data-stu-id="bff4c-158">visible</span></span>|<span data-ttu-id="bff4c-159">booliano</span><span class="sxs-lookup"><span data-stu-id="bff4c-159">boolean</span></span>|<span data-ttu-id="bff4c-160">Determina se o objeto fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="bff4c-160">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bff4c-161">Relações</span><span class="sxs-lookup"><span data-stu-id="bff4c-161">Relationships</span></span>
| <span data-ttu-id="bff4c-162">Relação</span><span class="sxs-lookup"><span data-stu-id="bff4c-162">Relationship</span></span>     | <span data-ttu-id="bff4c-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="bff4c-163">Type</span></span>   |<span data-ttu-id="bff4c-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="bff4c-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bff4c-165">planilha</span><span class="sxs-lookup"><span data-stu-id="bff4c-165">worksheet</span></span>|[<span data-ttu-id="bff4c-166">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="bff4c-166">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="bff4c-p108">Retorna a planilha em que o item nomeado está no escopo. Disponível somente se o item estiver com escopo de planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bff4c-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bff4c-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bff4c-170">JSON representation</span></span>

<span data-ttu-id="bff4c-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bff4c-171">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookNamedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": "string",
  "visible": true
  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
