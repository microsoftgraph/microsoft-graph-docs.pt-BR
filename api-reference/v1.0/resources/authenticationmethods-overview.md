---
title: Visão geral da API de métodos de autenticação do Azure AD
description: Os métodos de autenticação são como os usuários autenticam no Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 2c6c69522bf78b6e20a09e6e1d8310565041f333
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335594"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Visão geral da API de métodos de autenticação do Azure AD

Namespace: microsoft.graph

[Os métodos de autenticação](/azure/active-directory/authentication/concept-authentication-methods) são as maneiras que os usuários autenticam no Azure Active Directory (AD). Os métodos de autenticação no Azure AD incluem senha e telefone (por exemplo, chamadas de SMS e voz), que são gerenciáveis no ponto de extremidade beta do Microsoft Graph hoje, entre muitas outras, como chaves de segurança FIDO2 e o aplicativo Microsoft Authenticator. Os métodos de autenticação são usados nas autenticações primária, de segundo fator e de step-up. Além disso, no processo de redefinição de senha de autoatendimento (SSPR).

As APIs do método de autenticação são usadas para gerenciar os métodos de autenticação de um usuário. Por exemplo:

* Você pode recuperar detalhes da Chave de Segurança FIDO2 de um usuário e excluí-la se o usuário tiver perdido a chave.
* Você pode recuperar detalhes do registro de Microsoft Authenticator usuário e excluí-lo se o usuário tiver perdido o telefone.

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>Quais métodos de autenticação podem ser gerenciados no Microsoft Graph?

|Método de autenticação       | Descrição |Exemplos     |
|:---------------------------|:------------|:------------|
|[fido2AuthenticationMethod](fido2authenticationmethod.md)|Uma Chave de Segurança FIDO2 pode ser usada por um usuário para entrar no Azure AD.|Excluir uma chave de segurança FIDO2 perdida.|
|[microsoftAuthenticatorAuthenticationMethod](microsoftauthenticatorauthenticationmethod.md)|Microsoft Authenticator pode ser usado por um usuário para entrar ou executar a autenticação multifafação no Azure AD|Exclua um Microsoft Authenticator de autenticação.|
|[windowsHelloForBusinessAuthenticationMethod](windowsHelloForBusinessAuthenticationMethod.md)|Windows Hello for Business é um método de entrada sem senha em Windows dispositivos.|Consulte dispositivos em que um usuário habilitar Windows entrada hello for Business. Exclua uma Windows hello para empresas.|

Os métodos de autenticação a seguir ainda não são suportados no Microsoft Graph v1.0.

|Método de autenticação       | Descrição |Exemplos     |
|:---------------------------|:------------|:------------|
|Password | No momento, uma senha é o método de autenticação principal padrão no Azure AD.|Redefinir a senha de um usuário.|
|phoneAuthenticationMethod (ainda não suportado) |Um telefone pode ser usado por um usuário para autenticar usando SMS [ou](/azure/active-directory/authentication/concept-authentication-methods#phone-options) chamadas de voz (conforme permitido pela política).|Consulte os números de telefone de autenticação de um usuário. Adicionar, atualizar ou remover um número de telefone para um usuário. Habilitar ou desabilitar um telefone celular principal para SMS entrar.|
|Email |Um endereço de email pode ser usuário por um usuário como parte do processo Self-Service redefinição de senha (SSPR).|Consulte o endereço de email de autenticação de um usuário. Adicionar, atualizar ou remover um endereço de email para um usuário.|
|Passagem de Acesso Temporário |Passagem de Acesso Temporário é uma senha limitada por tempo que serve como uma credencial forte e permite a integração de credenciais sem senha. | Definir uma nova Passagem de Acesso Temporário em um usuário.|
|Token de hardware | Permitir que os usuários executem a autenticação multifator usando um dispositivo físico que fornece um código único. | Obter um token de hardware atribuído a um usuário.|
|Token de software | Permitir que os usuários executem a autenticação multifator usando um aplicativo que apoia a especificação DEM E fornece um código único. | Obter e excluir um token de software atribuído a um usuário.|
|Perguntas e respostas de segurança | Permitir que os usuários validem sua identidade ao executar uma redefinição de senha de autoatendida. |Excluir uma pergunta de segurança registrada por um usuário.|
|Método padrão | Representa o método que o usuário selecionou como padrão para executar a autenticação multifato.| Alterar o método MFA padrão de um usuário.|

## <a name="next-steps"></a>Próximas etapas

* Revise os tipos de método de autenticação e seus vários métodos.
* Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
