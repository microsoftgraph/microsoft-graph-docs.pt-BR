---
title: Listar comanagementEligibleDeviceEntity
description: Listar Propriedades e relações dos objetos comanagementEligibleDeviceEntity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 39d7a92c5914107cdd5ecfebb9b4b7948bc8b8b0
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636032"
---
# <a name="list-comanagementeligibledeviceentity"></a>Listar comanagementEligibleDeviceEntity

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Listar Propriedades e relações dos objetos comanagementEligibleDeviceEntity.

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/comanagementEligibleReports
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos comanagementEligibleDeviceEntity no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleReports
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1303

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.comanagementEligibleDeviceEntity",
      "id": "659554f2-54f2-6595-f254-9565f2549565",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "deviceType": "Device Type value",
      "clientRegistrationStatus": "Client Registration Status value",
      "ownerType": "Owner Type value",
      "managementAgents": "Management Agent value",
      "managementState": "Management State value",
      "referenceId": "Reference Id value",
      "mdmStatus": "MDM Status value",
      "osVersion": "OS Version value",
      "serialNumber": "Serial Number value",
      "manufacturer": "Manufacture value",
      "model": "Model value",
      "osDescription": "OS Description value",
      "entitySource": 1024,
      "userId": "User Id value",
      "upn": "UPN value",
      "userEmail": "User Email value",
      "userName": "User name value",
      "coManageEligibleStatus": "CO Manage Eligible Status value"
    }
  ]
}
```



