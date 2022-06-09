---
title: Visão geral da API de métodos de autenticação do Azure AD
description: Os métodos de autenticação são como os usuários se autenticam no Azure AD.
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: e7fe99adedfe0130e7fb4c3cc5f789f518a55b78
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971606"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Visão geral da API de métodos de autenticação do Azure AD

Namespace: microsoft.graph

[Os métodos de autenticação](/azure/active-directory/authentication/concept-authentication-methods) são as maneiras como os usuários se autenticam no Azure AD (Active Directory). Os métodos de autenticação no Azure AD incluem senha e telefone (por exemplo, sms e chamadas de voz), que são gerenciáveis atualmente no ponto de extremidade beta do Microsoft Graph, entre muitos outros, como chaves de segurança FIDO2 e o aplicativo Microsoft Authenticator. Os métodos de autenticação são usados nas autenticações primária, de segundo fator e de step-up. Além disso, no processo de redefinição de senha de autoatendimento (SSPR).

As APIs de método de autenticação são usadas para gerenciar os métodos de autenticação de um usuário. Por exemplo:

* Você pode recuperar detalhes da Chave de Segurança FIDO2 de um usuário e excluí-la se o usuário tiver perdido a chave.
* Você pode recuperar detalhes do registro do Microsoft Authenticator de um usuário e excluí-lo se o usuário tiver perdido o telefone.

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>Quais métodos de autenticação podem ser gerenciados no Microsoft Graph?

|Método de autenticação       | Descrição |Exemplos     |
|:---------------------------|:------------|:------------|
|[fido2AuthenticationMethod](fido2authenticationmethod.md)|Uma chave de segurança FIDO2 pode ser usada por um usuário para entrar no Azure AD.|Exclua uma chave de segurança FIDO2 perdida.|
|[microsoftAuthenticatorAuthenticationMethod](microsoftauthenticatorauthenticationmethod.md)|O Microsoft Authenticator pode ser usado por um usuário para entrar ou executar a autenticação multifator no Azure AD|Exclua um método de autenticação do Microsoft Authenticator.|
|[temporaryAccessPassAuthenticationMethod](temporaryaccesspassauthenticationmethod.md)|Uma senha com tempo limitado que serve como uma credencial forte e permite a integração de credenciais sem senha.|
|[windowsHelloForBusinessAuthenticationMethod](windowsHelloForBusinessAuthenticationMethod.md)|O Windows Hello para Empresas é um método de entrada sem senha em dispositivos Windows.|Veja os dispositivos em que um usuário habilitou a entrada do Windows Hello para Empresas. Exclua uma credencial do Windows Hello para Empresas.|

Os métodos de autenticação a seguir ainda não têm suporte no Microsoft Graph v1.0.

|Método de autenticação       | Descrição |Exemplos     |
|:---------------------------|:------------|:------------|
|Password | No momento, uma senha é o método de autenticação primária padrão no Azure AD.|Redefina a senha de um usuário.|
|phoneAuthenticationMethod (ainda sem suporte) |Um telefone pode ser usado por um usuário para autenticar usando [SMS ou chamadas de voz](/azure/active-directory/authentication/concept-authentication-methods#phone-options) (conforme permitido pela política).|Veja os números de telefone de autenticação de um usuário. Adicionar, atualizar ou remover um número de telefone para um usuário. Habilitar ou desabilitar um telefone celular primário para entrada por SMS.|
|Email |Um endereço de email pode ser usado por um usuário como parte do processo Self-Service SSPR (Redefinição de Senha).|Consulte o endereço de email de autenticação de um usuário. Adicionar, atualizar ou remover um endereço de email para um usuário.|
|Token de hardware | Permitir que os usuários executem a autenticação multifator usando um dispositivo físico que fornece um código único. | Obtenha um token de hardware atribuído a um usuário.|
|Token de software | Permitir que os usuários executem a autenticação multifator usando um aplicativo que dê suporte à especificação OAUTH e forneça um código único. | Obter e excluir um token de software atribuído a um usuário.|
|Perguntas e respostas de segurança | Permitir que os usuários validem sua identidade ao executar uma redefinição de senha de autoatendimento. |Excluir uma pergunta de segurança que um usuário registrou.|
|Método padrão | Representa o método que o usuário selecionou como padrão para executar a autenticação multifator.| Alterar o método de MFA padrão de um usuário. <br/> **NOTA:** Atualmente, o gerenciamento dos detalhes do método padrão só tem suporte por meio do MSOL `Get-MsolUser` `Set-MsolUser` e dos cmdlets, usando a propriedade **StrongAuthenticationMethods** . |
|Exigir o registro de MFA novamente | Representa uma configuração que exige que, quando o usuário entrar na próxima vez, ele seja solicitado a configurar um novo método de autenticação MFA.| Permitir que o usuário configure novos métodos de MFA, por exemplo, se ele tiver alterado seu dispositivo de autenticação. <br/> **NOTA:** Atualmente, esse recurso só tem suporte por meio do cmdlet MSOL`Set-MsolUser` , usando a **propriedade StrongAuthenticationMethods** . |

## <a name="next-steps"></a>Próximas etapas

* Examine os tipos de método de autenticação e seus vários métodos.
* Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
