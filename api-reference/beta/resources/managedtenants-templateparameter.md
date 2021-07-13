---
title: Tipo de recurso templateParameter
description: Representa um parâmetro usado em um modelo de gerenciamento.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 4f533bc375e2d7e4a1e4ef2f7f801f248c1801c4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402139"
---
# <a name="templateparameter-resource-type"></a>Tipo de recurso templateParameter

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um parâmetro usado em um modelo de gerenciamento.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|A descrição do parâmetro template. Opcional. Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição do parâmetro template. Obrigatório. Somente leitura.|
|jsonAllowedValues|Cadeia de caracteres|Os valores permitidos para o parâmetro template representados por uma cadeia de caracteres serializada de JSON. Opcional. Somente leitura.|
|jsonDefaultValue|Cadeia de caracteres|O valor padrão para o parâmetro template representado por uma cadeia de caracteres serializada de JSON. Obrigatório. Somente leitura.|
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
