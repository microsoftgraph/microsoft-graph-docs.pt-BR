---
title: Listar unmanagedDeviceDiscoveryTasks
description: Listar propriedades e relações dos objetos unmanagedDeviceDiscoveryTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d8f0ba52ca9302ff3580884f476852aa9e3195d6157929c0ba38cdb91bb5c1a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54151043"
---
# <a name="list-unmanageddevicediscoverytasks"></a>Listar unmanagedDeviceDiscoveryTasks

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Listar propriedades e relações dos [objetos unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1214

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.unmanagedDeviceDiscoveryTask",
      "id": "6caa2ba0-2ba0-6caa-a02b-aa6ca02baa6c",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
      "category": "advancedThreatProtection",
      "priority": "high",
      "creator": "Creator value",
      "creatorNotes": "Creator Notes value",
      "assignedTo": "Assigned To value",
      "status": "pending",
      "unmanagedDevices": [
        {
          "@odata.type": "microsoft.graph.unmanagedDevice",
          "os": "Os value",
          "osVersion": "Os Version value",
          "ipAddress": "Ip Address value",
          "deviceName": "Device Name value",
          "macAddress": "Mac Address value",
          "domain": "Domain value",
          "manufacturer": "Manufacturer value",
          "model": "Model value",
          "location": "Location value",
          "lastLoggedOnUser": "Last Logged On User value",
          "lastSeenDateTime": "2017-01-01T00:02:00.1006212-08:00"
        }
      ]
    }
  ]
}
```




