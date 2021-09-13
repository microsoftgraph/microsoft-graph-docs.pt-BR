---
title: Tipo de recurso macOSExtensionsConfiguration
description: Perfil de configuração de extensões do MacOS.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 113595f623c587e61834417eb84683b77bc32217
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59040404"
---
# <a name="macosextensionsconfiguration-resource-type"></a>Tipo de recurso macOSExtensionsConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Perfil de configuração de extensões do MacOS.


Herda de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSExtensionsConfigurations](../api/intune-deviceconfig-macosextensionsconfiguration-list.md)|[Coleção macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|Listar propriedades e relações dos [objetos macOSExtensionsConfiguration.](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|
|[Obter macOSExtensionsConfiguration](../api/intune-deviceconfig-macosextensionsconfiguration-get.md)|[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|Leia propriedades e relações do [objeto macOSExtensionsConfiguration.](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|
|[Criar macOSExtensionsConfiguration](../api/intune-deviceconfig-macosextensionsconfiguration-create.md)|[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|Crie um novo [objeto macOSExtensionsConfiguration.](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|
|[Excluir macOSExtensionsConfiguration](../api/intune-deviceconfig-macosextensionsconfiguration-delete.md)|Nenhum|Exclui um [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md).|
|[Atualizar macOSExtensionsConfiguration](../api/intune-deviceconfig-macosextensionsconfiguration-update.md)|[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|Atualize as propriedades de [um objeto macOSExtensionsConfiguration.](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String collection|Lista de marcas de escopo para esta instância entity. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boleano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|kernelExtensionOverridesAllowed|Boleano|Se definido como true, os usuários podem aprovar extensões de kernel adicionais não explicitamente permitidas pelos perfis de configurações.|
|kernelExtensionAllowedTeamIdentifiers|String collection|Todas as extensões de kernel assinadas pelos identificadores de equipe nesta lista terão permissão para carregar.|
|kernelExtensionsAllowed|[Coleção macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md)|Uma lista de extensões de kernel que poderão ser carregadas. . Esta coleção pode conter um máximo de 500 elementos.|
|systemExtensionsBlockOverride|Boleano|Obtém ou define se o usuário deve permitir que o usuário aprove extensões adicionais do sistema não explicitamente permitidas pelos perfis de configuração.|
|systemExtensionsAllowedTeamIdentifiers|String collection|Obtém ou define uma lista de identificadores de equipe permitidos. Qualquer extensão do sistema assinada com qualquer um dos identificadores de equipe especificados será aprovada.|
|systemExtensionsAllowed|[Coleção macOSSystemExtension](../resources/intune-deviceconfig-macossystemextension.md)|Obtém ou define uma lista de extensões de sistema macOS permitidas. Esta coleção pode conter um máximo de 500 elementos.|
|systemExtensionsAllowedTypes|[Coleção macOSSystemExtensionTypeMapping](../resources/intune-deviceconfig-macossystemextensiontypemapping.md)|Obtém ou define uma lista de tipos de extensão do sistema macOS permitidos. Esta coleção pode conter um máximo de 500 elementos.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|[Coleção deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status da instalação da configuração de dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status da instalação de configuração do dispositivo pelo usuário. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSExtensionsConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "String"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "String",
      "bundleId": "String"
    }
  ],
  "systemExtensionsBlockOverride": true,
  "systemExtensionsAllowedTeamIdentifiers": [
    "String"
  ],
  "systemExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtension",
      "teamIdentifier": "String",
      "bundleId": "String"
    }
  ],
  "systemExtensionsAllowedTypes": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping",
      "teamIdentifier": "String",
      "allowedTypes": "String"
    }
  ]
}
```



