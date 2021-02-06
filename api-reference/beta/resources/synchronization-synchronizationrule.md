---
title: Tipo de recurso synchronizationRule
description: Define como a sincronização deve ser realizada para o mecanismo de sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 94697fede9ab9055b1a477cfd94edea88f207331
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135993"
---
# <a name="synchronizationrule-resource-type"></a>Tipo de recurso synchronizationRule

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define como a sincronização deve ser realizada para o mecanismo de sincronização, incluindo quais objetos sincronizar e em qual direção, como os objetos do diretório de origem devem ser corresponder aos objetos no diretório de destino e como os atributos devem ser transformados quando são sincronizados da origem para o diretório de destino.

>**Observação:** As regras de sincronização definem a sincronização em uma direção- do diretório de origem para o diretório de destino. Os diretórios de origem e destino são definidos como parte das propriedades da regra.

As regras de sincronização são atualizadas como parte do esquema [de sincronização.](synchronization-synchronizationschema.md)

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição    |
|:--------------|:----------|:---------------|
|editável       |Boolean    |`true` se a regra de sincronização puder ser personalizada; `false` se essa regra for somente leitura e não deve ser alterada.|
|id             |String     |Identificador de regra de sincronização. Deve ser um dos identificadores reconhecidos pelo mecanismo de sincronização. Identificadores de regra suportados podem ser encontrados no modelo de sincronização retornado pela API.|
|metadados       |[Coleção stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) |Propriedades de extensão adicionais. A menos que seja explicitamente instruído pela equipe de suporte, os valores de metadados não devem ser alterados.|
|nome           |String     |Nome acessível para humanos da regra de sincronização. Não anulável.|
|objectMappings |[coleção objectMapping](synchronization-objectmapping.md)    |Conjunto de mapeamentos de objetos suportados pela regra. Informa ao mecanismo de sincronização quais objetos devem ser sincronizados.|
|prioridade       |Inteiro    |Prioridade relativa a outras regras no [synchronizationSchema](synchronization-synchronizationschema.md). As regras com o número de prioridade mais baixa serão processadas primeiro.|
|sourceDirectoryName       |String    |Nome do diretório de origem. Deve corresponder a uma das definições de diretório em [synchronizationSchema](synchronization-synchronizationschema.md).|
|targetDirectoryName       |String    |Nome do diretório de destino. Deve corresponder a uma das definições de diretório em [synchronizationSchema](synchronization-synchronizationschema.md).|

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


