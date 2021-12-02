---
title: 'servicePrincipal: addTokenSigningCertificate'
description: Adicione um certificado de assinatura a um servicePrincipal.
ms.localizationpriority: medium
author: alamaral
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: e8e7faffc0580391a27dabe8e76c98841e3fa7cb
ms.sourcegitcommit: 3e2239e60b6dc53997b7d4356a20fc3d365d6238
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2021
ms.locfileid: "61266394"
---
# <a name="serviceprincipal-addtokensigningcertificate"></a>servicePrincipal: addTokenSigningCertificate

Namespace: microsoft.graph

Crie um certificado de assinatura auto-assinado e retorne um [objeto selfSignedCertificate,](../resources/selfsignedcertificate.md) que é a parte pública do certificado gerado. 

O certificado de assinatura auto-assinado é composto pelos seguintes objetos, que são adicionados ao [servicePrincipal](../resources/serviceprincipal.md): 
+ O [objeto keyCredentials](../resources/keycredential.md) com os seguintes objetos:
    + Um objeto de chave privada com **o uso** definido como `Sign` .
    + Um objeto de chave pública com **o uso** definido como `Verify` .
+ O [objeto passwordCredentials.](../resources/passwordcredential.md) 


Todos os objetos têm o mesmo valor **de customKeyIdentifier**.

A **passwordCredential** é usada para abrir o arquivo PFX (chave privada). Ele e o objeto de chave privada associado têm o mesmo valor de **keyId**. Quando definido durante a criação por meio da **propriedade displayName,** o assunto do certificado não pode ser atualizado. O **startDateTime** é definido para o mesmo horário em que o certificado é criado usando a ação. O **endDateTime** pode ter até três anos após a criação do certificado.

## <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Application.ReadWrite.All, Directory.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Nenhum.    |
|Aplicativo | Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All |


## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addTokenSigningCertificate
```

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça as seguintes propriedades necessárias.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| displayName | cadeia de caracteres | Nome amigável para a chave.  Ele deve começar com `CN=` .|
| endDateTime | DateTimeOffset |A data e a hora em que a credencial expira. Pode ser até 3 anos a partir da data em que o certificado é criado. Se não for fornecido, o padrão será de três anos a partir do momento da criação. O tipo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um novo objeto [selfSignedCertificate](../resources/selfsignedcertificate.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addtokensigningcertificate"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/004375c5-6e2e-4dec-95e3-626838cb9f80/addTokenSigningCertificate
Content-type: application/json

{
    "displayName":"CN=customDisplayName",
    "endDateTime":"2024-01-25T00:00:00Z"
}
```


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.selfSignedCertificate"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.selfSignedCertificate",
  "customKeyIdentifier": "2iD8ppbE+D6Kmu1ZvjM2jtQh88E=",
  "displayName": "CN=customDisplayName",
  "endDateTime": "2024-01-25T00:00:00Z",
  "key": "MIICuDCCAaCgAwIBAgIIYXJsNtL4oUMwDQYJKoZIhvcNAQEL...StP8s/w==",
  "keyId": "93bc223f-7235-4b9c-beea-d66847531c49",
  "startDateTime": "2021-05-05T18:38:51.8100763Z",
  "thumbprint": "DA20FCA696C4F83E8A9AED59BE33368ED421F3C1",
  "type": "AsymmetricX509Cert",
  "usage": "Verify"
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-01-15 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: selfSignedCertificate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
} -->

