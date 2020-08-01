---
title: definir tipo de recurso
description: Representa um conjunto em um repositório de termos.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 5e74e0a603d088c7964b13fad51018171642c6ec
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539129"
---
# <a name="set-resource-type"></a>definir tipo de recurso

Namespace: Microsoft. Graph. termos

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o conjunto usado em um [repositório]de termos. O conjunto representa uma unidade que contém uma coleção de termos hierárquicos. Um [grupo] pode conter vários conjuntos.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar conjuntos](../api/termstore-group-list-sets.md)|coleção [Microsoft. Graph. termos. Set] | Retorna uma lista de conjuntos contidos em um [grupo] de um [repositório] de termos |
|[Criar conjunto](../api/termstore-set-post.md)|[Microsoft. Graph. termos. Set](../resources/termstore-set.md)|Criar um novo objeto Set em um [repositório]de termos.|
|[Criar termo](../api/termstore-term-post.md)|[Microsoft. Graph. termos. Term](../resources/termstore-term.md)|Criar um novo objeto [Term] em um [repositório]de termos.|
|[Obter conjunto](../api/termstore-set-get.md)|[Microsoft. Graph. termos. Set](../resources/termstore-set.md)| Obter um objeto Set em um [repositório]de termos.|
|[Obter termo](../api/termstore-term-get.md)|[Microsoft. Graph. termos. Term](../resources/termstore-term.md)| Obter um objeto [Term] em um [repositório]de termos.|
|[Conjunto de atualização](../api/termstore-set-update.md)|[Microsoft. Graph. termos. Set](../resources/termstore-set.md)|Atualizar as propriedades de um objeto Set em um [repositório]de termos.|
|[Excluir conjunto](../api/termstore-set-delete.md)|Nenhum|Exclui um objeto Set em um [repositório]de termos.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Data e hora da criação do conjunto. Somente leitura.|
|description|String|Descrição que oferece detalhes sobre o uso de termos.|
|id|Cadeia de caracteres|Identificador exclusivo. Somente leitura.|
|localizadores|coleção [Microsoft. Graph. termos.](../resources/termstore-localizedname.md) undeleble|Nome do conjunto para cada languageTag.|
|properties|coleção [Microsoft. Graph. KeyValue](../resources/keyvalue.md)|Propriedades personalizadas para o conjunto.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|filhos|coleção [Microsoft. Graph. termos. Term](../resources/termstore-term.md)|Termos filhos de Set no [repositório]de termos.|
|parentGroup|[Microsoft. Graph. termos. Group](../resources/termstore-group.md)|O [grupo] pai que contém o conjunto.|
|Relations|coleção [Microsoft. Graph. termos. relation](../resources/termstore-relation.md)|Indica quais termos foram afixados ou reutilizados diretamente sob o conjunto.|
|termos|coleção [Microsoft. Graph. termos. Term](../resources/termstore-term.md)|Todos os termos do conjunto.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.set",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.set",
  "id": "String (identifier)",
  "localizedNames": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedName"
    }
  ],
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "properties": [
    {
      "@odata.type": "microsoft.graph.termStore.keyValue"
    }
  ]
}
```

[microsoft.graph.termStore.term]: termstore-term.md
[Microsoft. Graph. termos. Set]: termstore-set.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.relation]: termstore-relation.md
[microsoft.graph.termStore.store]: termstore-store.md
[microsoft.graph.termStore.localizedName]: termstore-localizedname.md
[Guarde]: ../resources/termstore-store.md
[group]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
[terminal]: ../resources/termstore-term.md


<!--
{
  "type": "#page.annotation",
  "description": "TermSet is the entity containing the particular taxonomy for a tenant",
  "keywords": "termSet,facet,resource",
  "section": "documentation",
  "tocPath": "TermSet",
  "tocBookmarks": {
    "Resources/termStore.set": "#"
  },
  "suppressions": []
}
-->
