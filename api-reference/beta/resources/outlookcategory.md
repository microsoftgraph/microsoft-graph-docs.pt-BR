---
title: Tipo de recurso outlookCategory
description: Representa uma categoria pela qual um usuário pode agrupar itens do Outlook como mensagens e eventos. No Outlook, o usuário define as categorias em uma lista mestra e pode aplicar um ou mais desses definidas pelo usuário
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 9e4aa0c381e42522f80d933052ad7f0386643c60
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925165"
---
# <a name="outlookcategory-resource-type"></a><span data-ttu-id="ef7fb-104">Tipo de recurso outlookCategory</span><span class="sxs-lookup"><span data-stu-id="ef7fb-104">outlookCategory resource type</span></span>

> <span data-ttu-id="ef7fb-105">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ef7fb-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ef7fb-107">Representa uma categoria pela qual um usuário pode agrupar itens do Outlook como mensagens e eventos.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-107">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="ef7fb-108">No Outlook, o usuário define as categorias em uma lista mestra e pode aplicar uma ou mais destas categorias definidas pelo usuário a um item.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-108">In Outlook, the user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="ef7fb-109">Usando a API REST, é possível [criar](../api/outlookuser-post-mastercategories.md) e definir categorias na lista mestra de categorias para um usuário.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-109">Using the REST API, you can [create](../api/outlookuser-post-mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="ef7fb-110">Também é possível [acessar essa lista mestra de categorias](../api/outlookuser-list-mastercategories.md), [obter uma categoria específica](../api/outlookcategory-get.md), [atualizar](../api/outlookcategory-update.md) a cor associada a uma categoria ou [excluir](../api/outlookcategory-delete.md) uma categoria.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-110">You can also [get this master list of categories](../api/outlookuser-list-mastercategories.md), [get a specific category](../api/outlookcategory-get.md), [update](../api/outlookcategory-update.md) the color associated with a category, or [delete](../api/outlookcategory-delete.md) a category.</span></span> <span data-ttu-id="ef7fb-111">É possível aplicar uma categoria a um item atribuindo a propriedade **displayName** da categoria à coleção **categories** do item.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-111">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="ef7fb-112">Os recursos que podem ser atribuídos categorias incluem [Contatos](contact.md), [eventos](event.md), [mensagem](message.md), [outlookTask](outlooktask.md)e [postar](post.md).</span><span class="sxs-lookup"><span data-stu-id="ef7fb-112">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), [outlookTask](outlooktask.md), and [post](post.md).</span></span>   

<span data-ttu-id="ef7fb-113">Cada categoria é atribuída por duas propriedades: **displayName** e **color**.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-113">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="ef7fb-114">O valor **displayName** deve ser exclusivo na lista mestra de um usuário.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-114">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="ef7fb-115">No entanto, o valor **color** não precisa ser exclusivo. Várias categorias na lista mestra podem ser mapeadas para a mesma cor.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-115">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="ef7fb-116">É possível mapear até 25 cores diferentes para as categorias na lista mestra a um usuário.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-116">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="ef7fb-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef7fb-117">Properties</span></span>
| <span data-ttu-id="ef7fb-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef7fb-118">Property</span></span>     | <span data-ttu-id="ef7fb-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef7fb-119">Type</span></span>   |<span data-ttu-id="ef7fb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef7fb-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef7fb-121">displayName</span><span class="sxs-lookup"><span data-stu-id="ef7fb-121">displayName</span></span>|<span data-ttu-id="ef7fb-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef7fb-122">String</span></span>|<span data-ttu-id="ef7fb-123">Um nome exclusivo que identifica uma categoria na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-123">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="ef7fb-124">Após a criação de uma categoria, o nome não poderá ser alterado.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-124">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="ef7fb-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-125">Read-only.</span></span>|
|<span data-ttu-id="ef7fb-126">color</span><span class="sxs-lookup"><span data-stu-id="ef7fb-126">color</span></span>|<span data-ttu-id="ef7fb-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef7fb-127">String</span></span>|<span data-ttu-id="ef7fb-128">Uma constante de cor predefinida que caracteriza uma categoria e que é mapeada para uma das 25 cores predefinidas.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-128">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="ef7fb-129">Confira a observação abaixo.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-129">See the note below.</span></span> |

