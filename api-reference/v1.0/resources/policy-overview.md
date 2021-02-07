---
title: visão geral da API de política
description: O Azure Active Directory usa políticas para controlar os comportamentos de recursos do Azure AD em sua organização.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 4f1b705b13518bdd1b5ede0c85c20dad0a593e2a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128474"
---
# <a name="azure-ad-policy-overview"></a>Visão geral da política do Azure AD

Namespace: microsoft.graph



O Azure Active Directory (Azure AD) usa políticas para controlar os comportamentos de recursos do Azure AD em sua organização. As políticas são regras personalizadas que podem ser impostas a aplicativos, entidades de serviço, grupos ou em toda a organização à que são atribuídas.

## <a name="what-policies-are-available"></a>Quais políticas estão disponíveis?

| Tipo de política       | Descrição | Exemplos |
|:-------------|:------------|:------------|
|[activityBasedTimeoutPolicies](activityBasedTimeoutPolicy.md)| Representa uma política que controla a saída automática para sessões da Web após um período de inatividade, para aplicativos que suportam a funcionalidade de tempo de saída baseada em atividade.| Configure o portal do Azure para ter um tempo de inatividade de 15 minutos. |
|[claimsMappingPolicies](claimsMappingPolicy.md)| Representa as políticas de mapeamento de declaração para os protocolos WS-Fed, SAML, OAuth 2.0 e OpenID Connect, para tokens emitidos para um aplicativo específico. | Crie e atribua uma política para omitir as declarações básicas de tokens emitidos para uma entidade de serviço. |
|[homeRealmDiscoveryPolicies](homeRealmDiscoveryPolicy.md)| Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados, em particular para restrições de aceleração automática e autenticação de usuário em domínios federados.| Configure todos os usuários para ignorar a descoberta de realm inicial e ser roteado diretamente para o ADFS para autenticação. |
|[tokenLifetimePolicies](tokenlifetimepolicy.md)|Representa a duração da vida útil dos tokens de acesso usados para acessar recursos protegidos.| Configure um aplicativo particularmente sensível com um tempo de vida de token menor do que o padrão.|
|[tokenIssuancePolicy](tokenIssuancePolicy.md)|Representa a política para especificar as características dos tokens SAML emitidos pelo Azure AD.| Configure o algoritmo de assinatura ou a versão do token SAML a ser usada para emitir o token SAML.
|[identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)|Representa a política de padrões de segurança do Azure AD.| Configure a política de padrões de segurança do Azure AD para se proteger contra ataques comuns.

## <a name="next-steps"></a>Próximas etapas

* Revise os diferentes tipos de resouce de política listados acima e seus diversos métodos.
* Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

