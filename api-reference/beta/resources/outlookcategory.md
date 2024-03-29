---
title: Tipo de recurso outlookCategory
description: Representa uma categoria pela qual um usuário pode agrupar itens do Outlook como mensagens e eventos. No Outlook, o usuário define categorias em uma lista mestra e pode aplicar uma ou mais dessas definidas pelo usuário
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f88c5df573e52e852311f71eb08781cd8061d503
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820921"
---
# <a name="outlookcategory-resource-type"></a>Tipo de recurso outlookCategory

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

Representa uma categoria pela qual um usuário pode agrupar itens do Outlook como mensagens e eventos. No Outlook, o usuário define categorias em uma lista mestra e pode aplicar uma ou mais dessas categorias definidas pelo usuário a um item. 

Usando a API REST, é possível [criar](../api/outlookuser-post-mastercategories.md) e definir categorias na lista mestra de categorias para um usuário. Também é possível [acessar essa lista mestra de categorias](../api/outlookuser-list-mastercategories.md), [obter uma categoria específica](../api/outlookcategory-get.md), [atualizar](../api/outlookcategory-update.md) a cor associada a uma categoria ou [excluir](../api/outlookcategory-delete.md) uma categoria. É possível aplicar uma categoria a um item atribuindo a propriedade **displayName** da categoria à coleção **categories** do item.
Os recursos que podem ser atribuídos a categorias incluem [contato](contact.md)[,](message.md) [evento](event.md), mensagem, [outlookTask](outlooktask.md), [post](post.md) e [todoTask](todotask.md).   

Cada categoria é atribuída por duas propriedades: **displayName** e **color**. O valor **displayName** deve ser exclusivo na lista mestra de um usuário. No entanto, o valor **color** não precisa ser exclusivo. Várias categorias na lista mestra podem ser mapeadas para a mesma cor. É possível mapear até 25 cores diferentes para as categorias na lista mestra a um usuário.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres|Um nome exclusivo que identifica uma categoria na caixa de correio do usuário. Após a criação de uma categoria, o nome não poderá ser alterado. Somente leitura.|
|color|String|Uma constante de cor predefinida que caracteriza uma categoria e que é mapeada para uma das 25 cores predefinidas. Confira a observação abaixo. |

> **Observação** Os valores possíveis para **color** são constantes predefinidas como `None`, `preset0` e `preset1`. Cada constante predefinida é mapeada para uma cor. A cor real depende do cliente do Outlook em que as categorias estão sendo exibidas. A tabela a seguir mostra as cores mapeadas para cada constante predefinida do Outlook (cliente da área de trabalho). 


| Constante predefinida  | Cor mapeada para no Outlook |
|:---------------|:--------|
| Nenhum | Nenhuma cor mapeada |
| Preset0 | Vermelho |
| Preset1 | Laranja |
| Preset2 | Marrom |
| Preset3 | Amarelo |
| Preset4 | Verde |
| Preset5 | Azul-petróleo |
| Preset6 | Verde-oliva |
| Preset7 | Azul |
| Preset8 | Roxo |
| Preset9 | Cranberry |
| Preset10 | Steel |
| Preset11 | DarkSteel |
| Preset12 | Cinza |
| Preset13 | DarkGray |
| Preset14 | Preto |
| Preset15 | DarkRed |
| Preset16 | DarkOrange |
| Preset17 | DarkBrown |
| Preset18 | DarkYellow |
| Preset19 | DarkGreen |
| Preset20 | DarkTeal |
| Preset21 | DarkOlive |
| Preset22 | DarkBlue |
| Preset23 | DarkPurple |
| Preset24 | DarkCranberry |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

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

## <a name="methods"></a>Métodos
| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar categorias](../api/outlookuser-list-mastercategories.md) | Coleção [outlookCategory](../resources/outlookcategory.md) |Obtém todas as categorias que foram definidas para o usuário.|
|[Obter categoria](../api/outlookcategory-get.md) | [outlookCategory](../resources/outlookcategory.md) |Obtenha as propriedades e as relações do objeto **outlookCategory** especificado.|
|[Criar](../api/outlookuser-post-mastercategories.md) | [outlookCategory](../resources/outlookcategory.md) |Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.|
|[Atualizar](../api/outlookcategory-update.md) | [outlookCategory](../resources/outlookcategory.md) |Atualize a propriedade gravável, **color**, do objeto **outlookCategory** especificado. |
|[Delete](../api/outlookcategory-delete.md) | Nenhum |Exclua o objeto **outlookCategory** especificado. |


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
  ]
}
-->
 


