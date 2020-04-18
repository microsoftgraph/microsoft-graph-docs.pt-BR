---
title: Visão geral da API de métodos de autenticação do Azure AD
description: Os métodos de autenticação são como os usuários são autenticados no Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 73f4bb06d15c6b2e41226e872b71ba417de1076b
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557903"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Visão geral da API de métodos de autenticação do Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os [métodos de autenticação](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) são as maneiras como os usuários são autenticados no Azure Active Directory (AD). Os métodos de autenticação no Azure AD incluem senha e telefone (por exemplo, SMS e chamadas de voz), que podem ser gerenciados no Microsoft Graph hoje, entre muitas outras, como chaves de segurança do FIDO2 e o aplicativo Microsoft Authenticator. Os métodos de autenticação são usados na autenticação principal, de segundo fator e de etapa e também no processo de redefinição de senha de autoatendimento (SSPR).

As APIs do método de autenticação são usadas para gerenciar os métodos de autenticação de um usuário. Por exemplo:

* Você pode adicionar um número de telefone a um usuário. Em seguida, o usuário pode usar esse número de telefone para autenticação de SMS e de chamada de voz se estiver habilitado para usá-lo por política. 
* Você pode atualizar esse número ou excluí-lo do usuário.
* Você pode habilitar ou desabilitar o número para entrada do SMS.
* Você pode redefinir a senha de um usuário.

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>Quais métodos de autenticação podem ser gerenciados no Microsoft Graph?

|Método de autenticação       | Descrição |Exemplos     |
|:---------------------------|:------------|:------------|
|[passwordAuthenticationMethod](passwordauthenticationmethod.md)| No momento, uma senha é o método de autenticação principal padrão no Azure AD.|Redefinir a senha de um usuário|
|[phoneAuthenticationMethod](phoneauthenticationmethod.md)|Um telefone pode ser usado por um usuário para autenticar usando o [SMS ou chamadas de voz](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods#phone-options) (conforme permitido pela política).|Confira os números de telefone de autenticação de um usuário. Adicionar, atualizar ou remover um número de telefone para um usuário. Habilitar ou desabilitar um telefone celular principal para entrada do SMS.|

## <a name="next-steps"></a>Próximas etapas

* Revise os tipos de método de autenticação e seus vários métodos.
* Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
