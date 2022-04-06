---
title: 'servicePrincipal: addKey'
description: Adicione uma credencial de chave a uma servicePrincipal.
ms.localizationpriority: medium
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 0fbeb8479463fd52c2cbbf041ba24470ae2d7307
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2022
ms.locfileid: "63671661"
---
# <a name="serviceprincipal-addkey"></a>servicePrincipal: addKey

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Adiciona uma credencial de chave a [um servicePrincipal](../resources/serviceprincipal.md). Esse método juntamente com [removeKey](serviceprincipal-removekey.md) pode ser usado por um servicePrincipal para automatizar a rolagem de suas chaves expiradas.

> [!NOTE]
> [Criar servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) e [Atualizar service As operaçõesPrincipal](../api/serviceprincipal-update.md) podem continuar a ser usadas para adicionar e atualizar credenciais de chave para qualquer servicePrincipal com ou sem o contexto de um usuário.

Como parte da validação de solicitação para esse método, uma prova de posse de uma chave existente é verificada antes que a ação possa ser executada. 

ServicePrincipals que não têm certificados válidos existentes (ou seja: nenhum certificado foi adicionado ainda, ou todos os certificados expiraram), não poderão usar essa ação de serviço. [Atualizar servicePrincipal](../api/serviceprincipal-update.md) pode ser usado para executar uma atualização.

## <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Application.ReadWrite.All, Directory.ReadWrite.All   |
|Delegado (conta pessoal da Microsoft) | Nenhum.    |
|Aplicativo | Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All |


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
| keyCredential | [keyCredential](../resources/keycredential.md) | A nova credencial de chave servicePrincipal a ser acrescentada. O __tipo__, __o uso__ __e a chave__ são propriedades necessárias para esse uso. Os tipos de chave com suporte são:<br><ul><li>`AsymmetricX509Cert`: O uso deve ser `Verify`.</li><li>`X509CertAndPassword`: O uso deve ser `Sign`</li></ul>|
| passwordCredential | [passwordCredential](../resources/passwordcredential.md) | Somente __secretText__ é necessário para ser definido que deve conter a senha da chave. Essa propriedade é necessária apenas para chaves do tipo `X509CertAndPassword`. De defini-lo como `null` caso contrário.|
| proof | String | Um token JWT auto-assinado usado como prova de posse das chaves existentes. Esse token JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes do servicePrincipal. O token deve conter os seguintes argumentos:<ul><li>`aud` – A audiência deve ser `00000002-0000-0000-c000-000000000000`.</li><li>`iss` - O emissor precisa ser __a id__  do servicePrincipal que está fazendo a chamada.</li><li>`nbf` – Não antes da hora.</li><li>`exp` - O tempo de expiração deve ser `nbf` + 10 minutos.</li></ul><br>Para etapas para gerar essa prova de token de posse, consulte [Generating proof of possess tokens for rolling keys](/graph/application-rollkey-prooftoken).|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo [objeto keyCredential](../resources/keycredential.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-adding-a-new-key-credential-to-a-serviceprincipal"></a>Exemplo 1: Adicionando uma nova credencial de chave a um servicePrincipal

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey_1"
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
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addkey-1-javascript-snippets.md)]
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

### <a name="example-2-adding-a-key-credential-and-an-associated-password-for-the-key"></a>Exemplo 2: Adicionar uma credencial de chave e uma senha associada à chave

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey_2"
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
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addkey-2-javascript-snippets.md)]
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



