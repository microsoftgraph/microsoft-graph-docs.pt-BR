---
title: Tipo de recurso outlookCategory
description: Representa uma categoria pela qual um usuário pode agrupar itens do Outlook como mensagens e eventos. No Outlook, o usuário define categorias em uma lista mestra e pode aplicar uma ou mais dessas definições pelo usuário
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 516a4c42a93577b822f3b28ec1f0e886319905df
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130000"
---
# <a name="outlookcategory-resource-type"></a><span data-ttu-id="c9542-104">Tipo de recurso outlookCategory</span><span class="sxs-lookup"><span data-stu-id="c9542-104">outlookCategory resource type</span></span>

<span data-ttu-id="c9542-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9542-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="c9542-106">Representa uma categoria pela qual um usuário pode agrupar itens do Outlook como mensagens e eventos.</span><span class="sxs-lookup"><span data-stu-id="c9542-106">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="c9542-107">No Outlook, o usuário define categorias em uma lista mestra e pode aplicar uma ou mais dessas categorias definidas pelo usuário a um item.</span><span class="sxs-lookup"><span data-stu-id="c9542-107">In Outlook, the user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="c9542-108">Usando a API REST, é possível [criar](../api/outlookuser-post-mastercategories.md) e definir categorias na lista mestra de categorias para um usuário.</span><span class="sxs-lookup"><span data-stu-id="c9542-108">Using the REST API, you can [create](../api/outlookuser-post-mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="c9542-109">Também é possível [acessar essa lista mestra de categorias](../api/outlookuser-list-mastercategories.md), [obter uma categoria específica](../api/outlookcategory-get.md), [atualizar](../api/outlookcategory-update.md) a cor associada a uma categoria ou [excluir](../api/outlookcategory-delete.md) uma categoria.</span><span class="sxs-lookup"><span data-stu-id="c9542-109">You can also [get this master list of categories](../api/outlookuser-list-mastercategories.md), [get a specific category](../api/outlookcategory-get.md), [update](../api/outlookcategory-update.md) the color associated with a category, or [delete](../api/outlookcategory-delete.md) a category.</span></span> <span data-ttu-id="c9542-110">É possível aplicar uma categoria a um item atribuindo a propriedade **displayName** da categoria à coleção **categories** do item.</span><span class="sxs-lookup"><span data-stu-id="c9542-110">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="c9542-111">Recursos que podem ser atribuídos categorias incluem [contato](contact.md), [evento](event.md), [mensagem](message.md), [outlookTask](outlooktask.md)e [postagem](post.md).</span><span class="sxs-lookup"><span data-stu-id="c9542-111">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), [outlookTask](outlooktask.md), and [post](post.md).</span></span>   

<span data-ttu-id="c9542-112">Cada categoria é atribuída por duas propriedades: **displayName** e **color**.</span><span class="sxs-lookup"><span data-stu-id="c9542-112">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="c9542-113">O valor **displayName** deve ser exclusivo na lista mestra de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c9542-113">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="c9542-114">No entanto, o valor **color** não precisa ser exclusivo. Várias categorias na lista mestra podem ser mapeadas para a mesma cor.</span><span class="sxs-lookup"><span data-stu-id="c9542-114">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="c9542-115">É possível mapear até 25 cores diferentes para as categorias na lista mestra a um usuário.</span><span class="sxs-lookup"><span data-stu-id="c9542-115">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="c9542-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9542-116">Properties</span></span>
| <span data-ttu-id="c9542-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9542-117">Property</span></span>     | <span data-ttu-id="c9542-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9542-118">Type</span></span>   |<span data-ttu-id="c9542-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9542-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9542-120">displayName</span><span class="sxs-lookup"><span data-stu-id="c9542-120">displayName</span></span>|<span data-ttu-id="c9542-121">String</span><span class="sxs-lookup"><span data-stu-id="c9542-121">String</span></span>|<span data-ttu-id="c9542-122">Um nome exclusivo que identifica uma categoria na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="c9542-122">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="c9542-123">Após a criação de uma categoria, o nome não poderá ser alterado.</span><span class="sxs-lookup"><span data-stu-id="c9542-123">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="c9542-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9542-124">Read-only.</span></span>|
|<span data-ttu-id="c9542-125">color</span><span class="sxs-lookup"><span data-stu-id="c9542-125">color</span></span>|<span data-ttu-id="c9542-126">String</span><span class="sxs-lookup"><span data-stu-id="c9542-126">String</span></span>|<span data-ttu-id="c9542-127">Uma constante de cor predefinida que caracteriza uma categoria e que é mapeada para uma das 25 cores predefinidas.</span><span class="sxs-lookup"><span data-stu-id="c9542-127">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="c9542-128">Confira a observação abaixo.</span><span class="sxs-lookup"><span data-stu-id="c9542-128">See the note below.</span></span> |

