---
title: Tipo de recurso de usuário
description: Representa um objeto de usuário do Azure Active Directory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: daa6f7a4802341347f364040504368dc96d75e33
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163368"
---
# <a name="user-resource-type"></a>Tipo de recurso de usuário

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um objeto de usuário do Azure Active Directory.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar](../api/intune-shared-user-list.md) objetos users.|Conjunto [user](../resources/intune-shared-user.md)|Listar propriedades e relações de objetos de [user](../resources/intune-shared-user.md).|
|[Obtenha](../api/intune-shared-user-get.md) o objeto user.|[user](../resources/intune-shared-user.md)|Ler propriedades e relações de objetos de [user](../resources/intune-shared-user.md).|
|[Criar objeto user](../api/intune-shared-user-create.md) .|[user](../resources/intune-shared-user.md)|Criar um novo objeto de [user](../resources/intune-shared-user.md).|
|[Excluir usuário](../api/intune-shared-user-delete.md).|Nenhum|Excluir [user](../resources/intune-shared-user.md).|
|[Atualize](../api/intune-shared-user-update.md) o objeto do usuário.|[user](../resources/intune-shared-user.md)|Atualizar as propriedades de um objeto de [user](../resources/intune-shared-user.md).|
|**Gerenciamento de dispositivos**|
|[função getLoggedOnManagedDevices](../api/intune-shared-user-getloggedonmanageddevices.md)|Coleção [managedDevice](../resources/intune-devices-manageddevice.md)|Ainda não documentado|
|[Ação removeAllDevicesFromManagement](../api/intune-shared-user-removealldevicesfrommanagement.md)|Nenhum|Desativa todos os dispositivos de gerenciamento deste usuário|
|**Gerenciamento de aplicativo móvel (MAM)**|
|[função getManagedAppDiagnosticStatuses](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|Conjunto [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)|Obtém diagnóstico do status de validação para um determinado usuário.|
|[Função getManagedAppPolicies](../api/intune-shared-user-getmanagedapppolicies.md)|Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Obtém as restrições de aplicativo para um determinado usuário.|
|[Ação wipeManagedAppRegistrationByDeviceTag](../api/intune-shared-user-wipemanagedappregistrationbydevicetag.md)|Nenhum|Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.|
|[Ação wipeManagedAppRegistrationsByDeviceTag](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|Nenhum|Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.|
|**Integração**|
|[função exportDeviceAndAppManagementData](../api/intune-shared-user-exportdeviceandappmanagementdata.md)|[deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md)|Ainda não documentado|
|[função getEffectiveDeviceEnrollmentConfigurations](../api/intune-shared-user-geteffectivedeviceenrollmentconfigurations.md)|Coleção [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|Ainda não documentado|
|**Solução de problemas**|
|[função getManagedDevicesWithAppFailures](../api/intune-shared-user-getmanageddeviceswithappfailures.md)|Coleção de cadeias de caracteres|Recupera a lista de dispositivos com aplicativos com falha.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do usuário.|
|**Integração**|
|deviceEnrollmentLimit|Int32|O limite do número máximo de dispositivos que o usuário tem permissão para inscrever. Os valores permitidos vão de 5 a 1000.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Gerenciamento de dispositivos**|
|managedDevices|Conjunto [managedDevice](../resources/intune-devices-manageddevice.md)|Os dispositivos gerenciados associados ao usuário.|
|**Gerenciamento de aplicativo móvel (MAM)**|
|managedAppRegistrations|Conjunto [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Zero ou mais registros de aplicativos gerenciados que pertencem ao usuário.|
|**Integração**|
|deviceEnrollmentConfigurations|Coleção [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|Obter configurações de registro direcionadas para o usuário|
|**Solução de problemas**|
|deviceManagementTroubleshootingEvents|Conjunto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|A lista de eventos de solução de problemas desse usuário.|
|mobileAppIntentAndStates|coleção [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|A lista de eventos de solução de problemas desse usuário.|
|mobileAppTroubleshootingEvents|coleção [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|A lista de eventos de solução de problemas de aplicativo móvel para este usuário.|

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



