---
title: tipo de recurso androidManagedStoreAppConfigurationSchemaItem
description: Único item de configuração no esquema de configuração personalizada de um aplicativo Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3012542315cd30a565da315a9d383757557b1008
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950540"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a>tipo de recurso androidManagedStoreAppConfigurationSchemaItem

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Único item de configuração no esquema de configuração personalizada de um aplicativo Android.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|schemaItemKey|Cadeia de caracteres|Chave exclusiva que o aplicativo usa para identificar o item|
|displayName|String|Nome legível por humanos|
|description|String|Descrição do que o item controla dentro do aplicativo|
|defaultBoolValue|Booliano|Valor padrão para itens do tipo booliano, se especificado pelo desenvolvedor do aplicativo|
|defaultIntValue|Int32|Valor padrão para itens do tipo inteiro, se especificado pelo desenvolvedor do aplicativo|
|defaultStringValue|Cadeia de caracteres|Valor padrão para itens do tipo cadeia de caracteres, se especificado pelo desenvolvedor do aplicativo|
|defaultStringArrayValue|Coleção String|Valor padrão para itens do tipo matriz, se especificado pelo desenvolvedor do aplicativo|
|dataType|[androidManagedStoreAppConfigurationSchemaItemDataType](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|O tipo de valor que este item descreve. Os valores possíveis são: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.|
|selections|Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Lista de pares nome/valor legíveis por humanos dos valores válidos que podem ser definidos para esse item (somente itens de Escolha e Múltipla escolha)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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




