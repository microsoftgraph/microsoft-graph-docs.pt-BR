---
title: Introdução à API dos métodos de autenticação do Microsoft Graph
description: A API dos métodos de autenticação do Microsoft Graph oferece às organizações a capacidade de gerenciar programaticamente os métodos de autenticação dos usuários, registrando os usuários para autenticação multifator (MFA) e redefinição de senha de autoatendimento (SSPR).
author: mmcla
localization_priority: Priority
ms.prod: identity-and-sign-in
ms.openlocfilehash: 8750f56db54c1dd5c2ef8708ccd1f3b873c9ea0328517743b881f7502f299f89
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251656"
---
# <a name="get-started-with-the-microsoft-graph-authentication-methods-api"></a>Introdução à API dos métodos de autenticação do Microsoft Graph

Os [métodos de autenticação](/azure/active-directory/authentication/concept-authentication-methods) são como os usuários se autenticam no Azure Active Directory (Azure AD). Os métodos de autenticação do Azure AD incluem senha e telefone (por exemplo, SMS e chamadas de voz), que hoje são gerenciáveis no Microsoft Graph, entre muitos outros, como chaves de segurança FIDO2 e o aplicativo Microsoft Authenticator. Os métodos de autenticação são usados nas autenticações primária, de segundo fator e de step-up. Além disso, no processo de redefinição de senha de autoatendimento (SSPR).

Você pode usar as APIs de método de autenticação para gerenciar os métodos de autenticação de um usuário. Por exemplo, você pode:

* Adicionar um número de telefone para um usuário, que pode usar esse número para SMS e autenticação de chamada de voz, se estiverem habilitados para o uso pela política
* Atualizar ou excluir o número de telefone atribuído a um usuário
* Habilitar ou desabilitar o número para entrada de SMS
* Redefinir a senha de um usuário

As APIs são uma ferramenta fundamental para gerenciar os métodos de autenticação dos usuários.

Neste tutorial, você aprenderá a:

> [!div class="checklist"]
> * Autenticar-se no Azure AD com as funções e permissões certas
> * Verificar os métodos de autenticação do usuário
> * Adicionar novos números de telefone para o usuário
> * Remover um número de telefone do usuário
> * Redefinir a senha do usuário

## <a name="step-1-authenticate-to-azure-ad-with-the-right-roles-and-permissions"></a>Etapa 1: Autenticar-se no Azure AD com as funções e permissões certas

Usando sua [ferramenta favorita para interagir com o Microsoft Graph](use-the-api.md#tools-for-interacting-with-microsoft-graph), entre usando uma conta com uma destas funções:

* Administrador global
* Administrador de autenticação privilegiada
* Administrador de autenticação

Em seguida, modifique suas permissões. Usaremos o [UserAuthenticationMethod.ReadWrite.All](permissions-reference.md#user-authentication-method-permissions-preview) para este tutorial, portanto, verifique se ele está habilitado no Graph Explorer ou no aplicativo.

Comece a usar a API após o escopo ser atribuído e aprovado. Os exemplos aqui usam um usuário padrão chamado de Avery Howard. Use uma conta de teste preexistente ou crie uma nova seguindo [estas instruções](/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user). Essas APIs estão ativas, portanto não as testem em usuários reais.

## <a name="step-2-check-the-users-authentication-methods"></a>Etapa 2: Verificar os métodos de autenticação do usuário

Faça uma chamada para verificar os métodos de autenticação do usuário. Pegue a URL para ver o perfil de um usuário e adicione `/authentication/methods`:

### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a>Resposta

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/methods",
    "value": [
        {
            "@odata.type": "#microsoft.graph.passwordAuthenticationMethod",
            "id": "28c10230-6103-485e-b985-444c60001490",
            "password": null,
            "creationDateTime": null
        }
    ]
}
```

## <a name="step-3-add-new-phone-numbers-for-the-user"></a>Etapa 3: Adicionar novos números de telefone para o usuário

Da etapa anterior, um novo usuário (Avery) tem apenas uma senha registrada. Para atribuir um novo número de telefone para o Avery usar, faça uma solicitação de `POST` com o tipo de telefone e número no corpo. Para informar ao sistema que um número de telefone está sendo adicionado, também será necessário alterar o final da URL de `methods` para `phoneMethods`.

### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
Content-Type: application/json
```

```json
{
    "phoneType": "mobile",
    "phoneNumber": "+1 2065550123"
}
```

### <a name="response"></a>Resposta

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "3179e48a-750b-4051-897c-87b9720928f7",
    "phoneNumber": "+1 2065550123",
    "phoneType": "mobile",
    "smsSignInState": "ready"
}
```

Para adicionar o número comercial do Avery, você vai `POST` novamente para a mesma URL, mas atualizará o número e o tipo de telefone:

### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
Content-Type: application/json
```

