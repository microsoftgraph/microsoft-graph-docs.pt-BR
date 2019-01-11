---
title: tipo de recurso de remoteActionAudit
description: Relatório de ações remotos iniciadas nos dispositivos que pertencem a um determinado inquilino.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7624610ed35a583e0ec11582caa1dccda5ce4ce7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840807"
---
# <a name="remoteactionaudit-resource-type"></a>tipo de recurso de remoteActionAudit

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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
|id|Cadeia de caracteres|ID do relatório.|
|deviceDisplayName|Cadeia de caracteres|Nome do dispositivo Intune.|
|userName|Cadeia de caracteres|\[preterido\] use InitiatedByUserPrincipalName em vez disso.|
|initiatedByUserPrincipalName|Cadeia de caracteres|Usuário que iniciou a ação de dispositivo, formato é UPN.|
|action|[remoteAction](../resources/intune-devices-remoteaction.md)|O nome da ação. Os valores possíveis são: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` .|
|requestDateTime|DateTimeOffset|Tempo quando a ação foi emitida, dado em UTC.|
|deviceOwnerUserPrincipalName|Cadeia de caracteres|Nome UPN do proprietário do dispositivo.|
|deviceIMEI|Cadeia de caracteres|IMEI do dispositivo.|
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





