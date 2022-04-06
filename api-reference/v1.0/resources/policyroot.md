---
title: Tipo de recurso policyRoot
description: Tipo de recurso expondo propriedades de navegação para o singleton de políticas.
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9ca01343954e659da2133543a3454a56be85ecc5
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510180"
---
# <a name="policyroot-resource-type"></a>Tipo de recurso policyRoot

Namespace: microsoft.graph

Tipo de recurso expondo propriedades de navegação para o singleton de políticas.

## <a name="methods"></a>Methods
Nenhum

## <a name="properties"></a>Propriedades
Nenhuma


## <a name="relationships"></a>Relações
| Relação                              | Tipo                                                                                                      | Descrição                                                                                                                                                          |
|:------------------------------------------|:----------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| authenticationMethodsPolicy               | [authenticationMethodsPolicy](authenticationmethodspolicy.md)                                             | Os métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a autenticação multifato (MFA) no Azure Active Directory (Azure AD). |
| authenticationFlowsPolicy                 | [authenticationFlowsPolicy](authenticationflowspolicy.md)                                                 | A configuração de política da experiência de assinatura de autoatendam de usuários externos.                                                                                   |
| activityBasedTimeoutPolicies              | [Coleção activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md)                                    | A política que controla o tempo de ociosidade das sessões da Web para aplicativos.                                                                                        |
| authorizationPolicy                       | [Coleção authorizationPolicy](authorizationpolicy.md)                                                  | A política que controla as configurações de autorização do Azure AD.                                                                                                            |
| claimsMappingPolicies                     | Conjunto [claimsMappingPolicy](claimsmappingpolicy.md)                                                  | As políticas de mapeamento de declaração para protocolos WS-Fed, SAML, OAuth 2.0 e Conexão OpenID, para tokens emitidos para um aplicativo específico.                                   |
| homeRealmDiscoveryPolicies                | Conjunto [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)                                        | A política para controlar o comportamento de autenticação do Azure AD para usuários federados.                                                                                          |
| permissionGrantPolicies                   | conjunto [permissionGrantPolicy](permissiongrantpolicy.md)                                              | A política que especifica as condições sob as quais o consentimento pode ser concedido.                                                                                         |
| tokenIssuancePolicies                     | coleção [tokenIssuancePolicy](tokenissuancepolicy.md)                                                  | A política que especifica as características dos tokens SAML emitidos pelo Azure AD.                                                                                     |
| tokenLifetimePolicies                     | Conjunto [tokenLifetimePolicy](tokenlifetimepolicy.md)                                                  | A política que controla o tempo de vida de um token de acesso JWT, um token de ID ou um token SAML 1.1/2.0 emitido pelo Azure AD.                                                |
| featureRolloutPolicies                    | [Coleção featureRolloutPolicy](featurerolloutpolicy.md)                                                | A política de lançamento de recursos associada a um objeto de diretório.                                                                                                       |
| adminConsentRequestPolicy                 | [adminConsentRequestPolicy](adminconsentrequestpolicy.md)                                                 | A política pela qual as solicitações de consentimento são criadas e gerenciadas para todo o locatário.                                                                                  |
| conditionalAccessPolicies                 | [conditionalAccessPolicy](conditionalaccesspolicy.md)                                                     | As regras personalizadas que definem um cenário de acesso.                                                                                                                     |
| identitySecurityDefaultsEnforcementPolicy | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)                 | A política que representa os padrões de segurança que protegem contra ataques comuns.                                                                                |


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policyRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policyRoot"
}
```

