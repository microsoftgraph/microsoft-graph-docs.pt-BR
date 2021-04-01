---
author: mohitpcad
title: Tipo de recurso de grupo
doc_type: resourcePageType
description: Representa um grupo usado em um armazenamento de termos.
localization_priority: Normal
ms.prod: Sharepoint
ms.openlocfilehash: 1249f94b96e0c6ff7251a2a97f4885a21258aaeb
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473462"
---
# <a name="group-resource-type"></a>Tipo de recurso de grupo

Namespace: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Representa um grupo usado em um armazenamento de [termos.](../resources/termstore-store.md) Um grupo é uma hierarquia lógica que contém uma coleção de conjuntos sob ele. 

Herda da [entidade](../resources/entity.md).


## <a name="methods"></a>Métodos

| Método                                                   | Tipo de retorno       |    Descrição
|:---------------------------------------------------------|:------------------|:---------------------
| [Criar grupo](../api/termstore-group-post.md)                     | [microsoft.graph.termStore.group] | Criar um grupo em um armazenamento de [termos.]
| [Obter grupo](../api/termstore-store-get-group.md)                           | [microsoft.graph.termStore.group] | Recupere os dados de um grupo em um armazenamento de [termos.]
| [Excluir grupo](../api/termstore-group-delete.md)                     | Nenhum |  Excluir um grupo em um armazenamento de [termos.]

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo               | Descrição
|:---------------------|:-------------------|:------------------------------------
| createdDateTime      | DateTimeOffset     | Data e hora da criação do grupo. Somente leitura.
| description          | string             | Descrição que dá detalhes sobre o uso do termo.
| id                   | cadeia de caracteres             | Identificador exclusivo do grupo. Somente Leitura.
| displayName          | cadeia de caracteres             | Nome do grupo.
| escopo                | string              | Retorna o tipo de grupo. Os valores possíveis são 'global', 'system' e 'siteCollection'.
| parentSiteId         | cadeia de caracteres             | ID do site pai deste grupo.

## <a name="relationships"></a>Relações
| Relação       | Tipo                        | Descrição
|:-------------------|:----------------------------|:--------------------------
| sets           | [coleção microsoft.graph.termStore.set][] | Todos os conjuntos sob o grupo em um armazenamento de [termos].

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
    "Resources/termStore.group": "#"
  },
  "suppressions": []
}
-->


