---
title: Visão geral da API de política de métodos de autenticação do Azure AD
description: As políticas de métodos de autenticação definem quais métodos de autenticação podem ser usados pelos usuários no Azure AD.
localization_priority: Normal
author: mmcla
ms.author: michmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 1446603a027085902d5af27a33727bbec03f4496
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515433"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Visão geral das políticas de políticas de autenticação do Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As políticas de [](/azure/active-directory/authentication/concept-authentication-methods) métodos de autenticação definem métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a autenticação multifatofa (MFA) no Azure Active Directory (Azure AD). As políticas de métodos de autenticação que podem ser gerenciadas no Microsoft Graph incluem Chaves de Segurança FIDO2 e Login de Telefone Sem Senha com o aplicativo Microsoft Authenticator.

As APIs de políticas de método de autenticação são usadas para gerenciar configurações de política. Por exemplo:

* Defina os tipos de chaves de segurança FIDO2 que podem ser usadas no locatário do Azure AD.
* Defina os usuários ou grupos de usuários que têm permissão para usar chaves de segurança fido2 ou entrar sem senha para entrar no Azure AD.

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>Quais políticas de métodos de autenticação podem ser gerenciadas no Microsoft Graph?

|Política de método de autenticação       | Descrição |
|:---------------------------|:------------|
|[smsAuthenticationMethodConfiguration](smsAuthenticationMethodConfiguration.md)| Definir usuários que podem usar Mensagem de Texto no locatário do Azure AD.|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| Defina restrições de chave de segurança FIDO2 e usuários que podem usá-las para entrar no Azure AD.|
|[microsoftauthenticatorauthenticationmethodconfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)|Definir usuários que podem usar o Microsoft Authenticator no locatário do Azure AD.|
|[emailauthenticationmethodconfiguration](emailauthenticationmethodconfiguration.md)|Definir usuários que podem usar o OTP de email no locatário do Azure AD.|
|[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) (preterido)|Defina os usuários que podem usar o Acesso sem Senha para entrar no Azure AD.|
|[temporaryaccesspassauthenticationmethodconfiguration](temporaryaccesspassauthenticationmethodconfiguration.md)|Defina os usuários que podem usar o Passe de Acesso Temporário para entrar no Azure AD.|

## <a name="next-steps"></a>Próximas etapas

* Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
