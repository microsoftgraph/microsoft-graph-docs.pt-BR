---
title: Tipo de recurso appConfigurationSettingItem
description: Contém propriedades do item de configuração de Configuração do aplicativo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0c001e19758865e957cb3d72f3d49acf3387281a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006049"
---
# <a name="appconfigurationsettingitem-resource-type"></a>Tipo de recurso appConfigurationSettingItem

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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





