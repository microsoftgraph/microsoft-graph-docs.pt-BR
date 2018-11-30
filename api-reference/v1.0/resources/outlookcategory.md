---
title: Tipo de recurso outlookCategory
description: Representa uma categoria pela qual um usuário pode agrupar itens do Outlook como mensagens e eventos. O usuário define categorias em uma lista mestra e pode aplicar um ou mais desses definidas pelo usuário
ms.openlocfilehash: b466b3964a5f817bfafd3a8a79d40c58a4d7b17b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004227"
---
# <a name="outlookcategory-resource-type"></a><span data-ttu-id="d1543-104">Tipo de recurso outlookCategory</span><span class="sxs-lookup"><span data-stu-id="d1543-104">outlookCategory resource type</span></span>


<span data-ttu-id="d1543-105">Representa uma categoria pela qual um usuário pode agrupar itens do Outlook como mensagens e eventos.</span><span class="sxs-lookup"><span data-stu-id="d1543-105">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="d1543-106">O usuário define categorias em uma lista mestra e pode aplicar uma ou mais das seguintes categorias definidas pelo usuário a um item.</span><span class="sxs-lookup"><span data-stu-id="d1543-106">The user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="d1543-107">Usando a API REST, é possível [criar](../api/outlookuser-post-mastercategories.md) e definir categorias na lista mestra de categorias para um usuário.</span><span class="sxs-lookup"><span data-stu-id="d1543-107">Using the REST API, you can [create](../api/outlookuser-post-mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="d1543-108">Também é possível [acessar essa lista mestra de categorias](../api/outlookuser-list-mastercategories.md), [obter uma categoria específica](../api/outlookcategory-get.md), [atualizar](../api/outlookcategory-update.md) a cor associada a uma categoria ou [excluir](../api/outlookcategory-delete.md) uma categoria.</span><span class="sxs-lookup"><span data-stu-id="d1543-108">You can also [get this master list of categories](../api/outlookuser-list-mastercategories.md), [get a specific category](../api/outlookcategory-get.md), [update](../api/outlookcategory-update.md) the color associated with a category, or [delete](../api/outlookcategory-delete.md) a category.</span></span> <span data-ttu-id="d1543-109">É possível aplicar uma categoria a um item atribuindo a propriedade **displayName** da categoria à coleção **categories** do item.</span><span class="sxs-lookup"><span data-stu-id="d1543-109">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="d1543-110">Entre os recursos que podem ser atribuídos às categorias estão [contact](contact.md), [event](event.md), [message](message.md) e [post](post.md).</span><span class="sxs-lookup"><span data-stu-id="d1543-110">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), and [post](post.md).</span></span>   

<span data-ttu-id="d1543-111">Cada categoria é atribuída por duas propriedades: **displayName** e **color**.</span><span class="sxs-lookup"><span data-stu-id="d1543-111">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="d1543-112">O valor **displayName** deve ser exclusivo na lista mestra de um usuário.</span><span class="sxs-lookup"><span data-stu-id="d1543-112">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="d1543-113">No entanto, o valor **color** não precisa ser exclusivo. Várias categorias na lista mestra podem ser mapeadas para a mesma cor.</span><span class="sxs-lookup"><span data-stu-id="d1543-113">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="d1543-114">É possível mapear até 25 cores diferentes para as categorias na lista mestra a um usuário.</span><span class="sxs-lookup"><span data-stu-id="d1543-114">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="d1543-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1543-115">Properties</span></span>
| <span data-ttu-id="d1543-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1543-116">Property</span></span>     | <span data-ttu-id="d1543-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1543-117">Type</span></span>   |<span data-ttu-id="d1543-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1543-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1543-119">displayName</span><span class="sxs-lookup"><span data-stu-id="d1543-119">displayName</span></span>|<span data-ttu-id="d1543-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1543-120">String</span></span>|<span data-ttu-id="d1543-121">Um nome exclusivo que identifica uma categoria na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="d1543-121">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="d1543-122">Após a criação de uma categoria, o nome não poderá ser alterado.</span><span class="sxs-lookup"><span data-stu-id="d1543-122">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="d1543-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d1543-123">Read-only.</span></span>|
|<span data-ttu-id="d1543-124">color</span><span class="sxs-lookup"><span data-stu-id="d1543-124">color</span></span>|<span data-ttu-id="d1543-125">categoryColor</span><span class="sxs-lookup"><span data-stu-id="d1543-125">categoryColor</span></span>|<span data-ttu-id="d1543-126">Uma constante de cor predefinida que caracteriza uma categoria e que é mapeada para uma das 25 cores predefinidas.</span><span class="sxs-lookup"><span data-stu-id="d1543-126">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="d1543-127">Confira a observação abaixo.</span><span class="sxs-lookup"><span data-stu-id="d1543-127">See the note below.</span></span> |

