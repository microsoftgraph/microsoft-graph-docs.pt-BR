---
title: 'servicePrincipal: addTokenSigningCertificate'
description: Adicione um certificado de assinatura a um servicePrincipal.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 951bd3ecbc65e8778809f5fac149e1ab59a258d3
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202507"
---
# <a name="serviceprincipal-addtokensigningcertificate"></a>servicePrincipal: addTokenSigningCertificate

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Cria um certificado de assinatura auto-assinado e retorna um [selfSignedCertificate](../resources/selfsignedcertificate.md), que é a parte pública do certificado gerado. O certificado de assinatura auto-assinado é composto por esses recursos: a chave privada ([keyCredential](../resources/keycredential.md) com uso = 'Sign'), a chave pública ([keyCredential](../resources/keycredential.md) com uso = 'verify') e [a passwordCredential](../resources/passwordcredential.md). Todos os recursos criados têm o **mesmo customKeyIdentifier**.

A **senhaCredential** é usada para abrir a chave pfx/privada. Além disso, ele está associado ao privateKey ter a mesma **keyId**. O assunto do certificado é um valor constante. Ele não será afetado pelo **displayName opcional** fornecido na chamada POST. O **startDateTime** é definido para o mesmo horário em que o certificado é criado usando a ação. O **endDateTime** pode ter até três anos após a criação do certificado.

## <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Application.ReadWrite.All, Directory.ReadWrite.All |
|Delegada (conta pessoal da Microsoft) | Nenhum.    |
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
| endDateTime | DateTimeOffset |A data e a hora em que a credencial expira. Pode ser até 3 anos a partir da data em que o certificado é criado. Se não for fornecido, o padrão será de três anos a partir do momento da criação. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z' .|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um novo objeto [selfSignedCertificate](../resources/selfsignedcertificate.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addtokensigningcertificate"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/7c8d4399-b4bf-413a-8b6a-c577790cae7d/addTokenSigningCertificate
Content-type: application/json

{
    "displayName":"CN=customDisplayName",
    "endDateTime":"2024-01-25T00:00:00Z"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-addtokensigningcertificate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addtokensigningcertificate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-addtokensigningcertificate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-addtokensigningcertificate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



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
    "customKeyIdentifier": null,
    "displayName": "customDisplayName",
    "endDateTime": "2023-06-29T00:00:00Z",
    "key": null,
    "keyId": "b859fc29-969f-48b2-9a27-8399b69f441e",
    "startDateTime": "2020-06-29T00:00:00Z",
    "type": "AsymmetricX509Cert",
    "thumbprint":"QWESRTGFWQWEDSASDTGGSADASDWQW",
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
  "suppressions": [
    "Error: serviceprincipal_selfsignedcertificate:\r\n      Resource type was null or missing, so we assume there is no response to validate."
    ]
} -->

