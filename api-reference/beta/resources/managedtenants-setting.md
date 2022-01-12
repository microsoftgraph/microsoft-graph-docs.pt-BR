---
title: tipo de recurso de configuração
description: Representa uma configuração usada em uma linha de base.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 53eaf2dd4c3e97e183083f1a6c0d127ffbaefafd
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861291"
---
# <a name="setting-resource-type"></a>tipo de recurso de configuração

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma configuração usada em uma linha de base.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição da configuração. Obrigatório. Somente leitura.|
|jsonValue|String|O valor da configuração serializada como cadeia de caracteres de JSON. Obrigatório. Somente leitura.|
|overwriteAllowed|Booliano|Um sinalizador indicando se a configuração pode substituir as configurações existentes quando aplicada. Obrigatório. Somente leitura.|
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
