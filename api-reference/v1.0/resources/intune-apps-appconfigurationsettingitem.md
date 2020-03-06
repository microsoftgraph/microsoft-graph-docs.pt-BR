---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cb207355a6f637cc1f5c0e3031422f639e2bf357
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531247"
---
# <a name="appconfigurationsettingitem-resource-type"></a>Tipo de recurso appConfigurationSettingItem

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades do item de configuração de Configuração do aplicativo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appConfigKey|String|chave de configuração do aplicativo.|
|appConfigKeyType|[mdmAppConfigKeyType](../resources/intune-apps-mdmappconfigkeytype.md)|tipo de chave de configuração de aplicativo. Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.|
|appConfigKeyValue|Cadeia de caracteres|valor de chave de configuração de aplicativo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```




