---
title: Tipo de recurso androidForWorkAppConfigurationSchemaItem
description: Item de configuração único dentro de um esquema de configurações personalizadas de um aplicativo do Android for Work.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 7e8500df3065c68ae8ddc2ad85413aa4d31f8980
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923450"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a>Tipo de recurso androidForWorkAppConfigurationSchemaItem

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Item de configuração único dentro de um esquema de configurações personalizadas de um aplicativo do Android for Work.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|schemaItemKey|Cadeia de caracteres|Chave exclusiva que o aplicativo usa para identificar o item|
|displayName|Cadeia de caracteres|Nome legível por humanos|
|description|Cadeia de caracteres|Descrição do que o item controla dentro do aplicativo|
|defaultBoolValue|Booliano|Valor padrão para itens do tipo booliano, se especificado pelo desenvolvedor do aplicativo|
|defaultIntValue|Int32|Valor padrão para itens do tipo inteiro, se especificado pelo desenvolvedor do aplicativo|
|defaultStringValue|Cadeia de caracteres|Valor padrão para itens do tipo cadeia de caracteres, se especificado pelo desenvolvedor do aplicativo|
|defaultStringArrayValue|Coleção String|Valor padrão para itens do tipo matriz, se especificado pelo desenvolvedor do aplicativo|
|dataType|[androidForWorkAppConfigurationSchemaItemDataType](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|O tipo de valor que descreve este item. Os valores possíveis são: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.|
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





