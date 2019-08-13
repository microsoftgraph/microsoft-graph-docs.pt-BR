---
title: Criar deviceHealthScript
description: Criar um novo objeto deviceHealthScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0084852f4c0cb236931ee532f12e54a08c1e2fc2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36311613"
---
# <a name="create-devicehealthscript"></a>Criar deviceHealthScript

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Criar um novo objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .

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
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto deviceHealthScript.

A tabela a seguir mostra as propriedades que são necessárias ao criar deviceHealthScript.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do script de gerenciamento de dispositivo. Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|displayName|String|Nome do script de gerenciamento de dispositivo. Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|descrição|String|Descrição opcional para o script de gerenciamento de dispositivo. Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|O intervalo de execução do script. Se não definido, o script será executado uma vez herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|scriptContent|Binária|O conteúdo de script. Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|createdDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivo foi criado. Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez. Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Indica o tipo de contexto de execução. Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md). Os valores possíveis são: `system` e `user`.|
|enforceSignatureCheck|Booliano|Indica se a assinatura do script precisa ser verificada. Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|fileName|String|Nome do arquivo de script. Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de IDs de marca de escopo para esta instância de PowerShellScript. Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|runAs32Bit|Booliano|Um valor que indica se o script do PowerShell deve ser executado como 32 bits herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|complianceRule|[deviceHealthScriptComplianceRule](../resources/intune-devices-devicehealthscriptcompliancerule.md)|Ainda não documentado|
|remediationScriptContent|Binária|Ainda não documentado|
|runRemediationScript|Booliano|Ainda não documentado|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
Content-type: application/json
Content-length: 745

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "string",
    "operator": "equal",
    "detectionValue": "Detection Value value"
  },
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runRemediationScript": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 917

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "string",
    "operator": "equal",
    "detectionValue": "Detection Value value"
  },
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runRemediationScript": true
}
```






