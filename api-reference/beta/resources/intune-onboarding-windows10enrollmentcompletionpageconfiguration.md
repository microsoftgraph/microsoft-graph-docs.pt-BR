---
title: tipo de recurso windows10EnrollmentCompletionPageConfiguration
description: Configuração da página de status de registro do Windows 10
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4279ea38c168df6c3bfe8d1b74f9b570c8c327c1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997929"
---
# <a name="windows10enrollmentcompletionpageconfiguration-resource-type"></a>tipo de recurso windows10EnrollmentCompletionPageConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração da página de status de registro do Windows 10


Herda de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows10EnrollmentCompletionPageConfigurations](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-list.md)|coleção [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|Listar Propriedades e relações dos objetos [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .|
|[Obter windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-get.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|Leia as propriedades e as relações do objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .|
|[Criar windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-create.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|Criar um novo objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .|
|[Excluir windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-delete.md)|Nenhum|Exclui [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).|
|[Atualizar windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-update.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|Atualiza as propriedades de um objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da conta herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|displayName|String|O nome de exibição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|descrição|String|A descrição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|prioridade|Int32|A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro. Os usuários estão sujeitos somente à configuração com o menor valor de prioridade. Herdada do [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Data e hora de criação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|versão|Int32|A versão da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|showInstallationProgress|Booliano|Mostrar ou ocultar o andamento da instalação para o usuário|
|blockDeviceSetupRetryByUser|Booliano|Permitir que o usuário repita a configuração após a instalação falhar|
|allowDeviceResetOnInstallFailure|Booliano|Permitir ou bloquear falha de redefinição de dispositivo na instalação|
|allowLogCollectionOnInstallFailure|Booliano|Permitir ou bloquear coleta de log na falha de instalação|
|customErrorMessage|String|Definir uma mensagem de erro personalizada para mostrar após falha da instalação|
|installProgressTimeoutInMinutes|Int32|Definir o tempo limite de progresso da instalação em minutos|
|allowDeviceUseOnInstallFailure|Booliano|Permitir que o usuário continue usando o dispositivo em caso de falha de instalação|
|selectedMobileAppIds|Coleção de cadeias de caracteres|Aplicativos selecionados para acompanhar o status de instalação|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|atribuições|Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EnrollmentCompletionPageConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "showInstallationProgress": true,
  "blockDeviceSetupRetryByUser": true,
  "allowDeviceResetOnInstallFailure": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "String",
  "installProgressTimeoutInMinutes": 1024,
  "allowDeviceUseOnInstallFailure": true,
  "selectedMobileAppIds": [
    "String"
  ]
}
```





