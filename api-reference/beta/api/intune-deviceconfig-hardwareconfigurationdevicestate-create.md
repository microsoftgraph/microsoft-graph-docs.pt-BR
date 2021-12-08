---
title: Criar hardwareConfigurationDeviceState
description: Crie um novo objeto hardwareConfigurationDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d8e2a81c7d706d45e56dae807cb54fe26661459
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348371"
---
# <a name="create-hardwareconfigurationdevicestate"></a>Criar hardwareConfigurationDeviceState

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto hardwareConfigurationDeviceState.](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/deviceRunStates
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto hardwareConfigurationDeviceState.

A tabela a seguir mostra as propriedades que são necessárias ao criar o hardwareConfigurationDeviceState.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade de estado do dispositivo de script de configuração de hardware. Essa propriedade é somente leitura.|
|deviceName|String|O nome do dispositivo|
|osVersion|String|A versão do sistema operacional do dispositivo.|
|upn|Cadeia de caracteres|Nome principal do usuário (UPN).|
|internalVersion|Int32|A versão interna da Política|
|lastStateUpdateDateTime|DateTimeOffset|O último período de data/hora de quando a configuração de hardware foi executada|
|configurationState|[runState](../resources/intune-shared-runstate.md)|Estado de configuração da última execução de configuração de hardware. Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|configurationOutput|String|Saída da execução da configuração de hardware|
|configurationError|String|Erro da execução da configuração de hardware|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/deviceRunStates
Content-type: application/json
Content-length: 410

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationDeviceState",
  "deviceName": "Device Name value",
  "osVersion": "Os Version value",
  "upn": "Upn value",
  "internalVersion": 15,
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "configurationState": "success",
  "configurationOutput": "Configuration Output value",
  "configurationError": "Configuration Error value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 459

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationDeviceState",
  "id": "74b9fcd8-fcd8-74b9-d8fc-b974d8fcb974",
  "deviceName": "Device Name value",
  "osVersion": "Os Version value",
  "upn": "Upn value",
  "internalVersion": 15,
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "configurationState": "success",
  "configurationOutput": "Configuration Output value",
  "configurationError": "Configuration Error value"
}
```




