---
title: função getAllowedRemoteAssistanceActions
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6532e534624e9598beeb79669e882debb5d14089
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61343403"
---
# <a name="getallowedremoteassistanceactions-function"></a>função getAllowedRemoteAssistanceActions

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

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
GET /deviceManagement/getAllowedRemoteAssistanceActions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.
A tabela a seguir mostra os parâmetros que podem ser usados com esta função.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|sharerAadDeviceId|String|Ainda não documentado|
|sharerDeviceIntuneMDMEnrolled|Booliano|Ainda não documentado|
|sharerId|String|Ainda não documentado|
|sharerTenantId|String|Ainda não documentado|



## <a name="response"></a>Resposta
Se tiver êxito, essa função retornará um código `200 OK` de resposta e um [allowedRemoteAssistanceActions](../resources/intune-remoteassistance-allowedremoteassistanceactions.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAllowedRemoteAssistanceActions(sharerAadDeviceId='parameterValue',sharerDeviceIntuneMDMEnrolled=True,sharerId='parameterValue',sharerTenantId='parameterValue')
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 34

{
  "value": "takeFullControl"
}
```