> <span data-ttu-id="ef7fb-130">**Observação** Os valores possíveis para **color** são constantes predefinidas como `None`, `preset0` e `preset1`.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-130">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="ef7fb-131">Cada constante predefinida é mapeada para uma cor. A cor real depende do cliente do Outlook em que as categorias estão sendo exibidas.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-131">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="ef7fb-132">A tabela a seguir mostra as cores mapeadas para cada constante predefinida do Outlook (cliente da área de trabalho).</span><span class="sxs-lookup"><span data-stu-id="ef7fb-132">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 


| <span data-ttu-id="ef7fb-133">Constante predefinida</span><span class="sxs-lookup"><span data-stu-id="ef7fb-133">Pre-set constant</span></span>  | <span data-ttu-id="ef7fb-134">Cor mapeada para no Outlook</span><span class="sxs-lookup"><span data-stu-id="ef7fb-134">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ef7fb-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ef7fb-135">None</span></span> | <span data-ttu-id="ef7fb-136">Nenhuma cor mapeada</span><span class="sxs-lookup"><span data-stu-id="ef7fb-136">No color mapped</span></span> |
| <span data-ttu-id="ef7fb-137">Preset0</span><span class="sxs-lookup"><span data-stu-id="ef7fb-137">Preset0</span></span> | <span data-ttu-id="ef7fb-138">Vermelho</span><span class="sxs-lookup"><span data-stu-id="ef7fb-138">Red</span></span> |
| <span data-ttu-id="ef7fb-139">Preset1</span><span class="sxs-lookup"><span data-stu-id="ef7fb-139">Preset1</span></span> | <span data-ttu-id="ef7fb-140">Laranja</span><span class="sxs-lookup"><span data-stu-id="ef7fb-140">Orange</span></span> |
| <span data-ttu-id="ef7fb-141">Preset2</span><span class="sxs-lookup"><span data-stu-id="ef7fb-141">Preset2</span></span> | <span data-ttu-id="ef7fb-142">Marrom</span><span class="sxs-lookup"><span data-stu-id="ef7fb-142">Brown</span></span> |
| <span data-ttu-id="ef7fb-143">Preset3</span><span class="sxs-lookup"><span data-stu-id="ef7fb-143">Preset3</span></span> | <span data-ttu-id="ef7fb-144">Amarelo</span><span class="sxs-lookup"><span data-stu-id="ef7fb-144">Yellow</span></span> |
| <span data-ttu-id="ef7fb-145">Preset4</span><span class="sxs-lookup"><span data-stu-id="ef7fb-145">Preset4</span></span> | <span data-ttu-id="ef7fb-146">Verde</span><span class="sxs-lookup"><span data-stu-id="ef7fb-146">Green</span></span> |
| <span data-ttu-id="ef7fb-147">Preset5</span><span class="sxs-lookup"><span data-stu-id="ef7fb-147">Preset5</span></span> | <span data-ttu-id="ef7fb-148">Azul-petróleo</span><span class="sxs-lookup"><span data-stu-id="ef7fb-148">Teal</span></span> |
| <span data-ttu-id="ef7fb-149">Preset6</span><span class="sxs-lookup"><span data-stu-id="ef7fb-149">Preset6</span></span> | <span data-ttu-id="ef7fb-150">Verde-oliva</span><span class="sxs-lookup"><span data-stu-id="ef7fb-150">Olive</span></span> |
| <span data-ttu-id="ef7fb-151">Preset7</span><span class="sxs-lookup"><span data-stu-id="ef7fb-151">Preset7</span></span> | <span data-ttu-id="ef7fb-152">Azul</span><span class="sxs-lookup"><span data-stu-id="ef7fb-152">Blue</span></span> |
| <span data-ttu-id="ef7fb-153">Preset8</span><span class="sxs-lookup"><span data-stu-id="ef7fb-153">Preset8</span></span> | <span data-ttu-id="ef7fb-154">Roxo</span><span class="sxs-lookup"><span data-stu-id="ef7fb-154">Purple</span></span> |
| <span data-ttu-id="ef7fb-155">Preset9</span><span class="sxs-lookup"><span data-stu-id="ef7fb-155">Preset9</span></span> | <span data-ttu-id="ef7fb-156">Cranberry</span><span class="sxs-lookup"><span data-stu-id="ef7fb-156">Cranberry</span></span> |
| <span data-ttu-id="ef7fb-157">Preset10</span><span class="sxs-lookup"><span data-stu-id="ef7fb-157">Preset10</span></span> | <span data-ttu-id="ef7fb-158">Steel</span><span class="sxs-lookup"><span data-stu-id="ef7fb-158">Steel</span></span> |
| <span data-ttu-id="ef7fb-159">Preset11</span><span class="sxs-lookup"><span data-stu-id="ef7fb-159">Preset11</span></span> | <span data-ttu-id="ef7fb-160">DarkSteel</span><span class="sxs-lookup"><span data-stu-id="ef7fb-160">DarkSteel</span></span> |
| <span data-ttu-id="ef7fb-161">Preset12</span><span class="sxs-lookup"><span data-stu-id="ef7fb-161">Preset12</span></span> | <span data-ttu-id="ef7fb-162">Cinza</span><span class="sxs-lookup"><span data-stu-id="ef7fb-162">Gray</span></span> |
| <span data-ttu-id="ef7fb-163">Preset13</span><span class="sxs-lookup"><span data-stu-id="ef7fb-163">Preset13</span></span> | <span data-ttu-id="ef7fb-164">DarkGray</span><span class="sxs-lookup"><span data-stu-id="ef7fb-164">DarkGray</span></span> |
| <span data-ttu-id="ef7fb-165">Preset14</span><span class="sxs-lookup"><span data-stu-id="ef7fb-165">Preset14</span></span> | <span data-ttu-id="ef7fb-166">Preto</span><span class="sxs-lookup"><span data-stu-id="ef7fb-166">Black</span></span> |
| <span data-ttu-id="ef7fb-167">Preset15</span><span class="sxs-lookup"><span data-stu-id="ef7fb-167">Preset15</span></span> | <span data-ttu-id="ef7fb-168">DarkRed</span><span class="sxs-lookup"><span data-stu-id="ef7fb-168">DarkRed</span></span> |
| <span data-ttu-id="ef7fb-169">Preset16</span><span class="sxs-lookup"><span data-stu-id="ef7fb-169">Preset16</span></span> | <span data-ttu-id="ef7fb-170">DarkOrange</span><span class="sxs-lookup"><span data-stu-id="ef7fb-170">DarkOrange</span></span> |
| <span data-ttu-id="ef7fb-171">Preset17</span><span class="sxs-lookup"><span data-stu-id="ef7fb-171">Preset17</span></span> | <span data-ttu-id="ef7fb-172">DarkBrown</span><span class="sxs-lookup"><span data-stu-id="ef7fb-172">DarkBrown</span></span> |
| <span data-ttu-id="ef7fb-173">Preset18</span><span class="sxs-lookup"><span data-stu-id="ef7fb-173">Preset18</span></span> | <span data-ttu-id="ef7fb-174">DarkYellow</span><span class="sxs-lookup"><span data-stu-id="ef7fb-174">DarkYellow</span></span> |
| <span data-ttu-id="ef7fb-175">Preset19</span><span class="sxs-lookup"><span data-stu-id="ef7fb-175">Preset19</span></span> | <span data-ttu-id="ef7fb-176">DarkGreen</span><span class="sxs-lookup"><span data-stu-id="ef7fb-176">DarkGreen</span></span> |
| <span data-ttu-id="ef7fb-177">Preset20</span><span class="sxs-lookup"><span data-stu-id="ef7fb-177">Preset20</span></span> | <span data-ttu-id="ef7fb-178">DarkTeal</span><span class="sxs-lookup"><span data-stu-id="ef7fb-178">DarkTeal</span></span> |
| <span data-ttu-id="ef7fb-179">Preset21</span><span class="sxs-lookup"><span data-stu-id="ef7fb-179">Preset21</span></span> | <span data-ttu-id="ef7fb-180">DarkOlive</span><span class="sxs-lookup"><span data-stu-id="ef7fb-180">DarkOlive</span></span> |
| <span data-ttu-id="ef7fb-181">Preset22</span><span class="sxs-lookup"><span data-stu-id="ef7fb-181">Preset22</span></span> | <span data-ttu-id="ef7fb-182">DarkBlue</span><span class="sxs-lookup"><span data-stu-id="ef7fb-182">DarkBlue</span></span> |
| <span data-ttu-id="ef7fb-183">Preset23</span><span class="sxs-lookup"><span data-stu-id="ef7fb-183">Preset23</span></span> | <span data-ttu-id="ef7fb-184">DarkPurple</span><span class="sxs-lookup"><span data-stu-id="ef7fb-184">DarkPurple</span></span> |
| <span data-ttu-id="ef7fb-185">Preset24</span><span class="sxs-lookup"><span data-stu-id="ef7fb-185">Preset24</span></span> | <span data-ttu-id="ef7fb-186">DarkCranberry</span><span class="sxs-lookup"><span data-stu-id="ef7fb-186">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ef7fb-187">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef7fb-187">JSON representation</span></span>
<span data-ttu-id="ef7fb-188">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-188">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="ef7fb-189">Métodos</span><span class="sxs-lookup"><span data-stu-id="ef7fb-189">Methods</span></span>
| <span data-ttu-id="ef7fb-190">Método</span><span class="sxs-lookup"><span data-stu-id="ef7fb-190">Method</span></span>           | <span data-ttu-id="ef7fb-191">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ef7fb-191">Return Type</span></span>    |<span data-ttu-id="ef7fb-192">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef7fb-192">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ef7fb-193">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="ef7fb-193">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="ef7fb-194">Coleção [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="ef7fb-194">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="ef7fb-195">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-195">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="ef7fb-196">Obter categoria</span><span class="sxs-lookup"><span data-stu-id="ef7fb-196">Get category</span></span>](../api/outlookcategory-get.md) | [<span data-ttu-id="ef7fb-197">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="ef7fb-197">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="ef7fb-198">Obtenha as propriedades e as relações do objeto **outlookCategory** especificado.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-198">Get the properties and relationships of the specified **outlookCategory** object.</span></span>|
|[<span data-ttu-id="ef7fb-199">Criar</span><span class="sxs-lookup"><span data-stu-id="ef7fb-199">Create</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="ef7fb-200">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="ef7fb-200">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="ef7fb-201">Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-201">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="ef7fb-202">Atualizar</span><span class="sxs-lookup"><span data-stu-id="ef7fb-202">Update</span></span>](../api/outlookcategory-update.md) | [<span data-ttu-id="ef7fb-203">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="ef7fb-203">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="ef7fb-204">Atualize a propriedade gravável, **color**, do objeto **outlookCategory** especificado.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-204">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="ef7fb-205">Excluir</span><span class="sxs-lookup"><span data-stu-id="ef7fb-205">Delete</span></span>](../api/outlookcategory-delete.md) | <span data-ttu-id="ef7fb-206">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ef7fb-206">None</span></span> |<span data-ttu-id="ef7fb-207">Exclua o objeto **outlookCategory** especificado.</span><span class="sxs-lookup"><span data-stu-id="ef7fb-207">Delete the specified **outlookCategory** object.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/beta/resources/outlookcategory.md:
      Failed to parse any rows out of table with headers: |Pre-set constant|Color mapped to in Outlook|"
  ],
  "tocPath": ""
}-->
 
