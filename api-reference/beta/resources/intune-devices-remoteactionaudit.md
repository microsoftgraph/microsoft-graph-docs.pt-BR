---
title: tipo de recurso de remoteActionAudit
description: Relatório de ações remotos iniciadas nos dispositivos que pertencem a um determinado inquilino.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ebe93b2f2e70011fb75a08b91938f26d723d1d5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404908"
---
# <a name="remoteactionaudit-resource-type"></a>tipo de recurso de remoteActionAudit

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Relatório de ações remotos iniciadas nos dispositivos que pertencem a um determinado inquilino.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista remoteActionAudits](../api/intune-devices-remoteactionaudit-list.md)|coleção [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Lista as propriedades e os relacionamentos dos objetos [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .|
|[Obter remoteActionAudit](../api/intune-devices-remoteactionaudit-get.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Leia as propriedades e os relacionamentos do objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .|
|[Criar remoteActionAudit](../api/intune-devices-remoteactionaudit-create.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Crie um novo objeto de [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .|
|[Excluir remoteActionAudit](../api/intune-devices-remoteactionaudit-delete.md)|Nenhum|Exclui um [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).|
|[Atualizar remoteActionAudit](../api/intune-devices-remoteactionaudit-update.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Atualize as propriedades de um objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID do relatório.|
|deviceDisplayName|Cadeia de caracteres|Nome do dispositivo Intune.|
|userName|Cadeia de caracteres|\[preterido\] use InitiatedByUserPrincipalName em vez disso.|
|initiatedByUserPrincipalName|String|Usuário que iniciou a ação de dispositivo, formato é UPN.|
|action|[remoteAction](../resources/intune-devices-remoteaction.md)|O nome da ação. Os valores possíveis são: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` .|
|requestDateTime|DateTimeOffset|Tempo quando a ação foi emitida, dado em UTC.|
|deviceOwnerUserPrincipalName|String|Nome UPN do proprietário do dispositivo.|
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




