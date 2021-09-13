---
title: Tipo de recurso groupPolicySettingMapping
description: A configuração de Política de Grupo como mapeamento MDM/Intune.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 90cacd1f89b75f1c6cf60fe64e9c9c141664423f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063899"
---
# <a name="grouppolicysettingmapping-resource-type"></a>Tipo de recurso groupPolicySettingMapping

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A configuração de Política de Grupo como mapeamento MDM/Intune.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicySettingMappings](../api/intune-gpanalyticsservice-grouppolicysettingmapping-list.md)|[coleção groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Listar propriedades e relações dos [objetos groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|
|[Obter groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-get.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Leia propriedades e relações do [objeto groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|
|[Criar groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-create.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Crie um novo [objeto groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|
|[Excluir groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-delete.md)|Nenhum|Exclui um [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).|
|[Atualizar groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-update.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Atualize as propriedades de [um objeto groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Ainda não documentado|
|parentId|Cadeia de Caracteres|ID pai da configuração de política de grupo.|
|childIdList|Conjunto de cadeias de caracteres|Lista de IDs Filho da configuração de política de grupo.|
|settingName|Cadeia de caracteres|O nome dessa configuração de política de grupo.|
|settingValue|Cadeia de Caracteres|O valor dessa configuração de política de grupo.|
|settingValueType|Cadeia de caracteres|O tipo de valor dessa configuração de política de grupo.|
|settingDisplayName|String|O nome de exibição dessa configuração de política de grupo.|
|settingDisplayValue|Cadeia de caracteres|O valor de exibição dessa configuração de política de grupo.|
|settingDisplayValueType|Cadeia de caracteres|O tipo de valor de exibição dessa configuração de política de grupo.|
|settingValueDisplayUnits|Cadeia de caracteres|As unidades de exibição desse valor de configuração de política de grupo|
|settingCategory|Cadeia de Caracteres|A categoria em que a configuração da política de grupo está.|
|mdmCspName|Cadeia de Caracteres|O nome CSP para o que a configuração da política de grupo mapeia.|
|mdmSettingUri|String|O URI CSP do MDM para o que a política de grupo mapeia.|
|mdmMinimumOSVersion|Int32|A versão mínima do sistema operacional compatível com essa configuração mdm.|
|settingType|[groupPolicySettingType](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|O tipo de configuração (segurança ou admx) da Política de Grupo. Os valores possíveis são: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.|
|isMdmSupported|Booliano|Indica se a configuração é suportada pelo Intune ou não|
|mdmSupportedState|[mdmSupportedState](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|Indica se a configuração é suportada no Mdm ou não. Os valores possíveis são: `unknown`, `supported`, `unsupported`, `deprecated`.|
|settingScope|[groupPolicySettingScope](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|O escopo da configuração. Os valores possíveis são: `unknown`, `device`, `user`.|
|intuneSettingUriList|Conjunto de cadeias de caracteres|A lista de URIs de configuração do Intune para as configurações de política de grupo mapeia para|
|intuneSettingDefinitionId|Cadeia de caracteres|A ID de Definição de Configuração do Intune|
|admxSettingDefinitionId|Cadeia de caracteres|ID da Política de Grupo Admx|

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
  ],
  "intuneSettingDefinitionId": "String",
  "admxSettingDefinitionId": "String"
}
```



