---
title: Tipo de recurso androidForWorkAppConfigurationSchemaItem
description: Item de configuração único dentro de um esquema de configurações personalizadas de um aplicativo do Android for Work.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 086da317eedc908ea44a7ec0d1b9140bbe0534b4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552753"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a>Tipo de recurso androidForWorkAppConfigurationSchemaItem

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Item de configuração único dentro de um esquema de configurações personalizadas de um aplicativo do Android for Work.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|schemaItemKey|String|Chave exclusiva que o aplicativo usa para identificar o item|
|displayName|String|Nome legível por humanos|
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





