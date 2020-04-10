---
title: tipo de recurso synchronizationRule
description: Define como a sincronização deve ser executada para o mecanismo de sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0698afb7e3584aa1d4cd6697504138f6262e5141
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217364"
---
# <a name="synchronizationrule-resource-type"></a>tipo de recurso synchronizationRule

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define como a sincronização deve ser executada para o mecanismo de sincronização, incluindo quais objetos sincronizar e em que direção, como os objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos devem ser transformados quando forem sincronizados da origem para o diretório de destino.

>**Observação:** As regras de sincronização definem a sincronização em uma direção – do diretório de origem para o diretório de destino. Os diretórios de origem e de destino são definidos como parte das propriedades da regra.

As regras de sincronização são atualizadas como parte do [esquema de sincronização](synchronization-synchronizationschema.md).

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição    |
|:--------------|:----------|:---------------|
|edita       |Boolean    |`true`se a regra de sincronização puder ser personalizada; `false` se essa regra é somente leitura e não deve ser alterada.|
|id             |String     |Identificador de regra de sincronização. Deve ser um dos identificadores reconhecidos pelo mecanismo de sincronização. Os identificadores de regra suportados podem ser encontrados no modelo de sincronização retornado pela API.|
|los       |coleção [stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) |Propriedades de extensão adicionais. A menos que instruído explicitamente pela equipe de suporte, os valores de metadados não devem ser alterados.|
|nome           |String     |Nome legível da regra de sincronização. Não anulável.|
|objectmappings |coleção [Objectmapping](synchronization-objectmapping.md)    |Conjunto de mapeamentos de objeto com suporte da regra. Informa ao mecanismo de sincronização quais objetos devem ser sincronizados.|
|prioridade       |Inteiro    |Prioridade relativa a outras regras no [synchronizationSchema](synchronization-synchronizationschema.md). As regras com o número de prioridade mais baixa serão processadas primeiro.|
|sourceDirectoryName       |Cadeia de Caracteres    |Nome do diretório de origem. Deve corresponder a uma das definições de diretório no [synchronizationSchema](synchronization-synchronizationschema.md).|
|targetDirectoryName       |Cadeia de Caracteres    |Nome do diretório de destino. Deve corresponder a uma das definições de diretório no [synchronizationSchema](synchronization-synchronizationschema.md).|

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
