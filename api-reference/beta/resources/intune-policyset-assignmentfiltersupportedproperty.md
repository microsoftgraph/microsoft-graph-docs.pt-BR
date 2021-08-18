---
title: Tipo de recurso assignmentFilterSupportedProperty
description: Representa as informações sobre a propriedade que é suportada na criação da regra de AssignmentFilter.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed8ec505d314207a57fe3b743357e4217255db0d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265454"
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
|isCollection|Boolean|Indica se a propriedade é um tipo de coleção ou não.|
|nome|Cadeia de caracteres|Nome da propriedade.|
|propertyRegexConstraint|Cadeia de caracteres|Cadeia de caracteres Regex para fazer validação no valor da propriedade.|
|supportedOperators|[coleção assignmentFilterOperator](../resources/intune-policyset-assignmentfilteroperator.md)|Lista de todos os operadores com suporte nesta propriedade.|
|supportedValues|String collection|Lista de todos os valores com suporte para essa adequada, vazia se tudo for suportado.|

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




