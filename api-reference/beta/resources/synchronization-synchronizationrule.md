---
title: tipo de recurso de synchronizationRule
description: Define como a sincronização deve ser executada para o mecanismo de sincronização, incluindo quais objetos para sincronizar e na direção, como objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos deve ser transformados quando elas estiver sincronizadas da origem para o diretório de destino.
ms.openlocfilehash: c860228637a6cc3ad9137851408379bd7f779c75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035076"
---
# <a name="synchronizationrule-resource-type"></a>tipo de recurso de synchronizationRule

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Define como a sincronização deve ser executada para o mecanismo de sincronização, incluindo quais objetos para sincronizar e na direção, como objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos deve ser transformados quando elas estiver sincronizadas da origem para o diretório de destino.

>**Observação:** Regras de sincronização definem sincronização em uma direção - do diretório de origem para o diretório de destino. Os diretórios de origem e destino são definidos como parte das propriedades de regra.

Regras de sincronização são atualizadas como parte do [esquema de sincronização](synchronization-synchronizationschema.md).

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição    |
|:--------------|:----------|:---------------|
|editável       |Booliano    |`true`Se a regra de sincronização pode ser personalizada; `false` se esta regra é somente leitura e não deve ser alterada.|
|id             |String     |Identificador da regra de sincronização. Deve ser um dos identificadores reconhecidos pelo mecanismo de sincronização. Suporte para a regra identificadores podem ser encontrados no modelo de sincronização retornado pela API.|
|metadados       |coleção [stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) |Propriedades adicionais de extensão. A menos que seja instruído explicitamente pela equipe de suporte, valores de metadados não devem ser alterados.|
|name           |String     |Legíveis nome da regra de sincronização. Não anulável.|
|objectMappings |coleção [objectMapping](synchronization-objectmapping.md)    |Conjunto de mapeamentos de objeto suportado pela regra. Instrui o mecanismo de sincronização quais objetos devem ser sincronizados.|
|prioridade       |Inteiro    |Prioridade em relação a outras regras no [synchronizationSchema](synchronization-synchronizationschema.md). As regras com o número de prioridade mais baixa serão processadas pela primeira vez.|
|sourceDirectoryName       |String    |Nome do diretório de origem. Deve corresponder a uma das definições de diretório no [synchronizationSchema](synchronization-synchronizationschema.md).|
|targetDirectoryName       |String    |Nome do diretório de destino. Deve corresponder a uma das definições de diretório no [synchronizationSchema](synchronization-synchronizationschema.md).|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationRule"
}-->

```json
{
  "editable": true,
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objectMappings": [{"@odata.type": "microsoft.graph.objectMapping"}],
  "priority": 1024,
  "sourceDirectoryName": "String",
  "targetDirectoryName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->