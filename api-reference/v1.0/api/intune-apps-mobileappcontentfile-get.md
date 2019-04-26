---
title: Acessar mobileAppContentFile
description: Leia as propriedades e as relações do objeto mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5eb3e1470853afd84e681b658ff268bcf8d12a2d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566084"
---
# <a name="get-mobileappcontentfile"></a>Acessar mobileAppContentFile

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Leia as propriedades e as relações do objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 491

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppContentFile",
    "azureStorageUri": "Azure Storage Uri value",
    "isCommitted": true,
    "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "name": "Name value",
    "size": 4,
    "sizeEncrypted": 13,
    "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
    "manifest": "bWFuaWZlc3Q=",
    "uploadState": "transientError"
  }
}
```



