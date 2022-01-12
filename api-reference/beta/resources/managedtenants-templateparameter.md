---
title: Tipo de recurso templateParameter
description: Representa um parâmetro usado em um modelo de gerenciamento.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: a2fe8cc543f60e2e862af65b9e47f6a84389e453
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791864"
---
# <a name="templateparameter-resource-type"></a>Tipo de recurso templateParameter

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um parâmetro usado em um modelo de gerenciamento.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|A descrição do parâmetro template. Opcional. Somente leitura.|
|displayName|String|O nome de exibição do parâmetro template. Obrigatório. Somente leitura.|
|jsonAllowedValues|String|Os valores permitidos para o parâmetro template representados por uma cadeia de caracteres serializada de JSON. Opcional. Somente leitura.|
|jsonDefaultValue|String|O valor padrão para o parâmetro template representado por uma cadeia de caracteres serializada de JSON. Obrigatório. Somente leitura.|
|valueType|managementParameterValueType|O tipo de dados do parâmetro template.. Os valores possíveis são: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`. Obrigatório. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.templateParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.templateParameter",
  "displayName": "String",
  "description": "String",
  "valueType": "String",
  "jsonDefaultValue": "String",
  "jsonAllowedValues": "String"
}
```
