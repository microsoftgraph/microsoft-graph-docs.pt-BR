---
title: Criar deviceInstallState
description: Criar um novo objeto deviceInstallState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4afc3670cc230a790072d20c8b0e32af13cef326
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730501"
---
# <a name="create-deviceinstallstate"></a>Criar deviceInstallState

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Criar um novo objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementApps.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto deviceInstallState.

A tabela a seguir mostra as propriedades que são necessárias ao criar deviceInstallState.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|deviceName|Cadeia de caracteres|Nome do dispositivo.|
|deviceId|Cadeia de caracteres|ID do dispositivo.|
|lastSyncDateTime|DateTimeOffset|Última sincronização de data e hora.|
|installState|[installState](../resources/intune-books-installstate.md)|O estado de instalação do livro eletrônico. Os valores possíveis são: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.|
|errorCode|Cadeia de caracteres|O código de erro de falhas de instalação.|
|osVersion|Cadeia de caracteres|Versão do sistema operacional.|
|osDescription|Cadeia de caracteres|Descrição do sistema operacional.|
|userName|Cadeia de caracteres|Nome de usuário do dispositivo.|



## <a name="response"></a>Resposta
Se tiver êxito, esse método retornará um código de resposta `201 Created` e um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```





