---
title: Visão geral da API de métodos de autenticação do Azure AD
description: Os métodos de autenticação são como os usuários autenticam no Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 314d1ab950924f1b8f315029c9a829958396d120
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135468"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Visão geral da API de métodos de autenticação do Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Os métodos de autenticação](/azure/active-directory/authentication/concept-authentication-methods) são as maneiras que os usuários autenticam no Azure Active Directory (AD). Os métodos de autenticação do Azure AD incluem senha e telefone (por exemplo, SMS e chamadas de voz), que hoje são gerenciáveis no Microsoft Graph, entre muitos outros, como chaves de segurança FIDO2 e o aplicativo Microsoft Authenticator. Os métodos de autenticação são usados nas autenticações primária, de segundo fator e de step-up. Além disso, no processo de redefinição de senha de autoatendimento (SSPR).

As APIs do método de autenticação são usadas para gerenciar os métodos de autenticação de um usuário. Por exemplo:

* Você pode adicionar um número de telefone a um usuário. Em seguida, o usuário poderá usar esse número de telefone para autenticação de SMS e chamada de voz se estiver habilitado para usá-lo por política.
* Você pode atualizar esse número ou excluí-lo do usuário.
* Você pode habilitar ou desabilitar o número de login por SMS.
* Você pode redefinir a senha de um usuário.
* Você pode recuperar detalhes da Chave de Segurança FIDO2 de um usuário e excluí-la se o usuário tiver perdido a chave.
* Você pode recuperar detalhes do registro do Microsoft Authenticator de um usuário e excluí-lo se o usuário tiver perdido o telefone.
* Você pode adicionar um endereço de email a um usuário. Em seguida, o usuário pode usar esse email como parte do processo Self-Service redefinição de senha (SSPR).
* Você pode atualizar esse email ou excluí-lo do usuário.

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>Quais métodos de autenticação podem ser gerenciados no Microsoft Graph?

|Método de autenticação       | Descrição |Exemplos     |
|:---------------------------|:------------|:------------|
|[passwordAuthenticationMethod](passwordauthenticationmethod.md)| Uma senha é atualmente o método de autenticação principal padrão no Azure AD.|Redefinir a senha de um usuário|
|[phoneAuthenticationMethod](phoneauthenticationmethod.md)|Um telefone pode ser usado por um usuário para autenticar usando SMS ou [chamadas de voz](/azure/active-directory/authentication/concept-authentication-methods#phone-options) (conforme permitido pela política).|Veja os números de telefone de autenticação de um usuário. Adicionar, atualizar ou remover um número de telefone para um usuário. Habilitar ou desabilitar um telefone celular principal para entrar por SMS.|
|[fido2AuthenticationMethod](fido2authenticationmethod.md)|Uma Chave de Segurança FIDO2 pode ser usada por um usuário para entrar no Azure AD.|Excluir uma chave de segurança FIDO2 perdida.|
|[microsoftAuthenticatorAuthenticationMethod](microsoftauthenticatorauthenticationmethod.md)|O Microsoft Authenticator pode ser usado por um usuário para entrar ou executar a autenticação multifatório no Azure AD|Exclua um método de autenticação do Microsoft Authenticator.|
|[passwordlessmicrosoftauthenticatorauthenticationmethod](passwordlessmicrosoftauthenticatorauthenticationmethod.md) (preterido)|O Acesso por Telefone sem Senha do Microsoft Authenticator pode ser usado por um usuário para entrar no Azure AD|Exclua um método de autenticação de login de telefone sem senha.|
|[emailAuthenticationMethod](emailauthenticationmethod.md)|Um endereço de email pode ser usuário por um usuário como parte do processo Self-Service redefinição de senha (SSPR).|Consulte o endereço de email de autenticação de um usuário. Adicionar, atualizar ou remover um endereço de email para um usuário.|
|[windowsHelloForBusinessAuthenticationMethod](windowsHelloForBusinessAuthenticationMethod.md)|O Windows Hello para Empresas é um método de entrada sem senha em dispositivos Windows.|Ver dispositivos em que um usuário habilitar a entrada do Windows Hello para Empresas. Exclua uma credencial do Windows Hello para Empresas.|

## <a name="next-steps"></a>Próximas etapas

* Revise os tipos de método de autenticação e seus diversos métodos.
* Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
