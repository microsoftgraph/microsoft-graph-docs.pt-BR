---
title: Atualizar remoteActionAudit
description: Atualiza as propriedades de um objeto remoteActionAudit.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7f579d5f982daa1bc1ab045cfca464a8f3b6d5f4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43323448"
---
# <a name="update-remoteactionaudit"></a>Atualizar remoteActionAudit

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualiza as propriedades de um objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID de relatório.|
|deviceDisplayName|Cadeia de caracteres|Nome do dispositivo do Intune.|
|userName|String|\[\] preterido use InitiatedByUserPrincipalName em vez disso.|
|initiatedByUserPrincipalName|String|O formato de usuário que iniciou a ação do dispositivo é UPN.|
|ação|[remoteaction](../resources/intune-devices-remoteaction.md)|O nome da ação. Os valores possíveis são `unknown`: `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock` `enableLostMode` `disableLostMode`,,, `locateDevice`, `rebootNow`, `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser`,,, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey` `getFileVaultKey`,,,, `setDeviceName`,,,,,,,,,.|
|requestDateTime|DateTimeOffset|Hora em que a ação foi emitida, dada em UTC.|
|deviceOwnerUserPrincipalName|String|UPN do proprietário do dispositivo.|
|deviceIMEI|String|IMEI do dispositivo.|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Estado de ação. Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|managedDeviceId|String|Destino de ação.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
Content-type: application/json
Content-length: 504

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending",
  "managedDeviceId": "Managed Device Id value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "477f8d24-8d24-477f-248d-7f47248d7f47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending",
  "managedDeviceId": "Managed Device Id value"
}
```



