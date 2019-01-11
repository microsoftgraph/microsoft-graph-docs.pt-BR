---
title: tipo de recurso de windows10EnrollmentCompletionPageConfiguration
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f843a36c5852f3a565894e5ea7e2d6f0ff70954e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844713"
---
# <a name="windows10enrollmentcompletionpageconfiguration-resource-type"></a>tipo de recurso de windows10EnrollmentCompletionPageConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ainda não documentado

Herda de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista windows10EnrollmentCompletionPageConfigurations](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-list.md)|coleção [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|Lista as propriedades e os relacionamentos dos objetos [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .|
|[Obter windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-get.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|Leia as propriedades e os relacionamentos do objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .|
|[Criar windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-create.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|Crie um novo objeto de [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .|
|[Excluir windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-delete.md)|Nenhum|Exclui um [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).|
|[Atualizar windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-update.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|Atualize as propriedades de um objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|displayName|Cadeia de caracteres|Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|description|Cadeia de caracteres|Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|prioridade|Int32|Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|version|Int32|Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|showInstallationProgress|Booliano|Mostrar ou ocultar o progresso da instalação para o usuário|
|blockDeviceSetupRetryByUser|Booliano|Permitir que o usuário repetir a instalação em caso de falha de instalação|
|allowDeviceResetOnInstallFailure|Booliano|Permitir ou bloquear o dispositivo redefinir em caso de falha de instalação|
|allowLogCollectionOnInstallFailure|Booliano|Permitir ou bloquear o conjunto de log em caso de falha de instalação|
|customErrorMessage|Cadeia de caracteres|Definir a mensagem de erro personalizada para mostrar após a falha de instalação|
|installProgressTimeoutInMinutes|Int32|Definir tempo limite de progresso de instalação em minutos|
|allowDeviceUseOnInstallFailure|Booliano|Permitir que o usuário continue a usar o dispositivo em caso de falha de instalação|
|selectedMobileAppIds|String collection|Aplicativos selecionados para rastrear o status de instalação|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|atribuições|Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada do [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|

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





