---
title: Ação createServerLogCollectionRequest
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3497c47910f4616240b37b9dd5586def15a0ec57
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348268"
---
# <a name="createserverlogcollectionrequest-action"></a>Ação createServerLogCollectionRequest

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.Read.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.Read.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers/{microsoftTunnelServerId}/createServerLogCollectionRequest
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|startDateTime|DateTimeOffset|Ainda não documentado|
|endDateTime|DateTimeOffset|Ainda não documentado|



## <a name="response"></a>Resposta
Se tiver êxito, essa ação retornará um código de `200 OK` resposta e um [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers/{microsoftTunnelServerId}/createServerLogCollectionRequest

Content-type: application/json
Content-length: 115

{
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 481

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftTunnelServerLogCollectionResponse",
    "id": "05dcc2e9-c2e9-05dc-e9c2-dc05e9c2dc05",
    "status": "completed",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
    "sizeInBytes": 11,
    "serverId": "Server Id value",
    "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
    "expiryDateTime": "2017-01-01T00:03:32.5199332-08:00"
  }
}
```




