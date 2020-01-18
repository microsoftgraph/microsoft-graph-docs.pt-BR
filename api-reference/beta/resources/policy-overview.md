---
title: Visão geral da API de política
description: O Azure Active Directory usa políticas para controlar comportamentos de recursos do Azure AD em sua organização.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 3829a4018c9b904b058329d52149e98337ebfae6
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234131"
---
# <a name="azure-ad-policy-overview"></a>Visão geral da política do Azure AD

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O Azure Active Directory (Azure AD) usa políticas para controlar comportamentos de recursos do Azure AD em sua organização. As políticas são regras personalizadas que podem ser impostas em aplicativos, entidades de serviço, grupos ou em toda a organização à qual foram atribuídos.

## <a name="what-policies-are-available"></a>Quais políticas estão disponíveis?

| Tipo de política       | Descrição | Exemplos |
|:-------------|:------------|:------------|
|[activityBasedTimeoutPolicies](activityBasedTimeoutPolicy.md)| Representa uma política que controla a saída automática para sessões da Web após um período de inatividade, para aplicativos que dão suporte à funcionalidade de tempo limite baseada na atividade.| Configure o portal do Azure para ter um tempo limite de inatividade de 15 minutos. |
|[claimsMappingPolicies](claimsMappingPolicy.md)| Representa as políticas de mapeamento de declaração para protocolos WS-Alimentad, SAML, OAuth 2,0 e OpenID Connect, para tokens emitidos para um aplicativo específico. | Crie e atribua uma política para omitir as declarações básicas de tokens emitidos para uma entidade de serviço. |
|[homeRealmDiscoveryPolicies](homeRealmDiscoveryPolicy.md)| Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados, em particular para as restrições de aceleração automática e autenticação de usuário em domínios federados.| Configure todos os usuários para ignorar a descoberta de realm inicial e ser roteado diretamente para o ADFS para autenticação. |
|[tokenLifetimePolicies](tokenlifetimepolicy.md)|Representa a duração da vida útil dos tokens de acesso usados para acessar recursos protegidos.| Configure um aplicativo especialmente confidencial com uma vida útil mais curta do que o token padrão.|

## <a name="next-steps"></a>Próximas etapas

* Revise os diferentes tipos de recursos de política listados acima e seus vários métodos.
* Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
