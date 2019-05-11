---
title: Criar deviceManagementScript
description: Criar um novo objeto deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a58b0d4f957dc6cdfc98c58449c2b12dfba19397
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33910041"
---
# <a name="create-devicemanagementscript"></a>Criar deviceManagementScript

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Criar um novo objeto [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

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
No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScript.

A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScript.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do script de gerenciamento de dispositivo.|
|displayName|Cadeia de caracteres|Nome do script de gerenciamento de dispositivo.|
|description|String|Descrição opcional para o script de gerenciamento de dispositivo.|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|O intervalo de execução do script. Se não definido, o script será executado uma vez|
|scriptContent|Binária|O conteúdo de script.|
|createdDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivo foi criado.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Indica o tipo de contexto de execução. Os valores possíveis são: `system` e `user`.|
|enforceSignatureCheck|Booliano|Indica se a assinatura do script precisa ser verificada.|
|fileName|String|Nome do arquivo de script.|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de IDs de marca de escopo para esta instância de PowerShellScript.|
|runAs32Bit|Booliano|Um valor que indica se o script do PowerShell deve ser executado como 32 bits|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
Content-type: application/json
Content-length: 443

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
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
  "runAs32Bit": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 615

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
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
  "runAs32Bit": true
}
```




