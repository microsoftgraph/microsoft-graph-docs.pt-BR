---
title: Visão geral da API da política de métodos de autenticação do Azure AD
description: As políticas de métodos de autenticação definem quais métodos de autenticação podem ser usados pelos usuários no Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 1d8ba37ebcd97ae93f057d30ae20fb8031b45989
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135454"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Visão geral da API de políticas de métodos de autenticação do Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As políticas de métodos de autenticação [definem](/azure/active-directory/authentication/concept-authentication-methods) métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a MFA (autenticação multifatofa) no Azure Active Directory (Azure AD). As políticas de métodos de autenticação que podem ser gerenciadas no Microsoft Graph incluem chaves de segurança FIDO2 e login por telefone sem senha com o aplicativo Microsoft Authenticator.

As APIs de políticas de método de autenticação são usadas para gerenciar configurações de política. Por exemplo:

* Defina os tipos de chaves de segurança FIDO2 que podem ser usadas no locatário do Azure AD.
* Defina os usuários ou grupos de usuários que têm permissão para usar chaves de segurança FIDO2 ou login por telefone sem senha para entrar no Azure AD.

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>Quais políticas de métodos de autenticação podem ser gerenciadas no Microsoft Graph?

|Política de método de autenticação       | Descrição |
|:---------------------------|:------------|:------------|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| Defina restrições de chave de segurança FIDO2 e usuários que podem usá-las para entrar no Azure AD.|
|[microsoftauthenticatorauthenticationmethodconfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)|Defina os usuários que podem usar o Microsoft Authenticator no locatário do Azure AD.|
|[emailauthenticationmethodconfiguration](emailauthenticationmethodconfiguration.md)|Defina os usuários que podem usar o OTP de email no locatário do Azure AD.|
|[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) (preterido)|Defina os usuários que podem usar a Assinatura de Telefone Sem Senha para entrar no Azure AD.|

## <a name="next-steps"></a>Próximas etapas

* Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