> <span data-ttu-id="c9542-129">**Observação** Os valores possíveis para **color** são constantes predefinidas como `None`, `preset0` e `preset1`.</span><span class="sxs-lookup"><span data-stu-id="c9542-129">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="c9542-130">Cada constante predefinida é mapeada para uma cor. A cor real depende do cliente do Outlook em que as categorias estão sendo exibidas.</span><span class="sxs-lookup"><span data-stu-id="c9542-130">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="c9542-131">A tabela a seguir mostra as cores mapeadas para cada constante predefinida do Outlook (cliente da área de trabalho).</span><span class="sxs-lookup"><span data-stu-id="c9542-131">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 


| <span data-ttu-id="c9542-132">Constante predefinida</span><span class="sxs-lookup"><span data-stu-id="c9542-132">Pre-set constant</span></span>  | <span data-ttu-id="c9542-133">Cor mapeada para no Outlook</span><span class="sxs-lookup"><span data-stu-id="c9542-133">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c9542-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c9542-134">None</span></span> | <span data-ttu-id="c9542-135">Nenhuma cor mapeada</span><span class="sxs-lookup"><span data-stu-id="c9542-135">No color mapped</span></span> |
| <span data-ttu-id="c9542-136">Preset0</span><span class="sxs-lookup"><span data-stu-id="c9542-136">Preset0</span></span> | <span data-ttu-id="c9542-137">Vermelho</span><span class="sxs-lookup"><span data-stu-id="c9542-137">Red</span></span> |
| <span data-ttu-id="c9542-138">Preset1</span><span class="sxs-lookup"><span data-stu-id="c9542-138">Preset1</span></span> | <span data-ttu-id="c9542-139">Laranja</span><span class="sxs-lookup"><span data-stu-id="c9542-139">Orange</span></span> |
| <span data-ttu-id="c9542-140">Preset2</span><span class="sxs-lookup"><span data-stu-id="c9542-140">Preset2</span></span> | <span data-ttu-id="c9542-141">Marrom</span><span class="sxs-lookup"><span data-stu-id="c9542-141">Brown</span></span> |
| <span data-ttu-id="c9542-142">Preset3</span><span class="sxs-lookup"><span data-stu-id="c9542-142">Preset3</span></span> | <span data-ttu-id="c9542-143">Amarelo</span><span class="sxs-lookup"><span data-stu-id="c9542-143">Yellow</span></span> |
| <span data-ttu-id="c9542-144">Preset4</span><span class="sxs-lookup"><span data-stu-id="c9542-144">Preset4</span></span> | <span data-ttu-id="c9542-145">Verde</span><span class="sxs-lookup"><span data-stu-id="c9542-145">Green</span></span> |
| <span data-ttu-id="c9542-146">Preset5</span><span class="sxs-lookup"><span data-stu-id="c9542-146">Preset5</span></span> | <span data-ttu-id="c9542-147">Azul-petróleo</span><span class="sxs-lookup"><span data-stu-id="c9542-147">Teal</span></span> |
| <span data-ttu-id="c9542-148">Preset6</span><span class="sxs-lookup"><span data-stu-id="c9542-148">Preset6</span></span> | <span data-ttu-id="c9542-149">Verde-oliva</span><span class="sxs-lookup"><span data-stu-id="c9542-149">Olive</span></span> |
| <span data-ttu-id="c9542-150">Preset7</span><span class="sxs-lookup"><span data-stu-id="c9542-150">Preset7</span></span> | <span data-ttu-id="c9542-151">Azul</span><span class="sxs-lookup"><span data-stu-id="c9542-151">Blue</span></span> |
| <span data-ttu-id="c9542-152">Preset8</span><span class="sxs-lookup"><span data-stu-id="c9542-152">Preset8</span></span> | <span data-ttu-id="c9542-153">Roxo</span><span class="sxs-lookup"><span data-stu-id="c9542-153">Purple</span></span> |
| <span data-ttu-id="c9542-154">Preset9</span><span class="sxs-lookup"><span data-stu-id="c9542-154">Preset9</span></span> | <span data-ttu-id="c9542-155">Cranberry</span><span class="sxs-lookup"><span data-stu-id="c9542-155">Cranberry</span></span> |
| <span data-ttu-id="c9542-156">Preset10</span><span class="sxs-lookup"><span data-stu-id="c9542-156">Preset10</span></span> | <span data-ttu-id="c9542-157">Steel</span><span class="sxs-lookup"><span data-stu-id="c9542-157">Steel</span></span> |
| <span data-ttu-id="c9542-158">Preset11</span><span class="sxs-lookup"><span data-stu-id="c9542-158">Preset11</span></span> | <span data-ttu-id="c9542-159">DarkSteel</span><span class="sxs-lookup"><span data-stu-id="c9542-159">DarkSteel</span></span> |
| <span data-ttu-id="c9542-160">Preset12</span><span class="sxs-lookup"><span data-stu-id="c9542-160">Preset12</span></span> | <span data-ttu-id="c9542-161">Cinza</span><span class="sxs-lookup"><span data-stu-id="c9542-161">Gray</span></span> |
| <span data-ttu-id="c9542-162">Preset13</span><span class="sxs-lookup"><span data-stu-id="c9542-162">Preset13</span></span> | <span data-ttu-id="c9542-163">DarkGray</span><span class="sxs-lookup"><span data-stu-id="c9542-163">DarkGray</span></span> |
| <span data-ttu-id="c9542-164">Preset14</span><span class="sxs-lookup"><span data-stu-id="c9542-164">Preset14</span></span> | <span data-ttu-id="c9542-165">Preto</span><span class="sxs-lookup"><span data-stu-id="c9542-165">Black</span></span> |
| <span data-ttu-id="c9542-166">Preset15</span><span class="sxs-lookup"><span data-stu-id="c9542-166">Preset15</span></span> | <span data-ttu-id="c9542-167">DarkRed</span><span class="sxs-lookup"><span data-stu-id="c9542-167">DarkRed</span></span> |
| <span data-ttu-id="c9542-168">Preset16</span><span class="sxs-lookup"><span data-stu-id="c9542-168">Preset16</span></span> | <span data-ttu-id="c9542-169">DarkOrange</span><span class="sxs-lookup"><span data-stu-id="c9542-169">DarkOrange</span></span> |
| <span data-ttu-id="c9542-170">Preset17</span><span class="sxs-lookup"><span data-stu-id="c9542-170">Preset17</span></span> | <span data-ttu-id="c9542-171">DarkBrown</span><span class="sxs-lookup"><span data-stu-id="c9542-171">DarkBrown</span></span> |
| <span data-ttu-id="c9542-172">Preset18</span><span class="sxs-lookup"><span data-stu-id="c9542-172">Preset18</span></span> | <span data-ttu-id="c9542-173">DarkYellow</span><span class="sxs-lookup"><span data-stu-id="c9542-173">DarkYellow</span></span> |
| <span data-ttu-id="c9542-174">Preset19</span><span class="sxs-lookup"><span data-stu-id="c9542-174">Preset19</span></span> | <span data-ttu-id="c9542-175">DarkGreen</span><span class="sxs-lookup"><span data-stu-id="c9542-175">DarkGreen</span></span> |
| <span data-ttu-id="c9542-176">Preset20</span><span class="sxs-lookup"><span data-stu-id="c9542-176">Preset20</span></span> | <span data-ttu-id="c9542-177">DarkTeal</span><span class="sxs-lookup"><span data-stu-id="c9542-177">DarkTeal</span></span> |
| <span data-ttu-id="c9542-178">Preset21</span><span class="sxs-lookup"><span data-stu-id="c9542-178">Preset21</span></span> | <span data-ttu-id="c9542-179">DarkOlive</span><span class="sxs-lookup"><span data-stu-id="c9542-179">DarkOlive</span></span> |
| <span data-ttu-id="c9542-180">Preset22</span><span class="sxs-lookup"><span data-stu-id="c9542-180">Preset22</span></span> | <span data-ttu-id="c9542-181">DarkBlue</span><span class="sxs-lookup"><span data-stu-id="c9542-181">DarkBlue</span></span> |
| <span data-ttu-id="c9542-182">Preset23</span><span class="sxs-lookup"><span data-stu-id="c9542-182">Preset23</span></span> | <span data-ttu-id="c9542-183">DarkPurple</span><span class="sxs-lookup"><span data-stu-id="c9542-183">DarkPurple</span></span> |
| <span data-ttu-id="c9542-184">Preset24</span><span class="sxs-lookup"><span data-stu-id="c9542-184">Preset24</span></span> | <span data-ttu-id="c9542-185">DarkCranberry</span><span class="sxs-lookup"><span data-stu-id="c9542-185">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c9542-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9542-186">JSON representation</span></span>
<span data-ttu-id="c9542-187">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9542-187">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookCategory"
}-->

