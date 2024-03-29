---
title: Criar userExperienceAnalyticsRemoteConnection
description: Crie um novo objeto userExperienceAnalyticsRemoteConnection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ff06e498cd2f0d1757ae2e9f4c387c6f98efe90
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342101"
---
# <a name="create-userexperienceanalyticsremoteconnection"></a>Criar userExperienceAnalyticsRemoteConnection

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsRemoteConnection
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsRemoteConnection.

A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsRemoteConnection.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo da entidade de conexão remota de análise de experiência do usuário.|
|deviceId|Cadeia de caracteres|A id do dispositivo.|
|deviceName|String|O nome do dispositivo.|
|modelo|String|O modelo de dispositivo de análise de experiência do usuário.|
|virtualNetwork|String|A rede virtual de análise de experiência do usuário.|
|fabricante|String|O fabricante de análise de experiência do usuário.|
|deviceCount|Int32|A contagem de conexão remota. Valores válidos de 0 a 2147483647|
|cloudPcRoundTripTime|Duplo|O tempo de dica de ida e volta do dispositivo cloud pc. Valores válidos de 0 a 1,79769313486232E+308|
|cloudPcSignInTime|Duplo|A hora de entrada do dispositivo cloud pc. Valores válidos de 0 a 1,79769313486232E+308|
|remoteSignInTime|Duplo|A hora de entrada remota do dispositivo cloud pc. Valores válidos de 0 a 1,79769313486232E+308|
|coreBootTime|Duplo|O tempo de inicialização principal do Dispositivo cloud pc. Valores válidos de 0 a 1,79769313486232E+308|
|coreSignInTime|Duplo|A hora de entrada principal do dispositivo cloud pc. Valores válidos de 0 a 1,79769313486232E+308|
|cloudPcFailurePercentage|Duplo|A porcentagem de falha de entrada do dispositivo cloud pc. Valores válidos de 0 a 100|
|userPrincipalName|String|O usuário de análise de experiência do usuárioPrincipalName.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection
Content-type: application/json
Content-length: 573

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "virtualNetwork": "Virtual Network value",
  "manufacturer": "Manufacturer value",
  "deviceCount": 11,
  "cloudPcRoundTripTime": 6.666666666666667,
  "cloudPcSignInTime": 5.666666666666667,
  "remoteSignInTime": 5.333333333333333,
  "coreBootTime": 4.0,
  "coreSignInTime": 4.666666666666667,
  "cloudPcFailurePercentage": 8.0,
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 622

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
  "id": "9ecbcf80-cf80-9ecb-80cf-cb9e80cfcb9e",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "virtualNetwork": "Virtual Network value",
  "manufacturer": "Manufacturer value",
  "deviceCount": 11,
  "cloudPcRoundTripTime": 6.666666666666667,
  "cloudPcSignInTime": 5.666666666666667,
  "remoteSignInTime": 5.333333333333333,
  "coreBootTime": 4.0,
  "coreSignInTime": 4.666666666666667,
  "cloudPcFailurePercentage": 8.0,
  "userPrincipalName": "User Principal Name value"
}
```




