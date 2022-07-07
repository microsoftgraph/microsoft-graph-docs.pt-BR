---
title: Tipo de recurso deviceManagementConfigurationPolicyTemplate
description: Gerenciamento de Dispositivos de Política de Configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ab8a9ed5c4402ea61fa4d1d4263d186c41d6e928
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668717"
---
# <a name="devicemanagementconfigurationpolicytemplate-resource-type"></a>Tipo de recurso deviceManagementConfigurationPolicyTemplate

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Gerenciamento de Dispositivos de Política de Configuração

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementConfigurationPolicyTemplates](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-list.md)|[Coleção deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|Listar propriedades e relações dos [objetos deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) .|
|[Obter deviceManagementConfigurationPolicyTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-get.md)|[deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|Ler propriedades e relações do objeto [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) .|
|[Criar deviceManagementConfigurationPolicyTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-create.md)|[deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|Crie um novo [objeto deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) .|
|[Excluir deviceManagementConfigurationPolicyTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-delete.md)|Nenhum|Exclui um [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md).|
|[Atualizar deviceManagementConfigurationPolicyTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-update.md)|[deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|Atualize as propriedades de [um objeto deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave do documento de modelo, composta por BaseId e Version. Gerado automaticamente.|
|baseId|String|Identificador base do modelo|
|versão|Int32|Versão do modelo. Valores válidos 1 a 2147483647. Essa propriedade é somente leitura.|
|displayName|String|Nome de exibição do modelo|
|descrição|String|Descrição do modelo|
|displayVersion|Cadeia de caracteres|Descrição da versão do modelo|
|lifecycleState|[deviceManagementTemplateLifecycleState](../resources/intune-deviceconfigv2-devicemanagementtemplatelifecyclestate.md)|Indique o estado atual do ciclo de vida do modelo. Os possíveis valores são: `invalid`, `draft`, `active`, `superseded`, `deprecated`, `retired`.|
|Plataformas|[deviceManagementConfigurationPlatforms](../resources/intune-shared-devicemanagementconfigurationplatforms.md)|Plataformas para este modelo. Os valores possíveis são: `none`, `android`, `iOS`, `macOS`, `windows10X`, `windows10`, `linux`, `unknownFutureValue`.|
|Tecnologias|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Tecnologias para este modelo. Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`, `appleRemoteManagement`, `microsoftSense`, `exchangeOnline`, `linuxMdm`, `enrollment`, `unknownFutureValue`.|
|templateFamily|[deviceManagementConfigurationTemplateFamily](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|TemplateFamily para este modelo. Os valores possíveis são: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`, `baseline`.|
|allowUnmanagedSettings|Boolean|Permitir modelos de configuração não gerenciados|
|settingTemplateCount|Int32|Número de modelos de configuração. Valores válidos de 0 a 2147483647. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|settingTemplates|[Coleção deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|Definindo modelos|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplate",
  "id": "String (identifier)",
  "baseId": "String",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "displayVersion": "String",
  "lifecycleState": "String",
  "platforms": "String",
  "technologies": "String",
  "templateFamily": "String",
  "allowUnmanagedSettings": true,
  "settingTemplateCount": 1024
}
```




