---
title: Atualizar zebraFotaConnector
description: Atualize as propriedades de um objeto zebraFotaConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f38c88548649d462747dd1df0aa56df23276a66d
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212964"
---
# <a name="update-zebrafotaconnector"></a>Atualizar zebraFotaConnector

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de um [objeto zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md) .

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
PATCH /deviceManagement/zebraFotaConnector
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [o zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID de ZebraFotaConnector.|
|estado|[zebraFotaConnectorState](../resources/intune-androidfotaservice-zebrafotaconnectorstate.md)|O estado do conector Zebra. Os valores possíveis são: `none`, `connected`, `disconnected`, `unknownFutureValue`.|
|enrollmentToken|Cadeia de Caracteres|Token de registro de locatário da Zebra. O token é usado para registrar dispositivos Zebra no Serviço FOTA por meio da configuração do aplicativo.|
|enrollmentAuthorizationUrl|Cadeia de Caracteres|Conclua a URL de autorização de registro de conta. Isso corresponde ao verification_uri_complete nas documentações da API zebra.|
|lastSyncDateTime|DateTimeOffset|Data e hora em que a conta foi sincronizada pela última vez com a Zebra|
|fotaAppsApproved|Boolean|Sinalizador que indica se os aplicativos FOTA (Firmware Over-the-Air) necessários foram aprovados.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/zebraFotaConnector
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.zebraFotaConnector",
  "state": "connected",
  "enrollmentToken": "Enrollment Token value",
  "enrollmentAuthorizationUrl": "https://example.com/enrollmentAuthorizationUrl/",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "fotaAppsApproved": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.zebraFotaConnector",
  "id": "2301310a-310a-2301-0a31-01230a310123",
  "state": "connected",
  "enrollmentToken": "Enrollment Token value",
  "enrollmentAuthorizationUrl": "https://example.com/enrollmentAuthorizationUrl/",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "fotaAppsApproved": true
}
```




