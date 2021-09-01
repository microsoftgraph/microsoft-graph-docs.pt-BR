---
title: Tipo de recurso assignmentFilterSupportedProperty
description: Representa as informações sobre a propriedade que é suportada na criação da regra de AssignmentFilter.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b8b8a5bc422c2d663d74ea7dc93b7353f10e65d3
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786604"
---
# <a name="assignmentfiltersupportedproperty-resource-type"></a>Tipo de recurso assignmentFilterSupportedProperty

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa as informações sobre a propriedade que é suportada na criação da regra de AssignmentFilter.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|dataType|Cadeia de caracteres|O tipo de dados da propriedade.|
|isCollection|Boleano|Indica se a propriedade é um tipo de coleção ou não.|
|nome|Cadeia de caracteres|Nome da propriedade.|
|propertyRegexConstraint|Cadeia de caracteres|Cadeia de caracteres Regex para fazer validação no valor da propriedade.|
|supportedOperators|[coleção assignmentFilterOperator](../resources/intune-policyset-assignmentfilteroperator.md)|Lista de todos os operadores com suporte nesta propriedade.|
|supportedValues|Coleção de cadeias de caracteres|Lista de todos os valores com suporte para essa adequada, vazia se tudo for suportado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterSupportedProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterSupportedProperty",
  "dataType": "String",
  "isCollection": true,
  "name": "String",
  "propertyRegexConstraint": "String",
  "supportedOperators": [
    "String"
  ],
  "supportedValues": [
    "String"
  ]
}
```



