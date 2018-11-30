---
title: Tipo de recurso de usuário
description: Representa um objeto de usuário do Azure Active Directory.
ms.openlocfilehash: ec28b7ec44eddfa1e1e8b372956d1a29dc78553d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037645"
---
# <a name="user-resource-type"></a>Tipo de recurso de usuário

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Representa um objeto de usuário do Azure Active Directory.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Os usuários da lista](../api/intune-shared-user-list.md) de objetos.|Conjunto [user](../resources/intune-shared-user.md)|Listar propriedades e relações de objetos de [user](../resources/intune-shared-user.md).|
|Objeto [obter do usuário](../api/intune-shared-user-get.md) .|[user](../resources/intune-shared-user.md)|Ler propriedades e relações de objetos de [user](../resources/intune-shared-user.md).|
|Objeto de [usuário de criar](../api/intune-shared-user-create.md) .|[user](../resources/intune-shared-user.md)|Criar um novo objeto de [user](../resources/intune-shared-user.md).|
|[Excluir o usuário](../api/intune-shared-user-delete.md).|Nenhum|Excluir [user](../resources/intune-shared-user.md).|
|Objeto de [usuário de atualização](../api/intune-shared-user-update.md) .|[user](../resources/intune-shared-user.md)|Atualizar as propriedades de um objeto de [user](../resources/intune-shared-user.md).|
|**Gerenciamento de dispositivos**|
|[função getLoggedOnManagedDevices](../api/intune-shared-user-getloggedonmanageddevices.md)|Coleção [managedDevice](../resources/intune-devices-manageddevice.md)|Ainda não documentado|
|[Ação removeAllDevicesFromManagement](../api/intune-shared-user-removealldevicesfrommanagement.md)|Nenhum|Desativa todos os dispositivos de gerenciamento deste usuário|
|**Gerenciamento de aplicativos móveis (MAM)**|
|[função getManagedAppDiagnosticStatuses](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|Conjunto [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)|Obtém diagnóstico do status de validação para um determinado usuário.|
|[Função getManagedAppPolicies](../api/intune-shared-user-getmanagedapppolicies.md)|Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Obtém as restrições de aplicativo para um determinado usuário.|
|[ação de wipeManagedAppRegistrationByDeviceTag](../api/intune-shared-user-wipemanagedappregistrationbydevicetag.md)|Nenhum|Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.|
|[Ação wipeManagedAppRegistrationsByDeviceTag](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|Nenhum|Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.|
|**Inclusão**|
|[função exportDeviceAndAppManagementData](../api/intune-shared-user-exportdeviceandappmanagementdata.md)|[deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md)|Ainda não documentado|
|[função getEffectiveDeviceEnrollmentConfigurations](../api/intune-shared-user-geteffectivedeviceenrollmentconfigurations.md)|Coleção [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|Ainda não documentado|
|**Solução de problemas**|
|[função getManagedDevicesWithAppFailures](../api/intune-shared-user-getmanageddeviceswithappfailures.md)|String collection|Recupera a lista de dispositivos com aplicativos com falha.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do usuário.|
|**Inclusão**|
|deviceEnrollmentLimit|Int32|O limite do número máximo de dispositivos que o usuário tem permissão para inscrever. Os valores permitidos vão de 5 a 1000.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Gerenciamento de dispositivos**|
|managedDevices|Conjunto [managedDevice](../resources/intune-devices-manageddevice.md)|Os dispositivos gerenciados associados ao usuário.|
|**Gerenciamento de aplicativos móveis (MAM)**|
|managedAppRegistrations|Conjunto [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Zero ou mais registros de aplicativos gerenciados que pertencem ao usuário.|
|**Inclusão**|
|deviceEnrollmentConfigurations|Coleção [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|Fazer configurações de inscrição voltadas para o usuário|
|**Solução de problemas**|
|deviceManagementTroubleshootingEvents|Conjunto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|A lista de eventos de solução de problemas desse usuário.|
|mobileAppIntentAndStates|coleção [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|A lista de eventos de solução de problemas desse usuário.|
|mobileAppTroubleshootingEvents|coleção [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)|A lista de eventos para esse usuário de solução de problemas de aplicativos móveis.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



