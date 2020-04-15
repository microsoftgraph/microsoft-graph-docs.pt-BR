---
title: Tipo de recurso enrollmentTroubleshootingEvent
description: Evento que representa uma falha de registro.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e69ed266e5e3a543c79bc1fb08285bb68aa7e3d9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468372"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a>Tipo de recurso enrollmentTroubleshootingEvent

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Evento que representa uma falha de registro.


Herda de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar enrollmentTroubleshootingEvents](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|Coleção [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|Lista propriedades e relações dos objetos [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).|
|[Obter enrollmentTroubleshootingEvent](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|Propriedades de leitura e relações do objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).|
|[Criar enrollmentTroubleshootingEvent](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|Cria um novo objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).|
|[Excluir enrollmentTroubleshootingEvent](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|Nenhum|Exclui um [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).|
|[Atualizar enrollmentTroubleshootingEvent](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|Atualiza as propriedades de um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|eventDateTime|DateTimeOffset|A hora em que o evento ocorreu. Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|correlationId|String|ID usada para rastrear a falha no serviço. Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|managedDeviceIdentifier|String|Identificador de dispositivo criado ou coletado pelo Intune.|
|operatingSystem|String|Sistema operacional.|
|osVersion|String|Versão do sistema operacional.|
|userId|Cadeia de caracteres|Identificador do usuário que tentou registrar o dispositivo.|
|deviceId|String|Identificador do dispositivo Azure AD.|
|enrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|Tipo do registro. Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|failureCategory|[deviceEnrollmentFailureReason](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|Categoria de falha de alto nível. Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.|
|failureReason|Cadeia de caracteres|Motivo detalhado da falha.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "managedDeviceIdentifier": "String",
  "operatingSystem": "String",
  "osVersion": "String",
  "userId": "String",
  "deviceId": "String",
  "enrollmentType": "String",
  "failureCategory": "String",
  "failureReason": "String"
}
```







