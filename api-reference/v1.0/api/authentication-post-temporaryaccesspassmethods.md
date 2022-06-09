---
title: Criar temporaryAccessPassAuthenticationMethod
description: Crie um novo objeto temporaryAccessPassAuthenticationMethod para um usuário.
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5055f8631849b9942d6c47dad646b21ebeab4362
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971651"
---
# <a name="create-temporaryaccesspassauthenticationmethod"></a>Criar temporaryAccessPassAuthenticationMethod
Namespace: microsoft.graph

Crie um novo [objeto temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) em um usuário. Um usuário só pode ter uma Passagem de Acesso Temporária utilizável dentro do tempo de vida especificado. Se o usuário exigir uma nova Passagem de Acesso Temporária enquanto a senha de acesso temporária atual for válida, o administrador poderá criar uma nova Passagem de Acesso Temporária para o usuário, a passagem de acesso temporária anterior será excluída e uma nova Passagem de Acesso Temporária será criada.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

### <a name="permissions-acting-on-other-users"></a>Permissões que atuam em outros usuários

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:---------------------------------------|:-------------------------|
| Delegada (conta corporativa ou de estudante)     | UserAuthenticationMethod.ReadWrite.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | UserAuthenticationMethod.ReadWrite.All |

Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes funções do [Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):
* Administrador global
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
No corpo da solicitação, forneça uma representação JSON do objeto [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) .

A tabela a seguir descreve as propriedades opcionais que podem ser usadas ao criar [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isUsableOnce|Booleano|Opcional. Determina se a passagem está limitada a um uso único. If `true`, the pass can be used once; if `false`, the pass can be used multiple times within its **lifetimeInMinutes** setting. Uma Passagem de Acesso Temporário de vários usos (`isUsableOnce = false`) só poderá ser criada e usada para entrar se for permitida pela política de método de autenticação de Passagem  [de Acesso Temporário](../resources/temporaryaccesspassauthenticationmethodconfiguration.md).|
|lifetimeInMinutes|Int32|Opcional. O tempo de vida do temporaryAccessPass em minutos, começando na hora de criação ou em startDateTime, se definido. Deve estar entre 10 e 43200 (equivalente a 30 dias). Se não for especificado, a **configuração defaultLifetimeInMinutes** na política de método de autenticação de Passagem de [Acesso](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) Temporário será aplicada. |
|startDateTime|DateTimeOffset|Opcional. A data e a hora em que o temporaryAccessPass fica disponível para uso. Se não for especificado, a Passagem de Acesso Temporária estará disponível para uso imediatamente após sua criação.| 

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_temporaryaccesspassauthenticationmethod_from_"
}
-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/users/071cc716-8147-4397-a5ba-b2105951cc0b/authentication/temporaryAccessPassMethods
Content-Type: application/json

{
    "startDateTime": "2022-06-05T00:00:00.000Z",
    "lifetimeInMinutes": 60,
    "isUsableOnce": false
}
```

### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
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
    "id": "6f1967b7-15e8-4935-ac26-d50770ed07a7",
    "temporaryAccessPass": "+drkzqAD",
    "createdDateTime": "2022-06-02T16:21:09.765173Z",
    "startDateTime": "2022-06-05T00:00:00Z",
    "lifetimeInMinutes": 60,
    "isUsableOnce": false,
    "isUsable": false,
    "methodUsabilityReason": "NotYetValid"
}
```
