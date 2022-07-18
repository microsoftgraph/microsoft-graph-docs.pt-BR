---
title: Criar federatedIdentityCredential
description: Crie um novo objeto federatedIdentityCredential para um aplicativo.
author: shahzad-khalid
ms.localizationpriority: medium
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: b110f00734c7d7ad2044f289917713ad5d19887a
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602694"
---
# <a name="create-federatedidentitycredential"></a>Criar federatedIdentityCredential
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto federatedIdentityCredential](../resources/federatedidentitycredential.md) para um aplicativo. Ao [](/azure/active-directory/develop/workload-identity-federation-create-trust) configurar uma relação de confiança entre o registro do aplicativo Azure AD e o provedor de identidade para sua plataforma de computação, você pode usar tokens emitidos por essa plataforma para autenticar com plataforma de identidade da Microsoft e chamar APIs no ecossistema da Microsoft. Máximo de 20 objetos podem ser adicionados a um aplicativo.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Application.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) |  Application.ReadWrite.All |
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
No corpo da solicitação, forneça uma representação JSON do [objeto federatedIdentityCredential](../resources/federatedidentitycredential.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [o federatedIdentityCredential](../resources/federatedidentitycredential.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Público|Coleção de cadeias de caracteres|Lista as audiências que podem aparecer no token externo. Esse campo é obrigatório e usa como padrão "api://AzureADTokenExchange". Ele diz o plataforma de identidade da Microsoft deve aceitar na declaração `aud` no token de entrada. Esse valor representa Azure AD em seu provedor de identidade externo e não tem nenhum valor fixo entre provedores de identidade – talvez seja necessário criar um novo registro de aplicativo em seu provedor de identidade para servir como o público-alvo desse token. Obrigatório.|
|Emissor|String|A URL do provedor de identidade externa e deve corresponder à declaração do emissor do token externo que está sendo trocado. A combinação dos valores do **emissor e** **da entidade** deve ser exclusiva no aplicativo. Obrigatório.|
|nome|Cadeia de caracteres|O identificador exclusivo para a credencial de identidade federada, que tem um limite de caracteres de 120 caracteres e deve ser amigável para URL. Ele é imutável depois de criado|
|assunto|String|Obrigatório. O identificador da carga de trabalho de software externo no provedor de identidade externo. Como o valor do público-alvo, ele não tem nenhum formato fixo, pois cada provedor de identidade usa seu próprio – às vezes, um GUID, às vezes um identificador delimitado por dois-pontos, às vezes cadeias de caracteres arbitrárias. O valor aqui deve corresponder à sub declaração dentro do token apresentado Azure AD. A combinação de **emissor e** **assunto** deve ser exclusiva no aplicativo.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um [objeto federatedIdentityCredential](../resources/federatedidentitycredential.md) no corpo da resposta.

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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-federatedidentitycredential-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-federatedidentitycredential-from--powershell-snippets.md)]
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

