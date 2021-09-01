---
title: Listar windowsDriverUpdateInventories
description: Listar propriedades e relações dos objetos windowsDriverUpdateInventory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8da1556b2b38084fc1a9095a417d4277ab1b8d5a
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819014"
---
# <a name="list-windowsdriverupdateinventories"></a>Listar windowsDriverUpdateInventories

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Listar propriedades e relações dos [objetos windowsDriverUpdateInventory.](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}/driverInventories
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}/driverInventories
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 551

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDriverUpdateInventory",
      "id": "3b14b403-b403-3b14-03b4-143b03b4143b",
      "name": "Name value",
      "version": "Version value",
      "manufacturer": "Manufacturer value",
      "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
      "driverClass": "Driver Class value",
      "applicableDeviceCount": 5,
      "approvalStatus": "declined",
      "category": "previouslyApproved",
      "deployDateTime": "2017-01-01T00:01:14.7822152-08:00"
    }
  ]
}
```



