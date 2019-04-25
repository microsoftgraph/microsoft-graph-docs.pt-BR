---
title: Atualizar embeddedSIMDeviceState
description: Atualiza as propriedades de um objeto embeddedSIMDeviceState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1fbf7679467e228531bb7bc57eb9e11f5a2c9eff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532384"
---
# <a name="update-embeddedsimdevicestate"></a>Atualizar embeddedSIMDeviceState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualiza as propriedades de um objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para o status do dispositivo SIM incorporado. Valor gerado pelo sistema atribuído quando criado.|
|createdDateTime|DateTimeOffset|A hora em que o status do dispositivo SIM incorporado foi criado. Lado do serviço gerado.|
|modifiedDateTime|DateTimeOffset|A hora em que o status do dispositivo SIM incorporado foi modificado pela última vez. Atualizado o lado do serviço.|
|lastSyncDateTime|DateTimeOffset|A hora em que o dispositivo SIM incorporado foi verificado pela última vez. Atualizado o lado do serviço.|
|universalIntegratedCircuitCardIdentifier|String|O identificador de cartão de circuito integrado universal (UICCID) identificando o hardware no qual um perfil deve ser implantado.|
|deviceName|String|Nome do dispositivo para o qual a assinatura foi provisionada, por exemplo, DESKTOP-JOE|
|userName|Cadeia de caracteres|Nome de usuário para o qual a assinatura foi provisionada, por exemplo, joe@contoso.com|
|estado|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|O estado da operação de perfil aplicada ao dispositivo. Os valores possíveis são: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.|
|stateDetails|String|Descrição da cadeia de caracteres do estado de provisionamento.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "908884a3-84a3-9088-a384-8890a3848890",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```





