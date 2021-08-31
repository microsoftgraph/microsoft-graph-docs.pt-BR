---
title: Tipo de recurso deviceComanagementAuthorityConfiguration
description: Windows 10 Co-Management Configuração da Página de Autoridade
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c3314c33a80aaf4c922e22a88b3536f0012cfe95
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793793"
---
# <a name="devicecomanagementauthorityconfiguration-resource-type"></a>Tipo de recurso deviceComanagementAuthorityConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows 10 Co-Management Configuração da Página de Autoridade


Herda de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceComanagementAuthorityConfigurations](../api/intune-onboarding-devicecomanagementauthorityconfiguration-list.md)|[Coleção deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|Listar propriedades e relações dos [objetos deviceComanagementAuthorityConfiguration.](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|
|[Obter deviceComanagementAuthorityConfiguration](../api/intune-onboarding-devicecomanagementauthorityconfiguration-get.md)|[deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|Leia propriedades e relações do [objeto deviceComanagementAuthorityConfiguration.](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|
|[Criar deviceComanagementAuthorityConfiguration](../api/intune-onboarding-devicecomanagementauthorityconfiguration-create.md)|[deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|Crie um novo [objeto deviceComanagementAuthorityConfiguration.](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|
|[Excluir deviceComanagementAuthorityConfiguration](../api/intune-onboarding-devicecomanagementauthorityconfiguration-delete.md)|Nenhum(a)|Exclui um [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md).|
|[Atualizar deviceComanagementAuthorityConfiguration](../api/intune-onboarding-devicecomanagementauthorityconfiguration-update.md)|[deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|Atualize as propriedades de [um objeto deviceComanagementAuthorityConfiguration.](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da conta Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|Cadeia de caracteres|O nome de exibição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|descrição|Cadeia de caracteres|A descrição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|prioridade|Int32|A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro. Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixo. Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Hora de data criada em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Última data de modificação no UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|versão|Int32|A versão da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Marcas de escopo de função opcionais para as restrições de registro. Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|managedDeviceAuthority|Int32|Configuração da Autoridade de CoManagement ManagedDeviceAuthority|
|installConfigurationManagerAgent|Boleano|Configuração da Autoridade de Gerenciamento de CoManagement InstallConfigurationManagerAgent|
|configurationManagerAgentCommandLineArgument|Cadeia de caracteres|Configuração da Autoridade de CoManagement ConfigurationManagerAgentCommandLineArgument|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|atribuições|Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo Herdado de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComanagementAuthorityConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComanagementAuthorityConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "roleScopeTagIds": [
    "String"
  ],
  "managedDeviceAuthority": 1024,
  "installConfigurationManagerAgent": true,
  "configurationManagerAgentCommandLineArgument": "String"
}
```



