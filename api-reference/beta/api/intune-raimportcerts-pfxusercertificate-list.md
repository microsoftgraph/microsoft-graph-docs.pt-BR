---
title: Listar pfxUserCertificates
description: Listar propriedades e relações dos objetos pfxUserCertificate.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c60e0061ed642d41b3ca881cc6f540928a2b8fa
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59034152"
---
# <a name="list-pfxusercertificates"></a>Listar pfxUserCertificates

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Listar propriedades e relações dos objetos [pfxUserCertificate.](../resources/intune-raimportcerts-pfxusercertificate.md)

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
GET /pfxUserCertificates
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/pfxUserCertificates
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 894

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.pfxUserCertificate",
      "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
      "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
      "thumbprint": "Thumbprint value",
      "userUpn": "User Upn value",
      "encryptedPfxBlob": "Encrypted Pfx Blob value",
      "encryptedPfxPassword": "Encrypted Pfx Password value",
      "certStartDate": "2017-01-01T00:01:48.7697664-08:00",
      "certExpirationDate": "2016-12-31T23:56:39.3841403-08:00",
      "providerName": "Provider Name value",
      "encryptionKeyName": "Encryption Key Name value",
      "paddingScheme": 13,
      "status": 6,
      "intendedPurpose": 15,
      "createdTime": "2017-01-01T00:03:18.9597073-08:00",
      "isDeleted": true,
      "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
      "eTag": "ETag value"
    }
  ]
}
```



