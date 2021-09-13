---
title: Ação reportRemoteAssistance
description: Uma chamada post para enviar a carga de relatórios
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40be075dca577bb1febbeb68390fccb51dbeb0be
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59041448"
---
# <a name="reportremoteassistance-action"></a>Ação reportRemoteAssistance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma chamada post para enviar a carga de relatórios

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reportRemoteAssistance
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
|reportingPayload|[remoteAssistanceReporting](../resources/intune-remoteassistance-remoteassistancereporting.md)|Ainda não documentado|



## <a name="response"></a>Resposta
Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reportRemoteAssistance

Content-type: application/json
Content-length: 972

{
  "reportingPayload": {
    "@odata.type": "microsoft.graph.remoteAssistanceReporting",
    "id": "Id value",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
    "remoteAssistanceSessionType": "fullControl",
    "helperEmail": "Helper Email value",
    "helperTenantId": "Helper Tenant Id value",
    "helperFirstName": "Helper First Name value",
    "helperLastName": "Helper Last Name value",
    "helperDeviceAadId": "Helper Device Aad Id value",
    "helperDeviceName": "Helper Device Name value",
    "helperEnrollmentState": "enrolled",
    "sharerEmail": "Sharer Email value",
    "sharerTenantId": "Sharer Tenant Id value",
    "sharerFirstName": "Sharer First Name value",
    "sharerLastName": "Sharer Last Name value",
    "sharerDeviceAadId": "Sharer Device Aad Id value",
    "sharerDeviceName": "Sharer Device Name value",
    "sharerEnrollmentState": "enrolled"
  }
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 204 No Content
```



