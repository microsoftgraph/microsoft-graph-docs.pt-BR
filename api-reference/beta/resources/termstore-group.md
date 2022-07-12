---
author: mohitpcad
title: Tipo de recurso de grupo
doc_type: resourcePageType
description: Representa um grupo usado em um repositório de termos.
ms.localizationpriority: medium
ms.prod: taxonomy
ms.openlocfilehash: 3bd7f818cf9e38dcffcba9fac0c93b248d1d10d9
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732678"
---
# <a name="group-resource-type"></a>Tipo de recurso de grupo

Namespace: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Representa um grupo usado em um repositório de [termos](../resources/termstore-store.md). Um grupo é uma hierarquia lógica que contém uma coleção de conjuntos sob ele. 

Herda de [entidade](../resources/entity.md).


## <a name="methods"></a>Methods

| Método                                                   | Tipo de retorno       |    Descrição|
|:---------------------------------------------------------|:------------------|:---------------------|
| [Criar grupo](../api/termstore-group-post.md)                     | [microsoft.graph.termStore.group] | Crie um grupo em um repositório de [termos].|
| [Obter grupo](../api/termstore-group-get.md)                           | [microsoft.graph.termStore.group] | Recupere os dados de um grupo em um repositório de [termos].|
| [Excluir grupo](../api/termstore-group-delete.md)                     | Nenhum |  Excluir um grupo em um repositório de [termos].|

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo               | Descrição|
|:---------------------|:-------------------|:------------------------------------|
| createdDateTime      | DateTimeOffset     | Data e hora da criação do grupo. Somente leitura.|
| description          | string             | Descrição que fornece detalhes sobre o uso do termo.|
| id                   | string             | Identificador exclusivo do grupo. Somente Leitura.|
| displayName          | string             | Nome do grupo.|
| escopo                | string              | Retorna o tipo do grupo. Os valores possíveis são: `global`, `system` e `siteCollection`.|
| parentSiteId         | string             | ID do site pai deste grupo.|

## <a name="relationships"></a>Relações
| Relação       | Tipo                        | Descrição|
|:-------------------|:----------------------------|:--------------------------|
| Define           | [coleção microsoft.graph.termStore.set][] | Todos os conjuntos no grupo em um repositório de [termos].|

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
[Loja]: ../resources/termstore-store.md
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


