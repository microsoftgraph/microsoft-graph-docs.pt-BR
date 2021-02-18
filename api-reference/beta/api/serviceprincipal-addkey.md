---
title: 'servicePrincipal: addKey'
description: Adicione uma credencial de chave a uma servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 1010f2a5e1a26f834eeeabc9bfe7946515a529bd
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292081"
---
# <a name="serviceprincipal-addkey"></a>servicePrincipal: addKey

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Adiciona uma credencial de chave a [um servicePrincipal](../resources/serviceprincipal.md). Esse método, [juntamente com removeKey,](serviceprincipal-removekey.md) pode ser usado por uma servicePrincipal para automatizar a rolagem de suas chaves expiradas.

> [!NOTE]
> [Criar operações servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) e [Update servicePrincipal](../api/serviceprincipal-update.md) podem continuar a ser usadas para adicionar e atualizar credenciais de chave para qualquer servicePrincipal com ou sem o contexto de um usuário.

Como parte da validação da solicitação para esse método, uma prova de posse de uma chave existente é verificada antes que a ação possa ser executada. 

ServicePrincipals que não têm certificados válidos existentes (ou seja, se nenhum certificado tiver sido adicionado ainda ou todos os certificados expiraram), não poderão usar essa ação de serviço. [Atualizar servicePrincipal](../api/serviceprincipal-update.md) pode ser usado para executar uma atualização.

## <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Nenhum.  |
|Delegado (conta pessoal da Microsoft) | Nenhum.    |
|Aplicativo | Nenhum. |

> [!NOTE]
> Uma servicePrincipal não precisa de nenhuma permissão específica para rolar suas próprias chaves.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addKey
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome           | Descrição                |
|:---------------|:---------------------------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type   | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça as seguintes propriedades necessárias.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| keyCredential | [keyCredential](../resources/keycredential.md) | A nova credencial de chave servicePrincipal a ser acrescentada. O __tipo__, __uso__ __e chave__ são propriedades necessárias para esse uso. Os tipos de chave com suporte são:<br><ul><li>`AsymmetricX509Cert`: o uso deve `Verify` ser.</li><li>`X509CertAndPassword`: o uso deve ser `Sign`</li></ul>|
| passwordCredential | [passwordCredential](../resources/passwordcredential.md) | Somente __secretText__ é necessário para ser definido que deve conter a senha da chave. Essa propriedade é necessária somente para chaves do tipo `X509CertAndPassword` . De definida como `null` caso contrário.|
| proof | String | Um token JWT auto-assinado usado como prova de posse das chaves existentes. Esse token JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes do servicePrincipal. O token deve conter os seguintes argumentos:<ul><li>`aud` – A audiência deve ser `00000002-0000-0000-c000-000000000000`.</li><li>`iss` - O emissor precisa ser a __ID__  do servicePrincipal que está fazendo a chamada.</li><li>`nbf` – Não antes da hora.</li><li>`exp` – O tempo de expiração deve ser "nbf" + 10 min.</li></ul><br>Aqui está um exemplo [de código](/graph/application-rollkey-prooftoken) que pode ser usado para gerar esse token de comprovação de posse.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `200 OK` de resposta e um novo objeto [keyCredential](../resources/keycredential.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-adding-a-new-key-credential-to-a-serviceprincipal"></a>Exemplo 1: Adicionando uma nova credencial de chave a uma servicePrincipal

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/addKey
Content-type: application/json

{
    "keyCredential": {
        "type": "AsymmetricX509Cert",
        "usage": "Verify",
        "key": "MIIDYDCCAki..."
    },
    "passwordCredential": null,
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addkey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.keyCredential"
}
```

### <a name="example-2-adding-a-key-credential-and-an-associated-password-for-the-key"></a>Exemplo 2: Adicionando uma credencial de chave e uma senha associada à chave

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/addKey
Content-type: application/json

{
    "keyCredential": {
        "type": "X509CertAndPassword",
        "usage": "Sign",
        "key": "MIIDYDCCAki..."
    },
    "passwordCredential": {
        "secretText": "MKTr0w1..."
    },
    "proof":"eyJ0eXAiOiJ..."
}
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.keyCredential"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: addKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->



