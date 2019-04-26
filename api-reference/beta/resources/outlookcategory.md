---
title: Tipo de recurso outlookCategory
description: Representa uma categoria pela qual um usuário pode agrupar itens do Outlook como mensagens e eventos. No Outlook, o usuário define categorias em uma lista mestre e pode aplicar uma ou mais dessas definições de usuário
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 5124a681cd4dd1f37ef1ecfea250eb6eb2d228a3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568599"
---
# <a name="outlookcategory-resource-type"></a><span data-ttu-id="8ee7e-104">Tipo de recurso outlookCategory</span><span class="sxs-lookup"><span data-stu-id="8ee7e-104">outlookCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ee7e-105">Representa uma categoria pela qual um usuário pode agrupar itens do Outlook como mensagens e eventos.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-105">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="8ee7e-106">No Outlook, o usuário define categorias em uma lista mestre e pode aplicar uma ou mais dessas categorias definidas pelo usuário a um item.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-106">In Outlook, the user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="8ee7e-107">Usando a API REST, é possível [criar](../api/outlookuser-post-mastercategories.md) e definir categorias na lista mestra de categorias para um usuário.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-107">Using the REST API, you can [create](../api/outlookuser-post-mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="8ee7e-108">Também é possível [acessar essa lista mestra de categorias](../api/outlookuser-list-mastercategories.md), [obter uma categoria específica](../api/outlookcategory-get.md), [atualizar](../api/outlookcategory-update.md) a cor associada a uma categoria ou [excluir](../api/outlookcategory-delete.md) uma categoria.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-108">You can also [get this master list of categories](../api/outlookuser-list-mastercategories.md), [get a specific category](../api/outlookcategory-get.md), [update](../api/outlookcategory-update.md) the color associated with a category, or [delete](../api/outlookcategory-delete.md) a category.</span></span> <span data-ttu-id="8ee7e-109">É possível aplicar uma categoria a um item atribuindo a propriedade **displayName** da categoria à coleção **categories** do item.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-109">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="8ee7e-110">Os recursos que podem ser atribuídos categorias incluem [contato](contact.md), [evento](event.md), [mensagem](message.md), [outlookTask](outlooktask.md)e [post](post.md).</span><span class="sxs-lookup"><span data-stu-id="8ee7e-110">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), [outlookTask](outlooktask.md), and [post](post.md).</span></span>   

<span data-ttu-id="8ee7e-111">Cada categoria é atribuída por duas propriedades: **displayName** e **color**.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-111">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="8ee7e-112">O valor **displayName** deve ser exclusivo na lista mestra de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-112">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="8ee7e-113">No entanto, o valor **color** não precisa ser exclusivo. Várias categorias na lista mestra podem ser mapeadas para a mesma cor.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-113">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="8ee7e-114">É possível mapear até 25 cores diferentes para as categorias na lista mestra a um usuário.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-114">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="8ee7e-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ee7e-115">Properties</span></span>
| <span data-ttu-id="8ee7e-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ee7e-116">Property</span></span>     | <span data-ttu-id="8ee7e-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ee7e-117">Type</span></span>   |<span data-ttu-id="8ee7e-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ee7e-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ee7e-119">displayName</span><span class="sxs-lookup"><span data-stu-id="8ee7e-119">displayName</span></span>|<span data-ttu-id="8ee7e-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ee7e-120">String</span></span>|<span data-ttu-id="8ee7e-121">Um nome exclusivo que identifica uma categoria na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-121">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="8ee7e-122">Após a criação de uma categoria, o nome não poderá ser alterado.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-122">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="8ee7e-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-123">Read-only.</span></span>|
|<span data-ttu-id="8ee7e-124">color</span><span class="sxs-lookup"><span data-stu-id="8ee7e-124">color</span></span>|<span data-ttu-id="8ee7e-125">String</span><span class="sxs-lookup"><span data-stu-id="8ee7e-125">String</span></span>|<span data-ttu-id="8ee7e-126">Uma constante de cor predefinida que caracteriza uma categoria e que é mapeada para uma das 25 cores predefinidas.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-126">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="8ee7e-127">Confira a observação abaixo.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-127">See the note below.</span></span> |

