---
title: Listar windowsQualityUpdateProfiles
description: Listar propriedades e relações dos objetos windowsQualityUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a78f5fdb16a74b2aaeb7cb3f70542ad18d36fcb9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788251"
---
# <a name="list-windowsqualityupdateprofiles"></a>Listar windowsQualityUpdateProfiles

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Listar propriedades e relações dos objetos [windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsQualityUpdateProfiles
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 827

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsQualityUpdateProfile",
      "id": "76fc7b65-7b65-76fc-657b-fc76657bfc76",
      "displayName": "Display Name value",
      "description": "Description value",
      "expeditedUpdateSettings": {
        "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings",
        "qualityUpdateRelease": "Quality Update Release value",
        "daysUntilForcedReboot": 5
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "releaseDateDisplayName": "Release Date Display Name value",
      "deployableContentDisplayName": "Deployable Content Display Name value"
    }
  ]
}
```



