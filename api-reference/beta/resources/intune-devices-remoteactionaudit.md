---
title: Tipo de recurso remoteActionAudit
description: Relatório de ações remotas iniciadas nos dispositivos pertencentes a um determinado locatário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 214ef0f5eed28d02dd172e6acb7845ea379f372f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866570"
---
# <a name="remoteactionaudit-resource-type"></a>Tipo de recurso remoteActionAudit

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Relatório de ações remotas iniciadas nos dispositivos pertencentes a um determinado locatário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar remoteActionAudits](../api/intune-devices-remoteactionaudit-list.md)|[Coleção remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Listar propriedades e relações dos [objetos remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)|
|[Obter remoteActionAudit](../api/intune-devices-remoteactionaudit-get.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Leia propriedades e relações do [objeto remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)|
|[Criar remoteActionAudit](../api/intune-devices-remoteactionaudit-create.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Crie um novo [objeto remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)|
|[Excluir remoteActionAudit](../api/intune-devices-remoteactionaudit-delete.md)|Nenhum|Exclui um [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).|
|[Atualizar remoteActionAudit](../api/intune-devices-remoteactionaudit-update.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Atualize as propriedades de [um objeto remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID do relatório.|
|deviceDisplayName|Cadeia de caracteres|Nome do dispositivo do Intune.|
|userName|Cadeia de caracteres|\[preterido \] Use InitiatedByUserPrincipalName em vez disso.|
|initiatedByUserPrincipalName|Cadeia de Caracteres|Usuário que iniciou a ação do dispositivo, o formato é UPN.|
|ação|[remoteAction](../resources/intune-devices-remoteaction.md)|O nome da ação. Os valores possíveis são: `unknown` , , , , , , , , `factoryReset` `removeCompanyData` , `resetPasscode` , `remoteLock` `enableLostMode` `disableLostMode` `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan` `fullScan` , `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey` `getFileVaultKey` `setDeviceName` `activateDeviceEsim` .|
|requestDateTime|DateTimeOffset|Hora em que a ação foi emitida, dada em UTC.|
|deviceOwnerUserPrincipalName|Cadeia de Caracteres|Upn do proprietário do dispositivo.|
|deviceIMEI|Cadeia de Caracteres|IMEI do dispositivo.|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Estado da ação. Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|managedDeviceId|Cadeia de Caracteres|Destino da ação.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteActionAudit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "initiatedByUserPrincipalName": "String",
  "action": "String",
  "requestDateTime": "String (timestamp)",
  "deviceOwnerUserPrincipalName": "String",
  "deviceIMEI": "String",
  "actionState": "String",
  "managedDeviceId": "String"
}
```