> <span data-ttu-id="d1543-128">**Observação** Os valores possíveis para **color** são constantes predefinidas como `None`, `preset0` e `preset1`.</span><span class="sxs-lookup"><span data-stu-id="d1543-128">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="d1543-129">Cada constante predefinida é mapeada para uma cor. A cor real depende do cliente do Outlook em que as categorias estão sendo exibidas.</span><span class="sxs-lookup"><span data-stu-id="d1543-129">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="d1543-130">A tabela a seguir mostra as cores mapeadas para cada constante predefinida do Outlook (cliente da área de trabalho).</span><span class="sxs-lookup"><span data-stu-id="d1543-130">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 

| <span data-ttu-id="d1543-131">Constante predefinida</span><span class="sxs-lookup"><span data-stu-id="d1543-131">Pre-set constant</span></span>  | <span data-ttu-id="d1543-132">Cor mapeada para no Outlook</span><span class="sxs-lookup"><span data-stu-id="d1543-132">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d1543-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d1543-133">None</span></span> | <span data-ttu-id="d1543-134">Nenhuma cor mapeada</span><span class="sxs-lookup"><span data-stu-id="d1543-134">No color mapped</span></span> |
| <span data-ttu-id="d1543-135">Preset0</span><span class="sxs-lookup"><span data-stu-id="d1543-135">Preset0</span></span> | <span data-ttu-id="d1543-136">Vermelho</span><span class="sxs-lookup"><span data-stu-id="d1543-136">Red</span></span> |
| <span data-ttu-id="d1543-137">Preset1</span><span class="sxs-lookup"><span data-stu-id="d1543-137">Preset1</span></span> | <span data-ttu-id="d1543-138">Laranja</span><span class="sxs-lookup"><span data-stu-id="d1543-138">Orange</span></span> |
| <span data-ttu-id="d1543-139">Preset2</span><span class="sxs-lookup"><span data-stu-id="d1543-139">Preset2</span></span> | <span data-ttu-id="d1543-140">Marrom</span><span class="sxs-lookup"><span data-stu-id="d1543-140">Brown</span></span> |
| <span data-ttu-id="d1543-141">Preset3</span><span class="sxs-lookup"><span data-stu-id="d1543-141">Preset3</span></span> | <span data-ttu-id="d1543-142">Amarelo</span><span class="sxs-lookup"><span data-stu-id="d1543-142">Yellow</span></span> |
| <span data-ttu-id="d1543-143">Preset4</span><span class="sxs-lookup"><span data-stu-id="d1543-143">Preset4</span></span> | <span data-ttu-id="d1543-144">Verde</span><span class="sxs-lookup"><span data-stu-id="d1543-144">Green</span></span> |
| <span data-ttu-id="d1543-145">Preset5</span><span class="sxs-lookup"><span data-stu-id="d1543-145">Preset5</span></span> | <span data-ttu-id="d1543-146">Azul-petróleo</span><span class="sxs-lookup"><span data-stu-id="d1543-146">Teal</span></span> |
| <span data-ttu-id="d1543-147">Preset6</span><span class="sxs-lookup"><span data-stu-id="d1543-147">Preset6</span></span> | <span data-ttu-id="d1543-148">Verde-oliva</span><span class="sxs-lookup"><span data-stu-id="d1543-148">Olive</span></span> |
| <span data-ttu-id="d1543-149">Preset7</span><span class="sxs-lookup"><span data-stu-id="d1543-149">Preset7</span></span> | <span data-ttu-id="d1543-150">Azul</span><span class="sxs-lookup"><span data-stu-id="d1543-150">Blue</span></span> |
| <span data-ttu-id="d1543-151">Preset8</span><span class="sxs-lookup"><span data-stu-id="d1543-151">Preset8</span></span> | <span data-ttu-id="d1543-152">Roxo</span><span class="sxs-lookup"><span data-stu-id="d1543-152">Purple</span></span> |
| <span data-ttu-id="d1543-153">Preset9</span><span class="sxs-lookup"><span data-stu-id="d1543-153">Preset9</span></span> | <span data-ttu-id="d1543-154">Cranberry</span><span class="sxs-lookup"><span data-stu-id="d1543-154">Cranberry</span></span> |
| <span data-ttu-id="d1543-155">Preset10</span><span class="sxs-lookup"><span data-stu-id="d1543-155">Preset10</span></span> | <span data-ttu-id="d1543-156">Steel</span><span class="sxs-lookup"><span data-stu-id="d1543-156">Steel</span></span> |
| <span data-ttu-id="d1543-157">Preset11</span><span class="sxs-lookup"><span data-stu-id="d1543-157">Preset11</span></span> | <span data-ttu-id="d1543-158">DarkSteel</span><span class="sxs-lookup"><span data-stu-id="d1543-158">DarkSteel</span></span> |
| <span data-ttu-id="d1543-159">Preset12</span><span class="sxs-lookup"><span data-stu-id="d1543-159">Preset12</span></span> | <span data-ttu-id="d1543-160">Cinza</span><span class="sxs-lookup"><span data-stu-id="d1543-160">Gray</span></span> |
| <span data-ttu-id="d1543-161">Preset13</span><span class="sxs-lookup"><span data-stu-id="d1543-161">Preset13</span></span> | <span data-ttu-id="d1543-162">DarkGray</span><span class="sxs-lookup"><span data-stu-id="d1543-162">DarkGray</span></span> |
| <span data-ttu-id="d1543-163">Preset14</span><span class="sxs-lookup"><span data-stu-id="d1543-163">Preset14</span></span> | <span data-ttu-id="d1543-164">Preto</span><span class="sxs-lookup"><span data-stu-id="d1543-164">Black</span></span> |
| <span data-ttu-id="d1543-165">Preset15</span><span class="sxs-lookup"><span data-stu-id="d1543-165">Preset15</span></span> | <span data-ttu-id="d1543-166">DarkRed</span><span class="sxs-lookup"><span data-stu-id="d1543-166">DarkRed</span></span> |
| <span data-ttu-id="d1543-167">Preset16</span><span class="sxs-lookup"><span data-stu-id="d1543-167">Preset16</span></span> | <span data-ttu-id="d1543-168">DarkOrange</span><span class="sxs-lookup"><span data-stu-id="d1543-168">DarkOrange</span></span> |
| <span data-ttu-id="d1543-169">Preset17</span><span class="sxs-lookup"><span data-stu-id="d1543-169">Preset17</span></span> | <span data-ttu-id="d1543-170">DarkBrown</span><span class="sxs-lookup"><span data-stu-id="d1543-170">DarkBrown</span></span> |
| <span data-ttu-id="d1543-171">Preset18</span><span class="sxs-lookup"><span data-stu-id="d1543-171">Preset18</span></span> | <span data-ttu-id="d1543-172">DarkYellow</span><span class="sxs-lookup"><span data-stu-id="d1543-172">DarkYellow</span></span> |
| <span data-ttu-id="d1543-173">Preset19</span><span class="sxs-lookup"><span data-stu-id="d1543-173">Preset19</span></span> | <span data-ttu-id="d1543-174">DarkGreen</span><span class="sxs-lookup"><span data-stu-id="d1543-174">DarkGreen</span></span> |
| <span data-ttu-id="d1543-175">Preset20</span><span class="sxs-lookup"><span data-stu-id="d1543-175">Preset20</span></span> | <span data-ttu-id="d1543-176">DarkTeal</span><span class="sxs-lookup"><span data-stu-id="d1543-176">DarkTeal</span></span> |
| <span data-ttu-id="d1543-177">Preset21</span><span class="sxs-lookup"><span data-stu-id="d1543-177">Preset21</span></span> | <span data-ttu-id="d1543-178">DarkOlive</span><span class="sxs-lookup"><span data-stu-id="d1543-178">DarkOlive</span></span> |
| <span data-ttu-id="d1543-179">Preset22</span><span class="sxs-lookup"><span data-stu-id="d1543-179">Preset22</span></span> | <span data-ttu-id="d1543-180">DarkBlue</span><span class="sxs-lookup"><span data-stu-id="d1543-180">DarkBlue</span></span> |
| <span data-ttu-id="d1543-181">Preset23</span><span class="sxs-lookup"><span data-stu-id="d1543-181">Preset23</span></span> | <span data-ttu-id="d1543-182">DarkPurple</span><span class="sxs-lookup"><span data-stu-id="d1543-182">DarkPurple</span></span> |
| <span data-ttu-id="d1543-183">Preset24</span><span class="sxs-lookup"><span data-stu-id="d1543-183">Preset24</span></span> | <span data-ttu-id="d1543-184">DarkCranberry</span><span class="sxs-lookup"><span data-stu-id="d1543-184">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d1543-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1543-185">JSON representation</span></span>
<span data-ttu-id="d1543-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d1543-186">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookCategory"
}-->

