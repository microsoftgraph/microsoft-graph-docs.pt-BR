---
title: Obter hardwareConfigurationRunSummary
description: Leia propriedades e relações do objeto hardwareConfigurationRunSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c4ce6faae2c8d06513fdc3ba880adfdbdfd099c3
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345356"
---
# <a name="get-hardwareconfigurationrunsummary"></a>Obter hardwareConfigurationRunSummary

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Leia propriedades e relações do [objeto hardwareConfigurationRunSummary.](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/runSummary
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto hardwareConfigurationRunSummary](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/runSummary
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "value": {
    "@odata.type": "#microsoft.graph.hardwareConfigurationRunSummary",
    "id": "76b964f2-64f2-76b9-f264-b976f264b976",
    "successfulDeviceCount": 5,
    "failedDeviceCount": 1,
    "pendingDeviceCount": 2,
    "errorDeviceCount": 0,
    "notApplicableDeviceCount": 8,
    "unknownDeviceCount": 2,
    "successfulUserCount": 3,
    "failedUserCount": 15,
    "pendingUserCount": 0,
    "errorUserCount": 14,
    "notApplicableUserCount": 6,
    "unknownUserCount": 0,
    "lastRunDateTime": "2016-12-31T23:57:28.499537-08:00"
  }
}
```




