---
title: Visão geral da API de política de métodos de autenticação do Azure AD
description: As políticas de métodos de autenticação definem quais métodos de autenticação podem ser usados pelos usuários no Azure AD.
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 9e905b4c56da95f2dade997c1018d2b0f5b05494
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126965"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Visão geral das políticas de políticas de autenticação do Azure AD

Namespace: microsoft.graph

As políticas de [](/azure/active-directory/authentication/concept-authentication-methods) métodos de autenticação definem métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a autenticação multifato (MFA) no Azure Active Directory (Azure AD). As políticas de métodos de autenticação que podem ser gerenciadas no Microsoft Graph incluem chaves de segurança fido2 e Telefone de acesso sem senha com Microsoft Authenticator aplicativo.

As APIs de políticas de método de autenticação são usadas para gerenciar configurações de política. Por exemplo:

* Defina os tipos de chaves de segurança FIDO2 que podem ser usadas no locatário do Azure AD.
* Defina os usuários ou grupos de usuários que têm permissão para usar chaves de segurança FIDO2 ou senhas Telefone entrar no Azure AD.

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>Quais políticas de métodos de autenticação podem ser gerenciadas no Microsoft Graph?

|Política de método de autenticação       | Descrição |
|:---------------------------|:------------|:------------|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| Defina restrições de chave de segurança FIDO2 e usuários que podem usá-las para entrar no Azure AD.|
|[microsoftauthenticatorauthenticationmethodconfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)|Definir usuários que podem usar Microsoft Authenticator no locatário do Azure AD.|
|[emailauthenticationmethodconfiguration](emailauthenticationmethodconfiguration.md)|Definir usuários que podem usar o OTP de email no locatário do Azure AD.|

## <a name="next-steps"></a>Próximas etapas

* Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
