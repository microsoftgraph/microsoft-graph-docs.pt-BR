---
title: Azure AD de API de métodos de autenticação do Azure AD
description: Os métodos de autenticação são como os usuários se autenticam Azure AD.
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 6e4cbf0a80eec6e9e74d0d217847e5d4edb458a1
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819759"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Azure AD de API de métodos de autenticação do Azure AD

Namespace: microsoft.graph

[Os métodos de autenticação](/azure/active-directory/authentication/concept-authentication-methods) são as maneiras pelas quais os usuários se autenticam no Azure Active Directory (AD). Os métodos de autenticação no Azure AD incluem senha e telefone (por exemplo, SMS e chamadas de voz), que atualmente podem ser gerenciados no ponto de extremidade beta do Microsoft Graph, entre muitos outros, como chaves de segurança FIDO2 e o aplicativo Microsoft Authenticator. Os métodos de autenticação são usados nas autenticações primária, de segundo fator e de step-up. Além disso, no processo de redefinição de senha de autoatendimento (SSPR).

As APIs de método de autenticação são usadas para gerenciar os métodos de autenticação de um usuário. Por exemplo:

* Você pode recuperar detalhes da Chave de Segurança FIDO2 de um usuário e excluí-la se o usuário tiver perdido a chave.
* Você pode recuperar detalhes do registro de Microsoft Authenticator usuário e excluí-lo se o usuário tiver perdido o telefone.

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>Quais métodos de autenticação podem ser gerenciados no Microsoft Graph?

|Método de autenticação       | Descrição |Exemplos     |
|:---------------------------|:------------|:------------|
|[fido2AuthenticationMethod](fido2authenticationmethod.md)|Uma chave de segurança FIDO2 pode ser usada por um usuário para entrar no Azure AD.|Exclua uma chave de segurança FIDO2 perdida.|
|[microsoftAuthenticatorAuthenticationMethod](microsoftauthenticatorauthenticationmethod.md)|Microsoft Authenticator pode ser usado por um usuário para entrar ou executar a autenticação multifator para Azure AD|Exclua um Microsoft Authenticator de autenticação.|
|[windowsHelloForBusinessAuthenticationMethod](windowsHelloForBusinessAuthenticationMethod.md)|Windows Hello para Empresas é um método de entrada sem senha em Windows dispositivos.|Veja dispositivos em que um usuário habilitou Windows Hello para Empresas entrada. Exclua uma Windows Hello para Empresas credencial.|

Os métodos de autenticação a seguir ainda não têm suporte no Microsoft Graph v1.0.

|Método de autenticação       | Descrição |Exemplos     |
|:---------------------------|:------------|:------------|
|Password | No momento, uma senha é o método de autenticação primário padrão Azure AD.|Redefina a senha de um usuário.|
|phoneAuthenticationMethod (ainda sem suporte) |Um telefone pode ser usado por um usuário para autenticar usando [SMS ou chamadas de voz](/azure/active-directory/authentication/concept-authentication-methods#phone-options) (conforme permitido pela política).|Veja os números de telefone de autenticação de um usuário. Adicionar, atualizar ou remover um número de telefone para um usuário. Habilitar ou desabilitar um telefone celular primário para SMS logon.|
|Email |Um endereço de email pode ser usado por um usuário como parte do processo Self-Service SSPR (Redefinição de Senha).|Consulte o endereço de email de autenticação de um usuário. Adicionar, atualizar ou remover um endereço de email para um usuário.|
|Passagem de Acesso Temporária |A Passagem de Acesso Temporária é uma senha com tempo limitado que serve como uma credencial forte e permite a integração de credenciais sem senha. | Defina uma nova Passagem de Acesso Temporário em um usuário.|
|Token de hardware | Permitir que os usuários executem a autenticação multifator usando um dispositivo físico que fornece um código único. | Obtenha um token de hardware atribuído a um usuário.|
|Token de software | Permitir que os usuários executem a autenticação multifator usando um aplicativo que dê suporte à especificação OAUTH e forneça um código único. | Obter e excluir um token de software atribuído a um usuário.|
|Perguntas e respostas de segurança | Permitir que os usuários validem sua identidade ao executar uma redefinição de senha de autoatendimento. |Excluir uma pergunta de segurança que um usuário registrou.|
|Método padrão | Representa o método que o usuário selecionou como padrão para executar a autenticação multifator.| Alterar o método de MFA padrão de um usuário. <br/> **NOTA:** Atualmente, o gerenciamento dos detalhes do método padrão só tem suporte por meio do MSOL `Get-MsolUser` `Set-MsolUser` e dos cmdlets, usando a propriedade **StrongAuthenticationMethods** . |
|Exigir o registro de MFA novamente | Representa uma configuração que exige que, quando o usuário entrar na próxima vez, ele seja solicitado a configurar um novo método de autenticação MFA.| Permitir que o usuário configure novos métodos de MFA, por exemplo, se ele tiver alterado seu dispositivo de autenticação. <br/> **NOTA:** Atualmente, esse recurso só tem suporte por meio do cmdlet MSOL`Set-MsolUser` , usando a **propriedade StrongAuthenticationMethods** . |

## <a name="next-steps"></a>Próximas etapas

* Examine os tipos de método de autenticação e seus vários métodos.
* Experimente a API no [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).
