---
title: Visão geral da API de métodos de autenticação do Azure AD
description: Os métodos de autenticação são como os usuários autenticam no Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 6027e03a4c78c5359db77ee9c263c9e98f412a9f
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469119"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Visão geral da API de métodos de autenticação do Azure AD

Namespace: microsoft.graph

[Os métodos de autenticação](/azure/active-directory/authentication/concept-authentication-methods) são as maneiras que os usuários autenticam no Azure Active Directory (AD). Os métodos de autenticação no Azure AD incluem senha e telefone (por exemplo, sms e chamadas de voz), que são gerenciáveis no ponto de extremidade beta do Microsoft Graph hoje, entre muitas outras, como chaves de segurança FIDO2 e o aplicativo Microsoft Authenticator. Os métodos de autenticação são usados nas autenticações primária, de segundo fator e de step-up. Além disso, no processo de redefinição de senha de autoatendimento (SSPR).

As APIs do método de autenticação são usadas para gerenciar os métodos de autenticação de um usuário. Por exemplo:

* Você pode recuperar detalhes da Chave de Segurança FIDO2 de um usuário e excluí-la se o usuário tiver perdido a chave.
* Você pode recuperar detalhes do registro do Microsoft Authenticator de um usuário e excluí-lo se o usuário tiver perdido o telefone.

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>Quais métodos de autenticação podem ser gerenciados no Microsoft Graph?

|Método de autenticação       | Descrição |Exemplos     |
|:---------------------------|:------------|:------------|
|[fido2AuthenticationMethod](fido2authenticationmethod.md)|Uma Chave de Segurança FIDO2 pode ser usada por um usuário para entrar no Azure AD.|Excluir uma chave de segurança FIDO2 perdida.|
|[microsoftAuthenticatorAuthenticationMethod](microsoftauthenticatorauthenticationmethod.md)|O Microsoft Authenticator pode ser usado por um usuário para entrar ou executar a autenticação multifafatório no Azure AD|Exclua um método de autenticação do Microsoft Authenticator.|
|[windowsHelloForBusinessAuthenticationMethod](windowsHelloForBusinessAuthenticationMethod.md)|O Windows Hello para Empresas é um método de entrada sem senha em dispositivos Windows.|Consulte dispositivos em que um usuário habilitar a entrada do Windows Hello para Empresas. Exclua uma credencial do Windows Hello para Empresas.|

## <a name="next-steps"></a>Próximas etapas

* Revise os tipos de método de autenticação e seus vários métodos.
* Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).