---
title: visão geral da API de política
description: O Azure Active Directory usa políticas para controlar os comportamentos de recursos do Azure AD em sua organização.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 3e8d4134a1de4baa22ad8be511651c302b883f52
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882527"
---
# <a name="azure-ad-policy-overview"></a>Visão geral da política do Azure AD

Namespace: microsoft.graph

O Azure Active Directory (Azure AD) usa políticas para controlar os comportamentos de recursos do Azure AD em sua organização. As políticas são regras personalizadas que você pode impor a aplicativos, entidades de serviço, grupos ou em toda a organização à que são atribuídas.

## <a name="what-policies-are-available"></a>Quais políticas estão disponíveis?

| Tipo de política       | Descrição | Exemplos |
|:-------------|:------------|:------------|
|[activityBasedTimeoutPolicies](activityBasedTimeoutPolicy.md)| Representa uma política que controla a saída automática para sessões da Web após um período de inatividade, para aplicativos que suportam a funcionalidade de tempo de tempo de atividade baseada em atividade.| Configure o portal do Azure para ter um tempo de inatividade de 15 minutos. |
|[authenticationFlowsPolicies](authenticationflowspolicy.md)| Representa uma política que controla se os usuários externos devem ser capazes de se inscrever e obter uma conta de convidado por meio de um fluxo de usuário de autoatendado de Identidades Externas.| Habilita seus aplicativos para dar suporte a usuários externos que se insinuem por meio de um fluxo de usuário de inscrição de autoatendado. |
|[claimsMappingPolicies](claimsMappingPolicy.md)| Representa as políticas de mapeamento de declaração para protocolos WS-Fed, SAML, OAuth 2.0 e OpenID Connect para tokens emitidos para um aplicativo específico. | Crie e atribua uma política para omitir as declarações básicas de tokens emitidos para uma entidade de serviço. |
|[homeRealmDiscoveryPolicies](homeRealmDiscoveryPolicy.md)| Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados, em particular para restrições de aceleração automática e autenticação do usuário em domínios federados.| Configure todos os usuários para ignorar a descoberta do domínio inicial e ser roteado diretamente para o ADFS para autenticação. |
|[tokenLifetimePolicies](tokenlifetimepolicy.md)|Representa a duração da vida útil dos tokens de acesso usados para acessar recursos protegidos.| Configure um aplicativo particularmente sensível com um tempo de vida de token mais curto que o padrão.|
|[tokenIssuancePolicy](tokenIssuancePolicy.md)|Representa a política para especificar as características dos tokens SAML emitidos pelo Azure AD.| Configure o algoritmo de assinatura ou a versão de token SAML a ser usada para emitir o token SAML.
|[identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)|Representa a política de padrões de segurança do Azure AD.| Configure a política de padrões de segurança do Azure AD para proteger contra ataques comuns.

## <a name="next-steps"></a>Próximas etapas

* Revise os diferentes tipos de resouce de política listados acima e seus vários métodos.
* Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
