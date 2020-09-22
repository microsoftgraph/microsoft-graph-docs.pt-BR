---
title: Listar iosVppAppAssignedDeviceLicenses
description: Listar Propriedades e relações dos objetos iosVppAppAssignedDeviceLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eb3a6866c4bf16a078d01719257e6a7ec8e5bbd5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48012233"
---
# <a name="list-iosvppappassigneddevicelicenses"></a>Listar iosVppAppAssignedDeviceLicenses

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Listar Propriedades e relações dos objetos [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
      "id": "bed943d0-43d0-bed9-d043-d9bed043d9be",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "managedDeviceId": "Managed Device Id value",
      "deviceName": "Device Name value"
    }
  ]
}
```






