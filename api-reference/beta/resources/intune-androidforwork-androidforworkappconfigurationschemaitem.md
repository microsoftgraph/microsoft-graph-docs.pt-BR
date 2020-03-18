---
title: Tipo de recurso androidForWorkAppConfigurationSchemaItem
description: Item de configuração único dentro de um esquema de configurações personalizadas de um aplicativo do Android for Work.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1e64edefe6da8b0c09b0eb90a6c772f34d908cf5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799414"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a>Tipo de recurso androidForWorkAppConfigurationSchemaItem

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Item de configuração único dentro de um esquema de configurações personalizadas de um aplicativo do Android for Work.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|schemaItemKey|String|Chave exclusiva que o aplicativo usa para identificar o item|
|displayName|Cadeia de caracteres|Nome legível por humanos|
|description|String|Descrição do que o item controla dentro do aplicativo|
|defaultBoolValue|Booliano|Valor padrão para itens do tipo booliano, se especificado pelo desenvolvedor do aplicativo|
|defaultIntValue|Int32|Valor padrão para itens do tipo inteiro, se especificado pelo desenvolvedor do aplicativo|
|defaultStringValue|Cadeia de caracteres|Valor padrão para itens do tipo cadeia de caracteres, se especificado pelo desenvolvedor do aplicativo|
|defaultStringArrayValue|Coleção String|Valor padrão para itens do tipo matriz, se especificado pelo desenvolvedor do aplicativo|
|dataType|[androidForWorkAppConfigurationSchemaItemDataType](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|O tipo de valor que este item descreve. Os valores possíveis são: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.|
|selections|Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Lista de pares nome/valor legíveis por humanos dos valores válidos que podem ser definidos para esse item (somente itens de Escolha e Múltipla escolha)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchemaItem",
  "schemaItemKey": "String",
  "displayName": "String",
  "description": "String",
  "defaultBoolValue": true,
  "defaultIntValue": 1024,
  "defaultStringValue": "String",
  "defaultStringArrayValue": [
    "String"
  ],
  "dataType": "String",
  "selections": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



