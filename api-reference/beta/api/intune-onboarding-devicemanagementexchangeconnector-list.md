---
title: Listar deviceManagementExchangeConnectors
description: Listar propriedades e relações de objeto de deviceManagementExchangeConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3ca8daf702d5a355a888d7d9e8b0585044ad113a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210952"
---
# <a name="list-devicemanagementexchangeconnectors"></a>Listar deviceManagementExchangeConnectors

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Listar propriedades e relações de objeto de [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 616

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
      "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "status": "connectionPending",
      "primarySmtpAddress": "Primary Smtp Address value",
      "serverName": "Server Name value",
      "connectorServerName": "Connector Server Name value",
      "exchangeConnectorType": "hosted",
      "version": "Version value",
      "exchangeAlias": "Exchange Alias value",
      "exchangeOrganization": "Exchange Organization value"
    }
  ]
}
```




