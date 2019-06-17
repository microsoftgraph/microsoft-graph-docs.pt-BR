---
title: tipo de recurso remoteActionAudit
description: Relatório de ações remotas iniciadas nos dispositivos que pertencem a um determinado locatário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: daaf42914d18e2016c7db566f9a91bd4037b10a6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963881"
---
# <a name="remoteactionaudit-resource-type"></a>tipo de recurso remoteActionAudit

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Relatório de ações remotas iniciadas nos dispositivos que pertencem a um determinado locatário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar remoteActionAudits](../api/intune-devices-remoteactionaudit-list.md)|coleção [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Listar Propriedades e relações dos objetos [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .|
|[Obter remoteActionAudit](../api/intune-devices-remoteactionaudit-get.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Leia as propriedades e as relações do objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .|
|[Criar remoteActionAudit](../api/intune-devices-remoteactionaudit-create.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Criar um novo objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .|
|[Excluir remoteActionAudit](../api/intune-devices-remoteactionaudit-delete.md)|Nenhum|Exclui [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).|
|[Atualizar remoteActionAudit](../api/intune-devices-remoteactionaudit-update.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Atualiza as propriedades de um objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID de relatório.|
|deviceDisplayName|Cadeia de caracteres|Nome do dispositivo do Intune.|
|userName|String|\[\] preterido use InitiatedByUserPrincipalName em vez disso.|
|initiatedByUserPrincipalName|String|O formato de usuário que iniciou a ação do dispositivo é UPN.|
|ação|[remoteaction](../resources/intune-devices-remoteaction.md)|O nome da ação. Os valores possíveis são: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateFileVaultKey`, `getFileVaultKey`.|
|requestDateTime|DateTimeOffset|Hora em que a ação foi emitida, dada em UTC.|
|deviceOwnerUserPrincipalName|String|UPN do proprietário do dispositivo.|
|deviceIMEI|String|IMEI do dispositivo.|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Estado de ação. Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|

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
  "actionState": "String"
}
```





