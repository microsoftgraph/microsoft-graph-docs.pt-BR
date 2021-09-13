---
title: Tipo de recurso deviceManagementTemplate
description: Entidade que representa uma coleção definida de configurações de dispositivo
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 434f62be55ebd1fef116d07e27fd9fcb7541d009
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086384"
---
# <a name="devicemanagementtemplate-resource-type"></a>Tipo de recurso deviceManagementTemplate

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa uma coleção definida de configurações de dispositivo

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementTemplates](../api/intune-deviceintent-devicemanagementtemplate-list.md)|[Coleção deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Listar propriedades e relações dos [objetos deviceManagementTemplate.](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|[Obter deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-get.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Leia propriedades e relações do [objeto deviceManagementTemplate.](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|[Criar deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-create.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Crie um novo [objeto deviceManagementTemplate.](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|[Excluir deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-delete.md)|Nenhum|Exclui um [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).|
|[Atualizar deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-update.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Atualize as propriedades de [um objeto deviceManagementTemplate.](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|[ação createInstance](../api/intune-deviceintent-devicemanagementtemplate-createinstance.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Ainda não documentado|
|[função compare](../api/intune-deviceintent-devicemanagementtemplate-compare.md)|[Coleção deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md)|Ainda não documentado|
|[Ação importOffice365DeviceConfigurationPolicies](../api/intune-deviceintent-devicemanagementtemplate-importoffice365deviceconfigurationpolicies.md)|[Coleção deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID do modelo|
|displayName|Cadeia de caracteres|O nome de exibição do modelo|
|description|Cadeia de caracteres|A descrição do modelo|
|versionInfo|Cadeia de Caracteres|Informações de versão do modelo|
|isDeprecated|Boleano|O modelo está preterido ou não. As intenções não podem ser criadas a partir de um modelo preterido.|
|intentCount|Int32|Número de Intenções criadas a partir deste modelo.|
|templateType|[deviceManagementTemplateType](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|O tipo do modelo. Os valores possíveis são: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.|
|platformType|[policyPlatformType](../resources/intune-deviceintent-policyplatformtype.md)|A plataforma do modelo. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.|
|templateSubtype|[deviceManagementTemplateSubtype](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|O subtipo do modelo. Os valores possíveis são: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.|
|publishedDateTime|DateTimeOffset|Quando o modelo foi publicado|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|configurações|[Coleção deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Coleção de todas as configurações que este modelo tem|
|categories|[Coleção deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|Coleção de categorias de configuração dentro do modelo|
|migratableTo|[Coleção deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Coleção de modelos que este modelo pode migrar para|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
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



