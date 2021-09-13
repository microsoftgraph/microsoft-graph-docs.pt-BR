---
title: Tipo de recurso assignmentFilterSupportedProperty
description: Representa as informações sobre a propriedade que é suportada na criação da regra de AssignmentFilter.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 339f220b9508487735e2473133e61c2682263c05
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074945"
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
|propertyRegexConstraint|Cadeia de Caracteres|Cadeia de caracteres Regex para fazer validação no valor da propriedade.|
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



