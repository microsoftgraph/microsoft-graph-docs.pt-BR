---
title: Visão geral da API de política de métodos de autenticação do Azure AD
description: As políticas de métodos de autenticação definem quais métodos de autenticação podem ser usados pelos usuários no Azure AD.
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: e01a054de05f4a553775364aa2f7e8cf36ba19d5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015808"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Visão geral das políticas de políticas de autenticação do Azure AD

Namespace: microsoft.graph

As políticas de [](/azure/active-directory/authentication/concept-authentication-methods) métodos de autenticação definem métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a autenticação multifato (MFA) no Azure Active Directory (Azure AD). As políticas de métodos de autenticação que podem ser gerenciadas no Microsoft Graph incluem chaves de segurança fido2 e Telefone de acesso sem senha com Microsoft Authenticator aplicativo.

As APIs de políticas de método de autenticação são usadas para gerenciar configurações de política. Por exemplo:

* Defina os tipos de chaves de segurança FIDO2 que podem ser usadas no locatário do Azure AD.
* Defina os usuários ou grupos de usuários que têm permissão para usar chaves de segurança FIDO2 ou senhas Telefone entrar no Azure AD.
* Defina os usuários ou grupos de usuários que devem ser lembrados para configurar o Microsoft Authenticator para MFA usando notificações por push.

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>Quais políticas de métodos de autenticação podem ser gerenciadas no Microsoft Graph?

|Política de método de autenticação       | Descrição |
|:---------------------------|:------------|:------------|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| Defina restrições de chave de segurança FIDO2 e usuários que podem usá-las para entrar no Azure AD.|
|[microsoftauthenticatorauthenticationmethodconfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)|Definir usuários que podem usar Microsoft Authenticator no locatário do Azure AD.|
|[emailauthenticationmethodconfiguration](emailauthenticationmethodconfiguration.md)|Definir usuários que podem usar o OTP de email no locatário do Azure AD.|

## <a name="policies-available-for-authentication-methods-registration-campaign"></a>Políticas disponíveis para campanha de registro de métodos de autenticação:
|Política       | Descrição |
|:---------------------------|:------------|
|[authenticationMethodsRegistrationCampaign](authenticationmethodsregistrationcampaign.md)| Defina os usuários que devem ser lembrados para configurar um método de autenticação (atualmente, apenas com suporte para o Microsoft Authenticator).|

## <a name="next-steps"></a>Próximas etapas

* Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
