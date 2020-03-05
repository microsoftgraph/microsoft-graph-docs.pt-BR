---
title: tipo de recurso groupPolicySettingMapping
description: A configuração da política de grupo para o mapeamento MDM/Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d6d513f16debcec4c636101591e966eef58cd260
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528133"
---
# <a name="grouppolicysettingmapping-resource-type"></a>tipo de recurso groupPolicySettingMapping

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A configuração da política de grupo para o mapeamento MDM/Intune.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicySettingMappings](../api/intune-gpanalyticsservice-grouppolicysettingmapping-list.md)|coleção [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Listar Propriedades e relações dos objetos [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .|
|[Obter groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-get.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Leia as propriedades e as relações do objeto [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .|
|[Criar groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-create.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Criar um novo objeto [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .|
|[Excluir groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-delete.md)|Nenhum|Exclui [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).|
|[Atualizar groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-update.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Atualiza as propriedades de um objeto [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Ainda não documentado|
|parentId|String|ID pai da configuração de política de grupo.|
|childIdList|String collection|Lista de IDs filhos da configuração de política de grupo.|
|settingName|Cadeia de caracteres|O nome dessa configuração de política de grupo.|
|settingValue|String|O valor dessa configuração de política de grupo.|
|settingValueType|String|O tipo de valor dessa configuração de política de grupo.|
|settingDisplayName|String|O nome de exibição dessa configuração de política de grupo.|
|settingDisplayValue|String|O valor de exibição dessa configuração de política de grupo.|
|settingDisplayValueType|String|O tipo de valor de exibição dessa configuração de política de grupo.|
|settingValueDisplayUnits|String|As unidades de exibição desse valor de configuração da política de grupo|
|settingCategory|String|A categoria em que a configuração da política de grupo está.|
|mdmCspName|String|O nome do CSP para o qual esta configuração de política de grupo é mapeada.|
|mdmSettingUri|String|O URI de CSP do MDM para o qual essa configuração de política de grupo é mapeada.|
|mdmMinimumOSVersion|Int32|A versão mínima do sistema operacional para a qual esta configuração MDM oferece suporte.|
|SettingType|[groupPolicySettingType](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|O tipo de configuração (segurança ou ADMX) da política de grupo. Os valores possíveis são: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.|
|isMdmSupported|Boolean|Indica se a configuração é suportada pelo Intune ou não|
|mdmSupportedState|[mdmSupportedState](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|Indica se a configuração é suportada no MDM ou não. Os valores possíveis são: `unknown`, `supported`, `unsupported`, `deprecated`.|
|settingScope|[groupPolicySettingScope](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|O escopo da configuração. Os valores possíveis são: `unknown`, `device`, `user`.|
|intuneSettingUriList|String collection|A lista de URIs de configuração do Intune que esta configuração de política de grupo mapeia para|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicySettingMapping"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "id": "String (identifier)",
  "parentId": "String",
  "childIdList": [
    "String"
  ],
  "settingName": "String",
  "settingValue": "String",
  "settingValueType": "String",
  "settingDisplayName": "String",
  "settingDisplayValue": "String",
  "settingDisplayValueType": "String",
  "settingValueDisplayUnits": "String",
  "settingCategory": "String",
  "mdmCspName": "String",
  "mdmSettingUri": "String",
  "mdmMinimumOSVersion": 1024,
  "settingType": "String",
  "isMdmSupported": true,
  "mdmSupportedState": "String",
  "settingScope": "String",
  "intuneSettingUriList": [
    "String"
  ]
}
```



