---
title: Introdução à API dos métodos de autenticação do Microsoft Graph
description: A API de métodos de autenticação no Microsoft Graph oferece às organizações a capacidade de gerenciar programaticamente os métodos de autenticação de seus usuários, obtendo aos usuários registrados para fazer a autenticação multifator (MFA) e redefinição de senha de autoatendimento (SSPR).
author: mmcla
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8f08ae59f7a2ad0e16c4fc0c3af5637bcbfaaca
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272805"
---
# <a name="get-started-with-the-microsoft-graph-authentication-methods-api"></a>Introdução à API dos métodos de autenticação do Microsoft Graph

Os [métodos de autenticação](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) são as maneiras como os usuários são autenticados no Azure Active Directory (Azure AD). Os métodos de autenticação no Azure AD incluem senha e telefone (por exemplo, SMS e chamadas de voz), que podem ser gerenciados no Microsoft Graph hoje, entre muitas outras, como chaves de segurança do FIDO2 e o aplicativo Microsoft Authenticator. Os métodos de autenticação são usados na autenticação principal, de segundo fator e de etapa e também no processo de redefinição de senha de autoatendimento (SSPR).

Você pode usar as APIs do método de autenticação para gerenciar os métodos de autenticação de um usuário. Por exemplo, você pode:

* Adicionar um número de telefone para um usuário, que pode usar esse número para autenticação de SMS e de chamada de voz, se estiverem habilitados para usá-lo por política
* Atualizar ou excluir o número de telefone atribuído a um usuário
* Habilitar ou desabilitar o número para entrada do SMS
* Redefinir a senha de um usuário

As APIs são uma ferramenta principal para gerenciar os métodos de autenticação dos seus usuários.

Neste tutorial, você aprenderá a:

> [!div class="checklist"]
> * Autenticar no Azure AD com as funções e permissões corretas
> * Verificar os métodos de autenticação do usuário
> * Adicionar novos números de telefone para o usuário
> * Remover um número de telefone do usuário
> * Redefinir a senha do usuário

## <a name="step-1-authenticate-to-azure-ad-with-the-right-roles-and-permissions"></a>Etapa 1: autenticar no Azure AD com as funções e permissões corretas

Usando sua [ferramenta favorita para interagir com o Microsoft Graph](use-the-api.md#tools-for-interacting-with-microsoft-graph), entre usando uma conta com uma destas funções:

* Administrador global
* Administrador de autenticação privilegiada
* Administrador de Autenticação

Em seguida, modifique suas permissões. Usaremos [UserAuthenticationMethod. ReadWrite. All](permissions-reference.md#user-authentication-method-permissions-preview) para este tutorial, portanto, certifique-se de que ele esteja habilitado no explorador do Graph ou em seu aplicativo.

Depois que o escopo for atribuído e conenviado, você poderá começar a usar a API. Os exemplos aqui usam um usuário padrão chamado Avery Howard. Você deve usar uma conta de teste preexistente ou criar uma nova, seguindo [estas instruções](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user). Essas APIs estão ativas, portanto, não as testem em usuários reais.

## <a name="step-2-check-the-users-authentication-methods"></a>Etapa 2: verificar os métodos de autenticação do usuário

Faça uma chamada para ver os métodos de autenticação do usuário. Pegue a URL para ver o perfil de um usuário e adicionar `/authentication/methods` :

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

## <a name="step-3-add-new-phone-numbers-for-the-user"></a>Etapa 3: adicionar novos números de telefone para o usuário

Na etapa anterior, um novo usuário (Avery) tem apenas uma senha registrada. Para atribuir um novo número de telefone para uso da Avery, faça uma `POST` solicitação com o tipo de telefone e o número no corpo. Para informar ao sistema que um número de telefone está sendo adicionado, você também precisará alterar o final da URL de `methods` para `phoneMethods` .

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

Para adicionar o número de escritório da Avery, você irá `POST` novamente para a mesma URL, mas atualizará o tipo e o número de telefone:

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

Faça mais uma `GET` a URL dos métodos de telefone para ver todos os números de telefone da Avery:

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

Confirme que você pode ver os dois números conforme o esperado.

## <a name="step-4-remove-a-phone-number-from-the-user"></a>Etapa 4: remover um número de telefone do usuário

Neste cenário, a Avery agora está trabalhando em casa, você precisa remover o número do escritório de sua conta. Você precisará chamar `DELETE` a URL do telefone do Office, que você pode criar acrescentando a ID do telefone do escritório à URL dos métodos de telefone. Examine a lista de telefones da Avery acima: a ID do telefone do escritório começa com "e37f".

### <a name="request"></a>Solicitação

```http
DELETE https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods/e37fc753-ff3b-4958-9484-eaa9425c82bc
```

Não há dados na resposta porque não há mais telefone comercial conforme o esperado. Você pode confirmar se ele está examinando todos os métodos da Avery, que é o mesmo `GET` que foi feito anteriormente:

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

Como esperado, o usuário agora volta para ter apenas um telefone celular e uma senha.

## <a name="step-5-reset-the-users-password"></a>Etapa 5: redefinir a senha do usuário

Neste cenário, a Avery esqueceu a senha e você precisa redefini-la para elas. Para redefinir, você irá criar a `POST` URL de sua senha (consulte a ID que começa com "28c1" acima na lista de métodos de autenticação da Avery), especificando a ação "resetPassword". Forneça a nova senha no corpo da solicitação.

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

```
Location: https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

Como isso está sincronizando a senha para o Active Directory na infraestrutura local do locatário, pode levar alguns minutos, para que você tenha um endereço onde você pode verificar se está completo. Esse endereço está no cabeçalho de local da resposta e para ver o status da `GET` URL.

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

E sucesso! Você viu ver o perfil de um usuário, seus métodos de autenticação, adicionar e remover números de telefone e redefinir sua senha. Agora você está pronto para gerenciar os métodos de seus próprios usuários.

## <a name="api-reference"></a>Referência da API

Procurando a referência de API para métodos de autenticação?

* Consulte [visão geral da API de métodos de autenticação do Azure ad](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Próximas etapas

* Descubra como [usar as APIs REST do método de autenticação](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta).
* Use o Azure AD para se [autenticar](/graph/auth) no Microsoft Graph.
* Integre o [logon do Azure AD](https://azure.microsoft.com/develop/identity/signin/) ao seu aplicativo ou website.
* Confira o [Changelog](changelog.md) para obter informações sobre novidades nas APIs do Azure AD.
* Explore [exemplos](https://developer.microsoft.com/graph/graph/examples) para obter mais ideias sobre como usar o Microsoft Graph.
