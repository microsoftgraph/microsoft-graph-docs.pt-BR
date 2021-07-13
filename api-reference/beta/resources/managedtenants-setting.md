---
title: tipo de recurso de configuração
description: Representa uma configuração usada em uma linha de base.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 2545dc6aa11668359fa9dda636412d36f8d92de1
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402141"
---
# <a name="setting-resource-type"></a>tipo de recurso de configuração

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma configuração usada em uma linha de base.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição da configuração. Obrigatório. Somente leitura.|
|jsonValue|Cadeia de caracteres|O valor da configuração serializada como cadeia de caracteres de JSON. Obrigatório. Somente leitura.|
|overwriteAllowed|Boolean|Um sinalizador indicando se a configuração pode substituir as configurações existentes quando aplicada. Obrigatório. Somente leitura.|
|valueType|managementParameterValueType|O tipo de dados da configuração. Os valores possíveis são: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`. Obrigatório. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.setting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.setting",
  "displayName": "String",
  "overwriteAllowed": "Boolean",
  "valueType": "String",
  "jsonValue": "String"
}
```
