---
title: Listar chromeOSOnboardingSettingses
description: Listar propriedades e relações dos objetos chromeOSOnboardingSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b550aa89735123efee1e52a4c444f5300e27b219
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346525"
---
# <a name="list-chromeosonboardingsettingses"></a>Listar chromeOSOnboardingSettingses

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Listar propriedades e relações dos [objetos chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)

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
GET /deviceManagement/chromeOSOnboardingSettings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/chromeOSOnboardingSettings
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 408

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
      "id": "0344255d-255d-0344-5d25-44035d254403",
      "ownerUserPrincipalName": "Owner User Principal Name value",
      "onboardingStatus": "inprogress",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "lastDirectorySyncDateTime": "2016-12-31T23:57:56.1183185-08:00"
    }
  ]
}
```