> <span data-ttu-id="8ee7e-128">**Observação** Os valores possíveis para **color** são constantes predefinidas como `None`, `preset0` e `preset1`.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-128">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="8ee7e-129">Cada constante predefinida é mapeada para uma cor. A cor real depende do cliente do Outlook em que as categorias estão sendo exibidas.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-129">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="8ee7e-130">A tabela a seguir mostra as cores mapeadas para cada constante predefinida do Outlook (cliente da área de trabalho).</span><span class="sxs-lookup"><span data-stu-id="8ee7e-130">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 


| <span data-ttu-id="8ee7e-131">Constante predefinida</span><span class="sxs-lookup"><span data-stu-id="8ee7e-131">Pre-set constant</span></span>  | <span data-ttu-id="8ee7e-132">Cor mapeada para no Outlook</span><span class="sxs-lookup"><span data-stu-id="8ee7e-132">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8ee7e-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ee7e-133">None</span></span> | <span data-ttu-id="8ee7e-134">Nenhuma cor mapeada</span><span class="sxs-lookup"><span data-stu-id="8ee7e-134">No color mapped</span></span> |
| <span data-ttu-id="8ee7e-135">Preset0</span><span class="sxs-lookup"><span data-stu-id="8ee7e-135">Preset0</span></span> | <span data-ttu-id="8ee7e-136">Vermelho</span><span class="sxs-lookup"><span data-stu-id="8ee7e-136">Red</span></span> |
| <span data-ttu-id="8ee7e-137">Preset1</span><span class="sxs-lookup"><span data-stu-id="8ee7e-137">Preset1</span></span> | <span data-ttu-id="8ee7e-138">Laranja</span><span class="sxs-lookup"><span data-stu-id="8ee7e-138">Orange</span></span> |
| <span data-ttu-id="8ee7e-139">Preset2</span><span class="sxs-lookup"><span data-stu-id="8ee7e-139">Preset2</span></span> | <span data-ttu-id="8ee7e-140">Marrom</span><span class="sxs-lookup"><span data-stu-id="8ee7e-140">Brown</span></span> |
| <span data-ttu-id="8ee7e-141">Preset3</span><span class="sxs-lookup"><span data-stu-id="8ee7e-141">Preset3</span></span> | <span data-ttu-id="8ee7e-142">Amarelo</span><span class="sxs-lookup"><span data-stu-id="8ee7e-142">Yellow</span></span> |
| <span data-ttu-id="8ee7e-143">Preset4</span><span class="sxs-lookup"><span data-stu-id="8ee7e-143">Preset4</span></span> | <span data-ttu-id="8ee7e-144">Verde</span><span class="sxs-lookup"><span data-stu-id="8ee7e-144">Green</span></span> |
| <span data-ttu-id="8ee7e-145">Preset5</span><span class="sxs-lookup"><span data-stu-id="8ee7e-145">Preset5</span></span> | <span data-ttu-id="8ee7e-146">Azul-petróleo</span><span class="sxs-lookup"><span data-stu-id="8ee7e-146">Teal</span></span> |
| <span data-ttu-id="8ee7e-147">Preset6</span><span class="sxs-lookup"><span data-stu-id="8ee7e-147">Preset6</span></span> | <span data-ttu-id="8ee7e-148">Verde-oliva</span><span class="sxs-lookup"><span data-stu-id="8ee7e-148">Olive</span></span> |
| <span data-ttu-id="8ee7e-149">Preset7</span><span class="sxs-lookup"><span data-stu-id="8ee7e-149">Preset7</span></span> | <span data-ttu-id="8ee7e-150">Azul</span><span class="sxs-lookup"><span data-stu-id="8ee7e-150">Blue</span></span> |
| <span data-ttu-id="8ee7e-151">Preset8</span><span class="sxs-lookup"><span data-stu-id="8ee7e-151">Preset8</span></span> | <span data-ttu-id="8ee7e-152">Roxo</span><span class="sxs-lookup"><span data-stu-id="8ee7e-152">Purple</span></span> |
| <span data-ttu-id="8ee7e-153">Preset9</span><span class="sxs-lookup"><span data-stu-id="8ee7e-153">Preset9</span></span> | <span data-ttu-id="8ee7e-154">Cranberry</span><span class="sxs-lookup"><span data-stu-id="8ee7e-154">Cranberry</span></span> |
| <span data-ttu-id="8ee7e-155">Preset10</span><span class="sxs-lookup"><span data-stu-id="8ee7e-155">Preset10</span></span> | <span data-ttu-id="8ee7e-156">Steel</span><span class="sxs-lookup"><span data-stu-id="8ee7e-156">Steel</span></span> |
| <span data-ttu-id="8ee7e-157">Preset11</span><span class="sxs-lookup"><span data-stu-id="8ee7e-157">Preset11</span></span> | <span data-ttu-id="8ee7e-158">DarkSteel</span><span class="sxs-lookup"><span data-stu-id="8ee7e-158">DarkSteel</span></span> |
| <span data-ttu-id="8ee7e-159">Preset12</span><span class="sxs-lookup"><span data-stu-id="8ee7e-159">Preset12</span></span> | <span data-ttu-id="8ee7e-160">Cinza</span><span class="sxs-lookup"><span data-stu-id="8ee7e-160">Gray</span></span> |
| <span data-ttu-id="8ee7e-161">Preset13</span><span class="sxs-lookup"><span data-stu-id="8ee7e-161">Preset13</span></span> | <span data-ttu-id="8ee7e-162">DarkGray</span><span class="sxs-lookup"><span data-stu-id="8ee7e-162">DarkGray</span></span> |
| <span data-ttu-id="8ee7e-163">Preset14</span><span class="sxs-lookup"><span data-stu-id="8ee7e-163">Preset14</span></span> | <span data-ttu-id="8ee7e-164">Preto</span><span class="sxs-lookup"><span data-stu-id="8ee7e-164">Black</span></span> |
| <span data-ttu-id="8ee7e-165">Preset15</span><span class="sxs-lookup"><span data-stu-id="8ee7e-165">Preset15</span></span> | <span data-ttu-id="8ee7e-166">DarkRed</span><span class="sxs-lookup"><span data-stu-id="8ee7e-166">DarkRed</span></span> |
| <span data-ttu-id="8ee7e-167">Preset16</span><span class="sxs-lookup"><span data-stu-id="8ee7e-167">Preset16</span></span> | <span data-ttu-id="8ee7e-168">DarkOrange</span><span class="sxs-lookup"><span data-stu-id="8ee7e-168">DarkOrange</span></span> |
| <span data-ttu-id="8ee7e-169">Preset17</span><span class="sxs-lookup"><span data-stu-id="8ee7e-169">Preset17</span></span> | <span data-ttu-id="8ee7e-170">DarkBrown</span><span class="sxs-lookup"><span data-stu-id="8ee7e-170">DarkBrown</span></span> |
| <span data-ttu-id="8ee7e-171">Preset18</span><span class="sxs-lookup"><span data-stu-id="8ee7e-171">Preset18</span></span> | <span data-ttu-id="8ee7e-172">DarkYellow</span><span class="sxs-lookup"><span data-stu-id="8ee7e-172">DarkYellow</span></span> |
| <span data-ttu-id="8ee7e-173">Preset19</span><span class="sxs-lookup"><span data-stu-id="8ee7e-173">Preset19</span></span> | <span data-ttu-id="8ee7e-174">DarkGreen</span><span class="sxs-lookup"><span data-stu-id="8ee7e-174">DarkGreen</span></span> |
| <span data-ttu-id="8ee7e-175">Preset20</span><span class="sxs-lookup"><span data-stu-id="8ee7e-175">Preset20</span></span> | <span data-ttu-id="8ee7e-176">DarkTeal</span><span class="sxs-lookup"><span data-stu-id="8ee7e-176">DarkTeal</span></span> |
| <span data-ttu-id="8ee7e-177">Preset21</span><span class="sxs-lookup"><span data-stu-id="8ee7e-177">Preset21</span></span> | <span data-ttu-id="8ee7e-178">DarkOlive</span><span class="sxs-lookup"><span data-stu-id="8ee7e-178">DarkOlive</span></span> |
| <span data-ttu-id="8ee7e-179">Preset22</span><span class="sxs-lookup"><span data-stu-id="8ee7e-179">Preset22</span></span> | <span data-ttu-id="8ee7e-180">DarkBlue</span><span class="sxs-lookup"><span data-stu-id="8ee7e-180">DarkBlue</span></span> |
| <span data-ttu-id="8ee7e-181">Preset23</span><span class="sxs-lookup"><span data-stu-id="8ee7e-181">Preset23</span></span> | <span data-ttu-id="8ee7e-182">DarkPurple</span><span class="sxs-lookup"><span data-stu-id="8ee7e-182">DarkPurple</span></span> |
| <span data-ttu-id="8ee7e-183">Preset24</span><span class="sxs-lookup"><span data-stu-id="8ee7e-183">Preset24</span></span> | <span data-ttu-id="8ee7e-184">DarkCranberry</span><span class="sxs-lookup"><span data-stu-id="8ee7e-184">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8ee7e-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ee7e-185">JSON representation</span></span>
<span data-ttu-id="8ee7e-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-186">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="8ee7e-187">Métodos</span><span class="sxs-lookup"><span data-stu-id="8ee7e-187">Methods</span></span>
| <span data-ttu-id="8ee7e-188">Método</span><span class="sxs-lookup"><span data-stu-id="8ee7e-188">Method</span></span>           | <span data-ttu-id="8ee7e-189">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8ee7e-189">Return Type</span></span>    |<span data-ttu-id="8ee7e-190">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ee7e-190">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8ee7e-191">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="8ee7e-191">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="8ee7e-192">Coleção [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="8ee7e-192">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="8ee7e-193">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-193">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="8ee7e-194">Obter categoria</span><span class="sxs-lookup"><span data-stu-id="8ee7e-194">Get category</span></span>](../api/outlookcategory-get.md) | [<span data-ttu-id="8ee7e-195">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="8ee7e-195">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="8ee7e-196">Obtenha as propriedades e as relações do objeto **outlookCategory** especificado.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-196">Get the properties and relationships of the specified **outlookCategory** object.</span></span>|
|[<span data-ttu-id="8ee7e-197">Criar</span><span class="sxs-lookup"><span data-stu-id="8ee7e-197">Create</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="8ee7e-198">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="8ee7e-198">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="8ee7e-199">Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-199">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="8ee7e-200">Atualizar</span><span class="sxs-lookup"><span data-stu-id="8ee7e-200">Update</span></span>](../api/outlookcategory-update.md) | [<span data-ttu-id="8ee7e-201">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="8ee7e-201">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="8ee7e-202">Atualize a propriedade gravável, **color**, do objeto **outlookCategory** especificado.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-202">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="8ee7e-203">Excluir</span><span class="sxs-lookup"><span data-stu-id="8ee7e-203">Delete</span></span>](../api/outlookcategory-delete.md) | <span data-ttu-id="8ee7e-204">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ee7e-204">None</span></span> |<span data-ttu-id="8ee7e-205">Exclua o objeto **outlookCategory** especificado.</span><span class="sxs-lookup"><span data-stu-id="8ee7e-205">Delete the specified **outlookCategory** object.</span></span> |


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
 
