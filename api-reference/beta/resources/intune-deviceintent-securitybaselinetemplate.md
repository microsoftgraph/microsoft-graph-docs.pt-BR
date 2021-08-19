---
title: Tipo de recurso securityBaselineTemplate
description: O modelo de linha de base de segurança da conta
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 906f351dc79e0f624e2baf26138ad559418005f2
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58263811"
---
# <a name="securitybaselinetemplate-resource-type"></a>Tipo de recurso securityBaselineTemplate

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O modelo de linha de base de segurança da conta


Herda de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar securityBaselineTemplates](../api/intune-deviceintent-securitybaselinetemplate-list.md)|[Coleção securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|Listar propriedades e relações dos objetos [securityBaselineTemplate.](../resources/intune-deviceintent-securitybaselinetemplate.md)|
|[Obter securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-get.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|Leia propriedades e relações do [objeto securityBaselineTemplate.](../resources/intune-deviceintent-securitybaselinetemplate.md)|
|[Criar securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-create.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|Crie um novo [objeto securityBaselineTemplate.](../resources/intune-deviceintent-securitybaselinetemplate.md)|
|[Excluir securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-delete.md)|Nenhum|Exclui um [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).|
|[Atualizar securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-update.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|Atualize as propriedades de [um objeto securityBaselineTemplate.](../resources/intune-deviceintent-securitybaselinetemplate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID do modelo Herdada [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|displayName|Cadeia de caracteres|O nome de exibição do modelo Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|description|Cadeia de caracteres|Descrição do modelo Herdada de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|versionInfo|Cadeia de caracteres|Informações de versão do modelo Herdadas de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|isDeprecated|Boolean|O modelo está preterido ou não. As intenções não podem ser criadas a partir de um modelo preterido. Herdado [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|intentCount|Int32|Número de Intenções criadas a partir deste modelo. Herdado [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|templateType|[deviceManagementTemplateType](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|O tipo do modelo. Herdado [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md). Os valores possíveis são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.|
|platformType|[policyPlatformType](../resources/intune-deviceintent-policyplatformtype.md)|A plataforma do modelo. Herdado [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md). Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.|
|templateSubtype|[deviceManagementTemplateSubtype](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|O subtipo do modelo. Herdado [de deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md). Os valores possíveis são: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.|
|publishedDateTime|DateTimeOffset|Quando o modelo foi publicado Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|configurações|[Coleção deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Coleção de todas as configurações que este modelo herdou de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|categories|[Coleção deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|Coleção de categorias de configuração dentro do modelo Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|migratableTo|[Coleção deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Coleção de modelos que este modelo pode migrar para Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|deviceStateSummary|[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|O resumo do estado do dispositivo de linha de base de segurança|
|deviceStates|[coleção securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Os estados do dispositivo de linha de base de segurança|
|categoryDeviceStateSummaries|[coleção securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|Resumo do estado do dispositivo de categoria da linha de base de segurança por categoria|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "versionInfo": "String",
  "isDeprecated": true,
  "intentCount": 1024,
  "templateType": "String",
  "platformType": "String",
  "templateSubtype": "String",
  "publishedDateTime": "String (timestamp)"
}
```




