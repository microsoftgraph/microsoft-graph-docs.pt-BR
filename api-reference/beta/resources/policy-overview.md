---
title: visão geral da API de política
description: Azure Active Directory usa políticas para controlar os comportamentos de recursos do Azure AD em sua organização.
ms.localizationpriority: medium
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 1ab7e5ce61e2e7f0284e71a9a87046041afd140d
ms.sourcegitcommit: 2f394a9f33f2fab3634d0f18882985ee211067d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2021
ms.locfileid: "60127524"
---
# <a name="azure-ad-policy-overview"></a>Visão geral da política do Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) usa políticas para controlar os comportamentos de recursos do Azure AD em sua organização. As políticas são regras personalizadas que você pode impor a aplicativos, entidades de serviço, grupos ou em toda a organização à que são atribuídas.

## <a name="what-policies-are-available"></a>Quais políticas estão disponíveis?

| Tipo de política                                                                               | Descrição                                                                                                                                                                                       | Exemplos                                                                                                                                                                                               |
|:------------------------------------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [activityBasedTimeoutPolicies](activityBasedTimeoutPolicy.md)                             | Representa uma política que controla a saída automática para sessões da Web após um período de inatividade, para aplicativos que suportam a funcionalidade de tempo de tempo de atividade baseada em atividade.                           | Configure o portal do Azure para ter um tempo de inatividade de 15 minutos.                                                                                                                                |
| [applicationAuthenticationMethodPolicies](applicationAuthenticationMethodPolicy.md)       | Representa um conjunto de políticas que restringem operações de gerenciamento de aplicativos para aplicativos e entidades de serviço.                                                                                     | Configure aplicativos ou entidades de serviço para não usar segredos de senha ou impor a vida útil em segredos.                                                                                               |
| [authenticationFlowsPolicies](authenticationflowspolicy.md)                               | Representa uma política que controla se os usuários externos devem ser capazes de se inscrever e obter uma conta de convidado por meio de um fluxo de usuário de autoatendado de Identidades Externas.                            | Habilita seus aplicativos para dar suporte a usuários externos que se insinuem por meio de um fluxo de usuário de inscrição de autoatendado.                                                                                                    |
| [authorizationPolicy](authorizationpolicy.md)                                             | Representa uma política que pode controlar as configurações de autorização de Azure Active Directory.                                                                                                            | Configure o Azure AD para bloquear o MSOL PowerShell no locatário.                                                                                                                                             |
| [claimsMappingPolicies](claimsMappingPolicy.md)                                           | Representa as políticas de mapeamento de declaração para protocolos WS-Fed, SAML, OAuth 2.0 e OpenID Conexão, para tokens emitidos para um aplicativo específico.                                                     | Crie e atribua uma política para omitir as declarações básicas de tokens emitidos para uma entidade de serviço.                                                                                                         |
| [deviceRegistrationPolicy](deviceregistrationpolicy.md)                                   | Representa o escopo de política que controla restrições de cota, autenticação adicional e políticas de autorização para registrar identidades de dispositivos em sua organização.                           | Limite o número de dispositivos que podem ser registrados para um usuário em sua organização ou especifique usuários ou grupos que têm permissão para registrar dispositivos usando o **Azure AD Join** ou **o Azure AD registrado**. |
| [homeRealmDiscoveryPolicies](homeRealmDiscoveryPolicy.md)                                 | Representa uma política para controlar Azure Active Directory de autenticação para usuários federados, em particular para restrições de aceleração automática e autenticação do usuário em domínios federados. | Configure todos os usuários para ignorar a descoberta do domínio inicial e ser roteado diretamente para o ADFS para autenticação.                                                                                                    |
| [tokenLifetimePolicies](tokenlifetimepolicy.md)                                           | Representa a duração da vida útil dos tokens de acesso usados para acessar recursos protegidos.                                                                                                             | Configure um aplicativo particularmente sensível com um tempo de vida de token mais curto que o padrão.                                                                                                             |
| [tokenIssuancePolicy](tokenIssuancePolicy.md)                                             | Representa a política para especificar as características dos tokens SAML emitidos pelo Azure AD.                                                                                                           | Configure o algoritmo de assinatura ou a versão de token SAML a ser usada para emitir o token SAML.                                                                                                              |
| [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md) | Representa a política de padrões de segurança do Azure AD.                                                                                                                                                 | Configure a política de padrões de segurança do Azure AD para proteger contra ataques comuns.                                                                                                                     |

## <a name="next-steps"></a>Próximas etapas

- Revise os diferentes tipos de recursos de política listados acima e seus vários métodos.
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
