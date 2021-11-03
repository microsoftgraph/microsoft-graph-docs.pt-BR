---
title: Criar federatedIdentityCredential
description: Crie um novo objeto federatedIdentityCredential para um aplicativo.
author: kjyam98
ms.localizationpriority: medium
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: e1c32bb1429f048558443b0ed312c5130c036103
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689193"
---
# <a name="create-federatedidentitycredential"></a>Criar federatedIdentityCredential
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto federatedIdentityCredential](../resources/federatedidentitycredential.md) para um aplicativo. Ao configurar uma relação de confiança entre seu registro de aplicativo do Azure AD e o provedor de identidade para [sua](/azure/active-directory/develop/workload-identity-federation-create-trust) plataforma de computação, você pode usar tokens emitidos por essa plataforma para autenticar com plataforma de identidade da Microsoft e chamar APIs no ecossistema da Microsoft. No máximo 20 objetos podem ser adicionados a um aplicativo.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Application.ReadWrite.All    |
|Delegada (conta pessoal da Microsoft) |  Application.ReadWrite.All |
|Aplicativo | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /applications/{applicationsId}/federatedIdentityCredentials
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto federatedIdentityCredential.](../resources/federatedidentitycredential.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [federatedIdentityCredential](../resources/federatedidentitycredential.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|audiences|Coleção de cadeias de caracteres|Lista as audiências que podem aparecer no token externo. Esse campo é obrigatório e é padrão para "api://AzureADTokenExchange". Ele diz o plataforma de identidade da Microsoft deve aceitar na `aud` declaração no token de entrada. Esse valor representa o Azure AD em seu provedor de identidade externo e não tem valor fixo entre provedores de identidade - talvez seja necessário criar um novo registro de aplicativo em seu provedor de identidade para servir como audiência desse token. Obrigatório.|
|emissor|String|TThe URL of the external identity provider and must match the issuer claim of the external token being exchanged. A combinação dos valores de **emissor** e **assunto** deve ser exclusiva no aplicativo. Obrigatório.|
|name|String|O identificador exclusivo da credencial de identidade federada, que tem um limite de caracteres de 120 caracteres e deve ser amigável à URL. É imutável uma vez criado|
|assunto|String|Obrigatório. O identificador da carga de trabalho de software externo no provedor de identidade externa. Como o valor da audiência, ele não tem formato fixo, pois cada provedor de identidade usa seu próprio - às vezes um GUID, às vezes um identificador delimitado por dois pontos, às vezes cadeias de caracteres arbitrárias. O valor aqui deve corresponder à subclatura dentro do token apresentado ao Azure AD. A combinação de **emissor e** **assunto** deve ser exclusiva no aplicativo.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto federatedIdentityCredential](../resources/federatedidentitycredential.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_federatedidentitycredential_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/applications/bcd7c908-1c4d-4d48-93ee-ff38349a75c8/federatedIdentityCredentials/
Content-Type: application/json

{
    "name": "testing02",
    "issuer": "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0",
    "subject": "a7d388c3-5e3f-4959-ac7d-786b3383006a",
    "audiences": [
        "api://AzureADTokenExchange"
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-federatedidentitycredential-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-federatedidentitycredential-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-federatedidentitycredential-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-federatedidentitycredential-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.federatedIdentityCredential"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications('bcd7c908-1c4d-4d48-93ee-ff38349a75c8')/federatedIdentityCredentials/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/directoryObjects/$/Microsoft.DirectoryServices.Application('bcd7c908-1c4d-4d48-93ee-ff38349a75c8')/federatedIdentityCredentials/d9b7bf1e-429e-4678-8132-9b00c9846cc4",
    "id": "d9b7bf1e-429e-4678-8132-9b00c9846cc4",
    "name": "testing02",
    "issuer": "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0",
    "subject": "a7d388c3-5e3f-4959-ac7d-786b3383006a",
    "description": null,
    "audiences": [
        "api://AzureADTokenExchange"
    ]
}
```

