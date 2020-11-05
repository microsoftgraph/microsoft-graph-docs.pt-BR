---
title: Visão geral da API da política de métodos de autenticação do Azure AD
description: Métodos de autenticação as políticas definem quais métodos de autenticação podem ser usados por usuários no Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 730368b4e47c34353882e5e601644133dbb38225
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921568"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Visão geral da API de métodos de autenticação do Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Métodos de autenticação as políticas definem [métodos de autenticação](/azure/active-directory/authentication/concept-authentication-methods) e os usuários que têm permissão para usá-los para entrar e realizar a autenticação multifator (MFA) no Azure Active Directory (Azure AD). Métodos de autenticação as políticas que podem ser gerenciadas no Microsoft Graph incluem chaves de segurança FIDO2 e entrada de telefone sem senha com o aplicativo Microsoft Authenticator.

As APIs de diretivas de método de autenticação são usadas para gerenciar as configurações de política. Por exemplo:

* Defina os tipos de chaves de segurança do FIDO2 que podem ser usados no locatário do Azure AD.
* Definir os usuários ou grupos de usuários que têm permissão para usar chaves de segurança do FIDO2 ou entrada de telefone sem senha para entrar no Azure AD.

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>Quais políticas de métodos de autenticação podem ser gerenciadas no Microsoft Graph?

|Política de método de autenticação       | Descrição |
|:---------------------------|:------------|:------------|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| Definir restrições de chave de segurança FIDO2 e usuários que podem usá-las para entrar no Azure AD.|
|[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|Defina usuários que podem usar a entrada de telefone sem senha para entrar no Azure AD.|

## <a name="next-steps"></a>Próximas etapas

* Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