```json
{
  "color": "String",
  "displayName": "String"
}

```

## <a name="methods"></a><span data-ttu-id="d1543-187">Métodos</span><span class="sxs-lookup"><span data-stu-id="d1543-187">Methods</span></span>
| <span data-ttu-id="d1543-188">Método</span><span class="sxs-lookup"><span data-stu-id="d1543-188">Method</span></span>           | <span data-ttu-id="d1543-189">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d1543-189">Return Type</span></span>    |<span data-ttu-id="d1543-190">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1543-190">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d1543-191">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="d1543-191">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="d1543-192">Coleção [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="d1543-192">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="d1543-193">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="d1543-193">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="d1543-194">Obter categoria</span><span class="sxs-lookup"><span data-stu-id="d1543-194">Get category</span></span>](../api/outlookcategory-get.md) | [<span data-ttu-id="d1543-195">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="d1543-195">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="d1543-196">Obtenha as propriedades e as relações do objeto **outlookCategory** especificado.</span><span class="sxs-lookup"><span data-stu-id="d1543-196">Get the properties and relationships of the specified **outlookCategory** object.</span></span>|
|[<span data-ttu-id="d1543-197">Criar</span><span class="sxs-lookup"><span data-stu-id="d1543-197">Create</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="d1543-198">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="d1543-198">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="d1543-199">Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="d1543-199">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="d1543-200">Atualizar</span><span class="sxs-lookup"><span data-stu-id="d1543-200">Update</span></span>](../api/outlookcategory-update.md) | [<span data-ttu-id="d1543-201">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="d1543-201">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="d1543-202">Atualize a propriedade gravável, **color**, do objeto **outlookCategory** especificado.</span><span class="sxs-lookup"><span data-stu-id="d1543-202">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="d1543-203">Excluir</span><span class="sxs-lookup"><span data-stu-id="d1543-203">Delete</span></span>](../api/outlookcategory-delete.md) | <span data-ttu-id="d1543-204">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d1543-204">None</span></span> |<span data-ttu-id="d1543-205">Exclua o objeto **outlookCategory** especificado.</span><span class="sxs-lookup"><span data-stu-id="d1543-205">Delete the specified **outlookCategory** object.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/resources/outlookcategory.md:
      Failed to parse any rows out of table with headers: |Pre-set constant|Color mapped to in Outlook|"
  ],
  "tocPath": ""
}-->
 