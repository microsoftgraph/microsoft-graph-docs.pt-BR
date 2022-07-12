---
title: Listar vppTokens
description: Lista propriedades e relações de objetos vppToken.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9249eda7e7c9bb7374400d92fd1013a8520e6873
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732741"
---
# <a name="list-vpptokens"></a>Listar vppTokens

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Lista propriedades e relações de objetos [vppToken](../resources/intune-onboarding-vpptoken.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 659

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.vppToken",
      "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
      "organizationName": "Organization Name value",
      "vppTokenAccountType": "education",
      "appleId": "Apple Id value",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "token": "Token value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "state": "valid",
      "lastSyncStatus": "inProgress",
      "automaticallyUpdateApps": true,
      "countryOrRegion": "Country Or Region value"
    }
  ]
}
```





