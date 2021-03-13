---
title: Criar temporaryAccessPassAuthenticationMethod
description: Crie um novo objeto temporaryAccessPassAuthenticationMethod.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 801f82d30baf5a231b0fea78c3613773d4dd8f53
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761090"
---
# <a name="create-temporaryaccesspassauthenticationmethod"></a>Criar temporaryAccessPassAuthenticationMethod
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) em um usuário. Um usuário só pode ter um Passe de Acesso Temporário. A senha pode ser usada entre a hora de início e término do Passe de Acesso Temporário. Se o usuário exigir um novo Passe de Acesso Temporário:
* Embora o Passe de Acesso Temporário atual seja válido – o administrador precisa excluir o Passe de Acesso Temporário existente e criar uma nova passagem no usuário. Excluir um Passe de Acesso Temporário válido revoga as sessões do usuário. 
* Depois que o Passe de Acesso Temporário tiver expirado – uma nova passagem de acesso temporário substitui o passe de acesso temporário atual e não revoga as sessões do usuário.


## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

### <a name="permissions-acting-on-self"></a>Permissões agindo em si mesmo

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:---------------------------------------|:-------------------------|
| Delegado (conta corporativa ou de estudante)     | UserAuthenticationMethod.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

### <a name="permissions-acting-on-other-users"></a>Permissões atuando em outros usuários

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:---------------------------------------|:-------------------------|
| Delegado (conta corporativa ou de estudante)     | UserAuthenticationMethod.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Application                            | UserAuthenticationMethod.ReadWrite.All |

Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)
* Administração global
* Administrador de autenticação privilegiada
* Administrador de autenticação

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto temporaryAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)

A tabela a seguir descreve propriedades opcionais que podem ser usadas ao criar [o temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md).

|Propriedade|Tipo|Descrição|Obrigatório| 
|:---|:---|:---|:---|
|startDateTime|DateTimeOffset|A data e a hora em que o temporaryAccessPass fica disponível para uso, se não definir o Passe de Acesso Temporário estará disponível para uso no momento da criação.| Não|
|lifetimeInMinutes|Int32|O tempo de vida do temporaryAccessPass em minutos começando na hora da criação ou em startDateTime, se definido. Mínimo 10, Máximo 43200 (equivalente a 30 dias).| Não|
|isUsableOnce|Boolean|Determina se a passagem está limitada a um uso único. Se True – o passe pode ser usado uma vez, se False – o passe pode ser usado várias vezes dentro do tempo de vida temporaryAccessPass. Um Passe de Acesso Temporário com vários usos (isUsableOnce = false), só poderá ser criado e usado para entrar se for permitido pela política de método Autenticação de Passagem de Acesso Temporário.|  Não|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_temporaryaccesspassauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods
Content-Type: application/json
Content-length: 209

{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "startDateTime": "2021-01-26T00:00:00.000Z",
  "lifetimeInMinutes": 60,
  "isUsableOnce": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-temporaryaccesspassauthenticationmethod-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-temporaryaccesspassauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-temporaryaccesspassauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-temporaryaccesspassauthenticationmethod-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
    "id": "81757535-e21e-4330-a338-33b8038ff12b",
    "temporaryAccessPass": "nc+&G=xwDKCz",
    "createdDateTime": "2021-01-25T23:53:35.5026721Z",
    "startDateTime": "2021-01-26T00:00:00Z",
    "lifetimeInMinutes": 60,
    "isUsableOnce": false,
    "isUsable": false,
    "methodUsabilityReason": "NotYetValid"

}
```
