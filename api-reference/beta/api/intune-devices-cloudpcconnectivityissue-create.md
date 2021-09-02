---
title: Criar cloudPCConnectivityIssue
description: Crie um novo objeto cloudPCConnectivityIssue.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b5fae204dc8969dd1cb1507102b33353742bdf4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58801301"
---
# <a name="create-cloudpcconnectivityissue"></a>Criar cloudPCConnectivityIssue

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cloudPCConnectivityIssues
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto cloudPCConnectivityIssue.

A tabela a seguir mostra as propriedades necessárias ao criar o cloudPCConnectivityIssue.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo da entidade de evento de problema de conectividade de análise de experiência do usuário.|
|deviceId|Cadeia de caracteres|O DeviceId do Intune do dispositivo ao que a conexão está associada.|
|errorCode|Cadeia de caracteres|O código de erro do problema de conectividade.|
|errorDateTime|DateTimeOffset|A hora em que a conexão foi iniciada. O tempo é mostrado no formato ISO 8601 e hora UTC (Tempo Universal Coordenado).|
|userId|Cadeia de caracteres|A ID exclusiva do usuário que inicializa a conexão.|
|errorDescription|Cadeia de caracteres|A descrição detalhada do que deu errado.|
|recommendedAction|Cadeia de caracteres|A ação recomendada para corrigir o erro correspondente.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cloudPCConnectivityIssues
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
  "deviceId": "Device Id value",
  "errorCode": "Error Code value",
  "errorDateTime": "2016-12-31T23:58:20.6032957-08:00",
  "userId": "User Id value",
  "errorDescription": "Error Description value",
  "recommendedAction": "Recommended Action value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 374

{
  "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
  "id": "e8e2bf5f-bf5f-e8e2-5fbf-e2e85fbfe2e8",
  "deviceId": "Device Id value",
  "errorCode": "Error Code value",
  "errorDateTime": "2016-12-31T23:58:20.6032957-08:00",
  "userId": "User Id value",
  "errorDescription": "Error Description value",
  "recommendedAction": "Recommended Action value"
}
```



