---
title: Visão geral da API de política de métodos de autenticação do Azure AD
description: As políticas de métodos de autenticação definem quais métodos de autenticação podem ser usados pelos usuários no Azure AD.
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: cd3e67f249a4afabc946aaa09c1c4e7448ad99f7
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971074"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Visão geral da API de políticas de métodos de autenticação do Azure AD

Namespace: microsoft.graph

As políticas de métodos de [](/azure/active-directory/authentication/concept-authentication-methods) autenticação definem métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a MFA (autenticação multifator) no Azure AD (Azure Active Directory). As políticas de métodos de autenticação que podem ser gerenciadas no Microsoft Graph incluem chaves de segurança FIDO2 e entrada por telefone sem senha com o aplicativo Microsoft Authenticator.

As APIs de políticas de método de autenticação são usadas para gerenciar as configurações de política. Por exemplo:

* Defina os tipos de chaves de segurança FIDO2 que podem ser usadas no locatário do Azure AD.
* Defina os usuários ou grupos de usuários que têm permissão para usar chaves de segurança FIDO2 ou entrada por telefone sem senha para entrar no Azure AD.
* Defina os usuários ou grupos de usuários que devem ser lembrados para configurar o Microsoft Authenticator para MFA usando notificações por push.

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>Quais políticas de métodos de autenticação podem ser gerenciadas no Microsoft Graph?

|Política de método de autenticação       | Descrição |
|:---------------------------|:------------|:------------|
|[emailauthenticationmethodconfiguration](emailauthenticationmethodconfiguration.md)|Defina os usuários que podem usar o OTP de email no locatário do Azure AD.|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| Defina restrições de chave de segurança FIDO2 e usuários que podem usá-las para entrar no Azure AD.|
|[microsoftauthenticatorauthenticationmethodconfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)|Defina os usuários que podem usar o Microsoft Authenticator no locatário do Azure AD.|
|[temporaryAccessPassAuthenticationMethod](temporaryaccesspassauthenticationmethodconfiguration.md)|Defina as definições de configuração e os usuários ou grupos que estão habilitados para usar o método de autenticação de Passagem de Acesso Temporário.|

## <a name="policies-available-for-authentication-methods-registration-campaign"></a>Políticas disponíveis para a campanha de registro de métodos de autenticação:
|Política       | Descrição |
|:---------------------------|:------------|
|[authenticationMethodsRegistrationCampaign](authenticationmethodsregistrationcampaign.md)| Defina os usuários que devem ser lembrados para configurar um método de autenticação (atualmente, só há suporte para o Microsoft Authenticator).|

## <a name="next-steps"></a>Próximas etapas

* Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
