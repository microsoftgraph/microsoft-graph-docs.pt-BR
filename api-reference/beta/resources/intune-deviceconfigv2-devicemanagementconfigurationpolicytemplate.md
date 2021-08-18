---
title: Tipo de recurso deviceManagementConfigurationPolicyTemplate
description: Modelo de Política de Configuração de Gerenciamento de Dispositivos
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e891f9784e6306b69650672b8e4e18ed4f6a7d294d84916451a1a9553ba7d30e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182900"
---
# <a name="devicemanagementconfigurationpolicytemplate-resource-type"></a>Tipo de recurso deviceManagementConfigurationPolicyTemplate

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modelo de Política de Configuração de Gerenciamento de Dispositivos

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementConfigurationPolicyTemplates](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-list.md)|[Coleção deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|Listar propriedades e relações dos [objetos deviceManagementConfigurationPolicyTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|
|[Obter deviceManagementConfigurationPolicyTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-get.md)|[deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|Leia propriedades e relações do [objeto deviceManagementConfigurationPolicyTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|
|[Criar deviceManagementConfigurationPolicyTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-create.md)|[deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|Crie um novo [objeto deviceManagementConfigurationPolicyTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|
|[Excluir deviceManagementConfigurationPolicyTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-delete.md)|Nenhum|Exclui um [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md).|
|[Atualizar deviceManagementConfigurationPolicyTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-update.md)|[deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|Atualize as propriedades de [um objeto deviceManagementConfigurationPolicyTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave do documento do modelo, composta por BaseId e Version. Gerado automaticamente.|
|baseId|Cadeia de caracteres|Identificador de base de modelos|
|versão|Int32|Versão do modelo. Valores válidos 1 a 2147483647. Essa propriedade é somente leitura.|
|displayName|Cadeia de caracteres|Nome de exibição do modelo|
|description|Cadeia de caracteres|Descrição do modelo|
|displayVersion|Cadeia de caracteres|Descrição da versão do modelo|
|lifecycleState|[deviceManagementTemplateLifecycleState](../resources/intune-deviceconfigv2-devicemanagementtemplatelifecyclestate.md)|Indique o estado atual do modelo de ciclo de vida. Os possíveis valores são: `invalid`, `draft`, `active`, `superseded`, `deprecated`, `retired`.|
|plataformas|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Plataformas para este modelo. Os valores possíveis são: `none`, `macOS`, `windows10X`, `windows10`.|
|technologies|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Tecnologias para este modelo. Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.|
|templateFamily|[deviceManagementConfigurationTemplateFamily](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|TemplateFamily para este modelo. Os valores possíveis são: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.|
|allowUnmanagedSettings|Boolean|Permitir modelos de configuração nãomanageados|
|settingTemplateCount|Int32|Número de modelos de configuração. Valores válidos de 0 a 2147483647. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|settingTemplates|[Coleção deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|Modelos de configuração|

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




