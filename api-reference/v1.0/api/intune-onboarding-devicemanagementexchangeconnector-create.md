---
title: Criar deviceManagementExchangeConnector
description: Crie um novo objeto deviceManagementExchangeConnector.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7ea05e8f7d787065b72ad05f53c7411180293ee2
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362495"
---
# <a name="create-devicemanagementexchangeconnector"></a>Criar deviceManagementExchangeConnector

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementExchangeConnector.

A tabela a seguir mostra as propriedades obrigatórias ao criar deviceManagementExchangeConnector.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Ainda não documentado|
|lastSyncDateTime|DateTimeOffset|Hora da última sincronização do Exchange Connector|
|status|[deviceManagementExchangeConnectorStatus](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|Status do Exchange Connector. Os valores possíveis são: `none`, `connectionPending`, `connected`, `disconnected`.|
|primarySmtpAddress|String|Endereço de email usado para configurar o serviço a serviço do Exchange Connector.|
|serverName|String|O nome do servidor Exchange.|
|connectorServerName|String|O nome do servidor que hospeda o Exchange Connector.|
|exchangeConnectorType|[deviceManagementExchangeConnectorType](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|O tipo de Exchange Connector configurado. Os valores possíveis são: `onPremises`, `hosted`, `serviceToService`, `dedicated`.|
|versão|String|A versão do ExchangeConnectorAgent|
|exchangeAlias|String|Um alias atribuído a um servidor Exchange|
|exchangeOrganization|Cadeia de caracteres|Organização do Exchange no servidor Exchange|



## <a name="response"></a>Resposta
Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
Content-type: application/json
Content-length: 490

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
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
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 539

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
```




