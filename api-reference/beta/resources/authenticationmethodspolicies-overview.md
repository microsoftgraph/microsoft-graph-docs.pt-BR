---
title: Visão geral da API de política de métodos de autenticação do Azure AD
description: As políticas de métodos de autenticação definem quais métodos de autenticação podem ser usados pelos usuários no Azure AD.
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
---

# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Visão geral das políticas de políticas de autenticação do Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As políticas de métodos de [](/azure/active-directory/authentication/concept-authentication-methods) autenticação definem métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a autenticação multifato (MFA) no Azure Active Directory (Azure AD). As políticas de métodos de autenticação que podem ser gerenciadas no Microsoft Graph incluem chaves de segurança fido2 e Telefone de acesso sem senha com Microsoft Authenticator aplicativo.

As APIs de políticas de método de autenticação são usadas para gerenciar configurações de política. Por exemplo:

* Defina os tipos de chaves de segurança FIDO2 que podem ser usadas no locatário do Azure AD.
* Defina os usuários ou grupos de usuários que têm permissão para usar chaves de segurança FIDO2 ou senhas Telefone entrar no Azure AD.
* Defina os usuários ou grupos de usuários que devem ser lembrados para configurar o Microsoft Authenticator para MFA usando notificações por push.

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>Quais políticas de métodos de autenticação podem ser gerenciadas no Microsoft Graph?

|Política de método de autenticação       | Descrição |
|:---------------------------|:------------|
|[smsAuthenticationMethodConfiguration](smsAuthenticationMethodConfiguration.md)| Definir usuários que podem usar Mensagem de Texto no locatário do Azure AD.|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| Defina restrições de chave de segurança FIDO2 e usuários que podem usá-las para entrar no Azure AD.|
|[microsoftauthenticatorauthenticationmethodconfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)|Definir usuários que podem usar Microsoft Authenticator no locatário do Azure AD.|
|[emailauthenticationmethodconfiguration](emailauthenticationmethodconfiguration.md)|Definir usuários que podem usar o OTP de email no locatário do Azure AD.|
|[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) (preterido)|Defina os usuários que podem usar a senha Telefone entrar para entrar no Azure AD.|
|[temporaryaccesspassauthenticationmethodconfiguration](temporaryaccesspassauthenticationmethodconfiguration.md)|Defina os usuários que podem usar o Passe de Acesso Temporário para entrar no Azure AD.|
|[x509CertificateAuthenticationMethodConfiguration](x509CertificateAuthenticationMethodConfiguration.md)|Defina os usuários que podem usar o certificado X.509 para entrar no Azure AD.|

## <a name="policies-available-to-push-users-to-set-up-authentication-methods"></a>Políticas disponíveis para pressionar os usuários a configurar métodos de autenticação:
|Política       | Descrição |
|:---------------------------|:------------|
|[authenticationMethodsRegistrationCampaign](authenticationmethodsregistrationcampaign.md)| Defina os usuários que devem ser lembrados para configurar um método de autenticação (somente com suporte para o Microsoft Authenticator).|

## <a name="next-steps"></a>Próximas etapas

* Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
