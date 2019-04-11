---
title: tipo de recurso androidManagedStoreAppConfigurationSchemaItem
description: Único item de configuração no esquema de configuração personalizada de um aplicativo Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 964916f9f6a46cd8b276e304bfb341d6504db0d2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785815"
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
Nenhuma

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





