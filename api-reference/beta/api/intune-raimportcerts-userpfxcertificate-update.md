---
title: Atualizar userPFXCertificate
description: Atualiza as propriedades de um objeto userPFXCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8a010d0db6bf31089ae5bdd0cf6f59d3f1c4b13b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37189659"
---
# <a name="update-userpfxcertificate"></a>Atualizar userPFXCertificate

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualiza as propriedades de um objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo do certificado PFX.|
|identificação|String|Impressão digital SHA-1 do certificado PFX.|
|Da intendedpurpose|[userPfxIntendedPurpose](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|Finalidade do certificado do ponto de vista da implantação. Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.|
|userPrincipalName|String|Nome principal de usuário do certificado PFX.|
|startDateTime|DateTimeOffset|Data/hora de início da validade do certificado.|
|expirationDateTime|DateTimeOffset|Data/hora de validade do certificado.|
|providerName|String|Provedor de criptografia usado para criptografar este BLOB.|
|keyName|String|Nome da chave (dentro do provedor) usada para criptografar o blob.|
|paddingScheme|[userPfxPaddingScheme](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|Esquema de preenchimento usado pelo provedor durante a criptografia/descriptografia. Os possíveis valores são: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.|
|encryptedPfxBlob|Binária|Blob PFX criptografado.|
|encryptedPfxPassword|String|Senha PFX criptografada.|
|createdDateTime|DateTimeOffset|Data/hora em que este certificado PFX foi importado.|
|lastModifiedDateTime|DateTimeOffset|Data/hora em que este certificado PFX foi modificado pela última vez.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
Content-type: application/json
Content-length: 523

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "smimeEncryption",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "pkcs1",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 695

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "045c159b-159b-045c-9b15-5c049b155c04",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "smimeEncryption",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "pkcs1",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