```json
{
    "phoneType": "office",
    "phoneNumber": "+1 4255550199"
}
```

### <a name="response"></a>Resposta

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc",
    "phoneNumber": "+1 4255550199",
    "phoneType": "office",
    "smsSignInState": "notSupported"
}
```

Faça mais um `GET` na URL de métodos de telefone para ver todos os números de telefone do Avery:

### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
```

### <a name="response"></a>Resposta

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods",
    "value": [
        {
            "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc",
            "phoneNumber": "+1 4255550199",
            "phoneType": "office",
            "smsSignInState": "notSupported"
        },
        {
            "id": "3179e48a-750b-4051-897c-87b9720928f7",
            "phoneNumber": "+1 2065550123",
            "phoneType": "mobile",
            "smsSignInState": "ready"
        }
    ]
}
```

Confirme se você consegue ver os dois números conforme o esperado.

## <a name="step-4-remove-a-phone-number-from-the-user"></a>Etapa 4: Remover um número de telefone do usuário

Neste cenário, o Avery agora está trabalhando em casa e você precisa remover o número comercial da conta. É necessário chamar `DELETE` na URL do telefone comercial, que pode ser criado anexando a ID do telefone comercial à URL de métodos de telefone. Veja acima a lista de telefones do Avery: a ID do telefone comercial começa com "e37f".

### <a name="request"></a>Solicitação

```http
DELETE https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods/e37fc753-ff3b-4958-9484-eaa9425c82bc
```

Não há dados na resposta porque não há mais telefone comercial, conforme o esperado. Confirme se ele desapareceu em todos os métodos do Avery, que é o mesmo `GET` feito anteriormente:

### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a>Resposta

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/methods",
    "value": [
        {
            "@odata.type": "#microsoft.graph.phoneAuthenticationMethod",
            "id": "3179e48a-750b-4051-897c-87b9720928f7",
            "phoneNumber": "+1 2065550123",
            "phoneType": "mobile",
            "smsSignInState": "ready"
        },
        {
            "@odata.type": "#microsoft.graph.passwordAuthenticationMethod",
            "id": "28c10230-6103-485e-b985-444c60001490",
            "password": null,
            "creationDateTime": null
        }
    ]
}
```

Como esperado, o usuário agora voltou a ter apenas um telefone celular e uma senha.

## <a name="step-5-reset-the-users-password"></a>Etapa 5: Redefinir senha do usuário

Neste cenário, o Avery esqueceu a senha e você precisa redefini-la. Para redefinir, você fará uma `POST` na URL da senha (veja acima a ID começando com "28c1" na lista de métodos de autenticação do Avery), especificando a ação "resetPassword". Forneça a nova senha no corpo da solicitação.

### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/passwordMethods/28c10230-6103-485e-b985-444c60001490/resetPassword
Content-Type: application/json
```

```json
{
    "newPassword": "29sdjfw#fajsdA_a_3an3223"
}
```

### <a name="response"></a>Resposta

``` http
Location: https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

Como isso está sincronizando a senha com o Active Directory na infraestrutura local do locatário, poderá levar alguns minutos, então você tem um endereço onde poderá verificar se está completo. Esse endereço está no cabeçalho do local da resposta e, para ver o status, faça um `GET` na URL.

### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

### <a name="response"></a>Resposta

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('ed178e23-7447-4892-baf8-fc46f8af26ce')/authentication/operations/$entity",
    "id": "74bfa1a6-c0e0-4957-8c37-f91048f4959e",
    "createdDateTime": "2020-05-14T00:23:40Z",
    "lastActionDateTime": "2020-05-14T00:23:41Z",
    "status": "succeeded",
    "statusDetail": "ResetSuccess",
    "resourceLocation": "https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/methods/28c10230-6103-485e-b985-444c60001490"
}
```

E sucesso! Você viu o perfil de um usuário, seus métodos de autenticação, como adicionar e remover números de telefone, e como redefinir senha. Agora, você está pronto para gerenciar os métodos dos seus usuários.

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para métodos de autenticação?

* Confira [Visão geral da API dos métodos de autenticação do Azure AD](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Próximas etapas

* Descubra como [usar as APIs REST do método de autenticação](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta).
* Use o Azure AD para se [autenticar](./auth/index.yml) no Microsoft Graph.
* Integre o [logon do Azure AD](https://azure.microsoft.com/develop/identity/signin/) ao seu aplicativo ou website.
* Confira o [Changelog](changelog.md) para obter informações sobre novidades nas APIs do Azure AD.
* Explore [exemplos](https://developer.microsoft.com/graph/graph/examples) para obter mais ideias sobre como usar o Microsoft Graph.