```json
{
  "color": "String",
  "displayName": "String"
}

```

## <a name="methods"></a><span data-ttu-id="c9542-188">Métodos</span><span class="sxs-lookup"><span data-stu-id="c9542-188">Methods</span></span>
| <span data-ttu-id="c9542-189">Método</span><span class="sxs-lookup"><span data-stu-id="c9542-189">Method</span></span>           | <span data-ttu-id="c9542-190">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c9542-190">Return Type</span></span>    |<span data-ttu-id="c9542-191">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9542-191">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c9542-192">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="c9542-192">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="c9542-193">Coleção [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="c9542-193">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="c9542-194">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="c9542-194">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="c9542-195">Obter categoria</span><span class="sxs-lookup"><span data-stu-id="c9542-195">Get category</span></span>](../api/outlookcategory-get.md) | [<span data-ttu-id="c9542-196">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="c9542-196">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="c9542-197">Obtenha as propriedades e as relações do objeto **outlookCategory** especificado.</span><span class="sxs-lookup"><span data-stu-id="c9542-197">Get the properties and relationships of the specified **outlookCategory** object.</span></span>|
|[<span data-ttu-id="c9542-198">Criar</span><span class="sxs-lookup"><span data-stu-id="c9542-198">Create</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="c9542-199">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="c9542-199">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="c9542-200">Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="c9542-200">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="c9542-201">Atualizar</span><span class="sxs-lookup"><span data-stu-id="c9542-201">Update</span></span>](../api/outlookcategory-update.md) | [<span data-ttu-id="c9542-202">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="c9542-202">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="c9542-203">Atualize a propriedade gravável, **color**, do objeto **outlookCategory** especificado.</span><span class="sxs-lookup"><span data-stu-id="c9542-203">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="c9542-204">Delete</span><span class="sxs-lookup"><span data-stu-id="c9542-204">Delete</span></span>](../api/outlookcategory-delete.md) | <span data-ttu-id="c9542-205">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c9542-205">None</span></span> |<span data-ttu-id="c9542-206">Exclua o objeto **outlookCategory** especificado.</span><span class="sxs-lookup"><span data-stu-id="c9542-206">Delete the specified **outlookCategory** object.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Warning: /api-reference/beta/resources/outlookcategory.md:\r\n      Failed to parse any rows out of table with headers: |Pre-set constant|Color mapped to in Outlook|"
  ]
}
-->
 


