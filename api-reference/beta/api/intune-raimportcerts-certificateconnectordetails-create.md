---
title: Criar certificateConnectorDetails
description: Crie um novo objeto certificateConnectorDetails.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ec640219d77c991804f3ab5680c956a203df755f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111996"
---
# <a name="create-certificateconnectordetails"></a>Criar certificateConnectorDetails

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto certificateConnectorDetails.](../resources/intune-raimportcerts-certificateconnectordetails.md)

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
POST /deviceManagement/certificateConnectorDetails
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto certificateConnectorDetails.

A tabela a seguir mostra as propriedades que são necessárias ao criar o certificateConnectorDetails.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para este conjunto de ConnectorDetails.|
|connectorName|Cadeia de Caracteres|Nome do conector (definido durante o registro).|
|machineName|Cadeia de Caracteres|Nome do computador que hospeda esse serviço de conector.|
|enrollmentDateTime|DateTimeOffset|Data/hora em que esse conector foi inscrito.|
|lastCheckinDateTime|DateTimeOffset|Data/hora em que esse conector se conectou pela última vez ao serviço.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/certificateConnectorDetails
Content-type: application/json
Content-length: 278

{
  "@odata.type": "#microsoft.graph.certificateConnectorDetails",
  "connectorName": "Connector Name value",
  "machineName": "Machine Name value",
  "enrollmentDateTime": "2016-12-31T23:57:59.3726057-08:00",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 327

{
  "@odata.type": "#microsoft.graph.certificateConnectorDetails",
  "id": "104d7361-7361-104d-6173-4d1061734d10",
  "connectorName": "Connector Name value",
  "machineName": "Machine Name value",
  "enrollmentDateTime": "2016-12-31T23:57:59.3726057-08:00",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
}
```



