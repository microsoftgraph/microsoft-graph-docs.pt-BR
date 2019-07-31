---
title: tipo de recurso workbookNamedItem
description: Representa um nome definido para um intervalo de células ou um valor. Os nomes podem ser objetos nomeados primitivos (conforme exibido no tipo abaixo), objetos de intervalo ou uma referência a um intervalo. Use esse objeto para obter um objeto de intervalo associado aos nomes.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: 90c816bde49cf7062bf2b04deebd8ce6a7e08669
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007113"
---
# <a name="workbooknameditem-resource-type"></a><span data-ttu-id="e9004-105">tipo de recurso workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="e9004-105">workbookNamedItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9004-p102">Representa um nome definido para um intervalo de células ou um valor. Os nomes podem ser objetos nomeados primitivos (conforme exibido no tipo abaixo), objetos de intervalo ou uma referência a um intervalo. Use esse objeto para obter um objeto de intervalo associado aos nomes.</span><span class="sxs-lookup"><span data-stu-id="e9004-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="e9004-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="e9004-109">Methods</span></span>

| <span data-ttu-id="e9004-110">Método</span><span class="sxs-lookup"><span data-stu-id="e9004-110">Method</span></span>           | <span data-ttu-id="e9004-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e9004-111">Return Type</span></span>    |<span data-ttu-id="e9004-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9004-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e9004-113">Add</span><span class="sxs-lookup"><span data-stu-id="e9004-113">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="e9004-114">workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="e9004-114">workbookNamedItem</span></span>](workbooknameditem.md)|<span data-ttu-id="e9004-115">Adiciona um novo nome à coleção do escopo fornecido.</span><span class="sxs-lookup"><span data-stu-id="e9004-115">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="e9004-116">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="e9004-116">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="e9004-117">workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="e9004-117">workbookNamedItem</span></span>](workbooknameditem.md)|<span data-ttu-id="e9004-118">Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.</span><span class="sxs-lookup"><span data-stu-id="e9004-118">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="e9004-119">Get NamedItem</span><span class="sxs-lookup"><span data-stu-id="e9004-119">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="e9004-120">workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="e9004-120">workbookNamedItem</span></span>](workbooknameditem.md) |<span data-ttu-id="e9004-121">Leia as propriedades e os relacionamentos do objeto namedItem.</span><span class="sxs-lookup"><span data-stu-id="e9004-121">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="e9004-122">Update</span><span class="sxs-lookup"><span data-stu-id="e9004-122">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="e9004-123">workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="e9004-123">workbookNamedItem</span></span>](workbooknameditem.md)   |<span data-ttu-id="e9004-124">Atualize o objeto NamedItem.</span><span class="sxs-lookup"><span data-stu-id="e9004-124">Update NamedItem object.</span></span> |
|[<span data-ttu-id="e9004-125">Range</span><span class="sxs-lookup"><span data-stu-id="e9004-125">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="e9004-126">workbookRange</span><span class="sxs-lookup"><span data-stu-id="e9004-126">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="e9004-p103">Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.</span><span class="sxs-lookup"><span data-stu-id="e9004-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="e9004-129">List</span><span class="sxs-lookup"><span data-stu-id="e9004-129">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="e9004-130">coleção [workbookNamedItem](workbooknameditem.md)</span><span class="sxs-lookup"><span data-stu-id="e9004-130">[workbookNamedItem](workbooknameditem.md) collection</span></span> |<span data-ttu-id="e9004-131">Obtenha uma coleção de objetos namedItem.</span><span class="sxs-lookup"><span data-stu-id="e9004-131">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="e9004-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e9004-132">Properties</span></span>
| <span data-ttu-id="e9004-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9004-133">Property</span></span>     | <span data-ttu-id="e9004-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9004-134">Type</span></span>   |<span data-ttu-id="e9004-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9004-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9004-136">name</span><span class="sxs-lookup"><span data-stu-id="e9004-136">name</span></span>|<span data-ttu-id="e9004-137">string</span><span class="sxs-lookup"><span data-stu-id="e9004-137">string</span></span>|<span data-ttu-id="e9004-p104">O nome do objeto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e9004-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="e9004-140">comment</span><span class="sxs-lookup"><span data-stu-id="e9004-140">comment</span></span>|<span data-ttu-id="e9004-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9004-141">string</span></span>|<span data-ttu-id="e9004-142">Representa o comentário associado a esse nome.</span><span class="sxs-lookup"><span data-stu-id="e9004-142">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="e9004-143">scope</span><span class="sxs-lookup"><span data-stu-id="e9004-143">scope</span></span>|<span data-ttu-id="e9004-144">string</span><span class="sxs-lookup"><span data-stu-id="e9004-144">string</span></span>|<span data-ttu-id="e9004-p105">Indica se o nome tem escopo para a pasta de trabalho ou uma planilha específica. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e9004-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="e9004-147">type</span><span class="sxs-lookup"><span data-stu-id="e9004-147">type</span></span>|<span data-ttu-id="e9004-148">string</span><span class="sxs-lookup"><span data-stu-id="e9004-148">string</span></span>|<span data-ttu-id="e9004-p106">Indica o tipo de referência associado ao nome. Os valores possíveis são: `String`, `Integer`, `Double`, `Boolean` e `Range`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e9004-p106">Indicates what type of reference is associated with the name. Possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`. Read-only.</span></span>|
|<span data-ttu-id="e9004-152">value</span><span class="sxs-lookup"><span data-stu-id="e9004-152">value</span></span>|<span data-ttu-id="e9004-153">string</span><span class="sxs-lookup"><span data-stu-id="e9004-153">string</span></span>|<span data-ttu-id="e9004-p107">Representa a fórmula à qual o nome está definido para fazer referência. Por exemplo, =Plan14!$B$2:$H$12, =4,75, etc. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e9004-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="e9004-157">visible</span><span class="sxs-lookup"><span data-stu-id="e9004-157">visible</span></span>|<span data-ttu-id="e9004-158">booliano</span><span class="sxs-lookup"><span data-stu-id="e9004-158">boolean</span></span>|<span data-ttu-id="e9004-159">Determina se o objeto fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="e9004-159">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9004-160">Relações</span><span class="sxs-lookup"><span data-stu-id="e9004-160">Relationships</span></span>
| <span data-ttu-id="e9004-161">Relação</span><span class="sxs-lookup"><span data-stu-id="e9004-161">Relationship</span></span>     | <span data-ttu-id="e9004-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9004-162">Type</span></span>   |<span data-ttu-id="e9004-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9004-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9004-164">planilha</span><span class="sxs-lookup"><span data-stu-id="e9004-164">worksheet</span></span>|[<span data-ttu-id="e9004-165">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="e9004-165">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="e9004-p108">Retorna a planilha em que o item nomeado está no escopo. Disponível somente se o item estiver com escopo de planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e9004-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9004-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e9004-169">JSON representation</span></span>

<span data-ttu-id="e9004-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e9004-170">Here is a JSON representation of the resource.</span></span>

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
