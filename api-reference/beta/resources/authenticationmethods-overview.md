---
title: Visão geral da API de métodos de autenticação do Azure AD
description: Os métodos de autenticação são como os usuários autenticam no Azure AD.
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 4830a9e098c84488441ec95250919ea317a0e8fb
ms.sourcegitcommit: 709d2e3069765c2e570ac1128847c165ab233aa8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2022
ms.locfileid: "62184070"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Visão geral da API de métodos de autenticação do Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Os métodos de autenticação](/azure/active-directory/authentication/concept-authentication-methods) são as maneiras que os usuários autenticam no Azure Active Directory (AD). Os métodos de autenticação do Azure AD incluem senha e telefone (por exemplo, SMS e chamadas de voz), que hoje são gerenciáveis no Microsoft Graph, entre muitos outros, como chaves de segurança FIDO2 e o aplicativo Microsoft Authenticator. Os métodos de autenticação são usados nas autenticações primária, de segundo fator e de step-up. Além disso, no processo de redefinição de senha de autoatendimento (SSPR).

As APIs do método de autenticação são usadas para gerenciar os métodos de autenticação de um usuário. Por exemplo:

* Você pode adicionar um número de telefone a um usuário. Em seguida, o usuário pode usar esse número de telefone para autenticação de SMS e chamada de voz se estiver habilitado para usá-lo por política.
* Você pode atualizar esse número ou excluí-lo do usuário.
* Você pode habilitar ou desabilitar o número de login sms.
* Você pode redefinir a senha de um usuário.
* Você pode recuperar detalhes da Chave de Segurança FIDO2 de um usuário e excluí-la se o usuário tiver perdido a chave.
* Você pode recuperar detalhes do registro de Microsoft Authenticator usuário e excluí-lo se o usuário tiver perdido o telefone.
* Você pode adicionar um endereço de email a um usuário. Em seguida, o usuário pode usar esse email como parte do processo Self-Service redefinição de senha (SSPR).
* Você pode atualizar esse email ou excluí-lo do usuário.

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>Quais métodos de autenticação podem ser gerenciados no Microsoft Graph?

|Método de autenticação       | Descrição |Exemplos     |
|:---------------------------|:------------|:------------|
|[passwordAuthenticationMethod](passwordauthenticationmethod.md)| No momento, uma senha é o método de autenticação principal padrão no Azure AD.|Redefinir a senha de um usuário|
|[phoneAuthenticationMethod](phoneauthenticationmethod.md)|Um telefone pode ser usado por um usuário para autenticar usando SMS ou chamadas de [voz](/azure/active-directory/authentication/concept-authentication-methods#phone-options) (conforme permitido pela política).|Consulte os números de telefone de autenticação de um usuário. Adicionar, atualizar ou remover um número de telefone para um usuário. Habilitar ou desabilitar um telefone celular principal para a assinatura SMS.|
|[fido2AuthenticationMethod](fido2authenticationmethod.md)|Uma Chave de Segurança FIDO2 pode ser usada por um usuário para entrar no Azure AD.|Excluir uma chave de segurança FIDO2 perdida.|
|[microsoftAuthenticatorAuthenticationMethod](microsoftauthenticatorauthenticationmethod.md)|Microsoft Authenticator pode ser usado por um usuário para entrar ou executar a autenticação multifafação no Azure AD|Exclua um Microsoft Authenticator de autenticação.|
|[passwordlessmicrosoftauthenticatorauthenticationmethod](passwordlessmicrosoftauthenticatorauthenticationmethod.md) (preterido)|Microsoft Authenticator senha Telefone entrar sem senha pode ser usado por um usuário para entrar no Azure AD|Exclua um método Telefone autenticação de login sem senha.|
|[emailAuthenticationMethod](emailauthenticationmethod.md)|Um endereço de email pode ser usado por um usuário como parte do processo Self-Service redefinição de senha (SSPR).|Consulte o endereço de email de autenticação de um usuário. Adicionar, atualizar ou remover um endereço de email para um usuário.|
|[windowsHelloForBusinessAuthenticationMethod](windowsHelloForBusinessAuthenticationMethod.md)|Windows Hello para Empresas é um método de entrada sem senha em Windows dispositivos.|Consulte dispositivos onde um usuário habilitar Windows Hello entrada para Empresas. Exclua uma Windows Hello para Empresas.|
|[temporaryaccesspassauthenticationmethod](temporaryaccesspassauthenticationmethod.md)|Passagem de Acesso Temporário é uma senha limitada por tempo que serve como uma credencial forte e permite a integração de credenciais sem senha. | Definir uma nova Passagem de Acesso Temporário em um usuário.|
|[softwareOathAuthenticationMethod](../resources/softwareoathauthenticationmethod.md)| Permitir que os usuários executem a autenticação multifator usando um aplicativo que dá suporte à especificação DODL e fornece um código único. | Obter e excluir um token de software atribuído a um usuário.|

Os métodos de autenticação a seguir ainda não são suportados no Microsoft Graph `beta` .

|Método de autenticação       | Descrição |Exemplos     |
|:---------------------------|:------------|:------------|
|Token de hardware | Permitir que os usuários executem a autenticação multifator usando um dispositivo físico que fornece um código único. | Obter um token de hardware atribuído a um usuário.|
|Perguntas e respostas de segurança | Permitir que os usuários validem sua identidade ao executar uma redefinição de senha de autoatendida. |Excluir uma pergunta de segurança registrada por um usuário.|
|Método padrão | Representa o método que o usuário selecionou como padrão para executar a autenticação multifato.| Alterar o método MFA padrão de um usuário. <br/> **OBSERVAÇÃO:** No momento, o gerenciamento dos detalhes do método padrão só tem suporte por meio do MSOL e `Get-MsolUser` `Set-MsolUser` cmdlets, usando a propriedade **StrongAuthenticationMethods.** |
|Exigir o re-registro MFA | Representa uma configuração que exige que, quando o usuário entrar na próxima vez, ele seja solicitado a configurar um novo método de autenticação MFA.| Permita que o usuário configurar novos métodos MFA, por exemplo, se ele alterou seu dispositivo de autenticação. <br/> **OBSERVAÇÃO:** Atualmente, esse recurso só tem suporte por meio do `Set-MsolUser` cmdlet MSOL, usando a **propriedade StrongAuthenticationMethods.** |

## <a name="next-steps"></a>Próximas etapas

* Revise os tipos de método de autenticação e seus vários métodos.
* Experimente a API no [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).
