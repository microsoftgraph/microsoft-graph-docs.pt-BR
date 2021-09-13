---
author: vishriv
title: Tipo de recurso de grupo
doc_type: resourcePageType
description: Representa um grupo usado em um armazenamento de termos.
ms.localizationpriority: medium
ms.prod: taxonomy
ms.openlocfilehash: 121f195e8054645be47d7a98c5287c52d754b4e7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129751"
---
# <a name="group-resource-type"></a>Tipo de recurso de grupo

Namespace: microsoft.graph.termStore


Representa um grupo usado em um armazenamento de [termos.](../resources/termstore-store.md) Um grupo é uma hierarquia lógica que contém uma coleção de conjuntos sob ele. 

Herda da [entidade](../resources/entity.md).


## <a name="methods"></a>Métodos

| Método                                                   | Tipo de retorno       |    Descrição      |
|:---------------------------------------------------------|:------------------|:---------------------
| [Criar grupo](../api/termstore-group-post.md)                     | [microsoft.graph.termStore.group] | Criar um grupo em um armazenamento de [termos.] |
| [Obter grupo](../api/termstore-group-get.md)                           | [microsoft.graph.termStore.group] | Recupere os dados de um grupo em um armazenamento de [termos.] |
| [Excluir grupo](../api/termstore-group-delete.md)                     | Nenhum |  Excluir um grupo em um armazenamento de [termos.] |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo               | Descrição                        |
|:---------------------|:-------------------|:------------------------------------
| createdDateTime      | DateTimeOffset     | Data e hora da criação do grupo. Somente leitura. |
| description          | string             | Descrição que dá detalhes sobre o uso do termo. |
| id                   | cadeia de caracteres             | Identificador exclusivo do grupo. Somente Leitura. |
| displayName          | cadeia de caracteres             | Nome do grupo. |
| escopo                | string              | Retorna o tipo de grupo. Os valores possíveis são 'global', 'system' e 'siteCollection'. |
| parentSiteId         | cadeia de caracteres             | ID do site pai deste grupo. |

## <a name="relationships"></a>Relações
| Relação       | Tipo                        | Descrição              |
|:-------------------|:----------------------------|:--------------------------
| sets           | [coleção microsoft.graph.termStore.set][] | Todos os conjuntos sob o grupo em um armazenamento de [termos]. |

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON de um **recurso de** grupo.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.group",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
```json
{
  "@odata.type": "#microsoft.graph.termStore.group",
  "id": "string",
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "scope" : "microsoft.graph.termStore.groupScope",
  "displayName": "string",
  "parentSiteId" : "string"
}
```



[identitySet]: identitySet.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.store]: termstore-store.md
[store]: ../resources/termstore-store.md
[group]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
<!--
{
  "type": "#page.annotation",
  "description": "TermGroup is the entity used for managing permissions for the termSets in termStore",
  "keywords": "termGroup,facet,resource",
  "section": "documentation",
  "tocPath": "TermGroup",
  "tocBookmarks": {
    "Resources/termStore.group&quot;: &quot;#"
  },
  "suppressions": []
}
-->


