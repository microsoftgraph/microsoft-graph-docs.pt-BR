---
title: Tipo de recurso policyRoot
description: Tipo de recurso expondo propriedades de navegação para o singleton de políticas.
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6f0a5b9862a955b9508fb9a9075a848646dbcac8
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688434"
---
# <a name="policyroot-resource-type"></a>Tipo de recurso policyRoot

Namespace: microsoft.graph

Tipo de recurso expondo propriedades de navegação para o singleton de políticas.

## <a name="methods"></a>Methods
Nenhum

## <a name="properties"></a>Propriedades
Nenhuma


## <a name="relationships"></a>Relações
| Relação                              | Tipo                                                                                                      | Descrição                                                                                                                                                             |
|:------------------------------------------|:----------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| accessReviewPolicy                        | [accessReviewPolicy](accessreviewpolicy.md)                                                               | A política que contém configurações de revisão de acesso no nível do diretório.                                                                                                        |
| activityBasedTimeoutPolicies              | [Coleção activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md)                                    | A política que controla o tempo de ociosidade das sessões da Web para aplicativos.                                                                                           |
| adminConsentRequestPolicy                 | [adminConsentRequestPolicy](adminconsentrequestpolicy.md)                                                 | A política pela qual as solicitações de consentimento são criadas e gerenciadas para todo o locatário.                                                                                     |
| appManagementPolicies                     | [appManagementPolicy](appmanagementpolicy.md) collection                                                  | As políticas que impõem restrições de gerenciamento de aplicativos para aplicativos e entidades de serviço específicas, substituindo o defaultAppManagementPolicy.                      |
| authenticationFlowsPolicy                 | [authenticationFlowsPolicy](authenticationflowspolicy.md)                                                 | A configuração de política da experiência de assinatura de autoatendam de usuários externos.                                                                                      |
| authenticationMethodsPolicy               | [authenticationMethodsPolicy](authenticationmethodspolicy.md)                                             | Os métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a autenticação multifato (MFA) no Azure Active Directory (Azure AD).    |
| authorizationPolicy                       | [Coleção authorizationPolicy](authorizationpolicy.md)                                                  | A política que controla as configurações de autorização do Azure AD.                                                                                                               |
| b2cauthenticationmethodspolicy            | [b2cauthenticationmethodspolicy](b2cauthenticationmethodspolicy.md)                                       | As políticas do Azure AD B2C que definem como os usuários finais se registram por meio de contas locais.                                                                                        |
| claimsMappingPolicies                     | Conjunto [claimsMappingPolicy](claimsmappingpolicy.md)                                                  | As políticas de mapeamento de declaração para protocolos WS-Fed, SAML, OAuth 2.0 e Conexão OpenID, para tokens emitidos para um aplicativo específico.                                      |
| conditionalAccessPolicies                 | [conditionalAccessPolicy](conditionalaccesspolicy.md)                                                     | As regras personalizadas que definem um cenário de acesso.                                                                                                                        |
| defaultAppManagementPolicy                | [tenantAppManagementPolicy](tenantappmanagementpolicy.md)                                                 | A política de todo o locatário que impõe restrições de gerenciamento de aplicativos para todos os aplicativos e entidades de serviço.                                                           |
| deviceRegistrationPolicy                  | [deviceRegistrationPolicy](deviceregistrationpolicy.md)                                                   | Representa o escopo de política que controla restrições de cota, autenticação adicional e políticas de autorização para registrar identidades de dispositivos em sua organização. |
| featureRolloutPolicies                    | [Coleção featureRolloutPolicy](featurerolloutpolicy.md)                                                | A política de lançamento de recursos associada a um objeto de diretório.                                                                                                          |
| homeRealmDiscoveryPolicies                | Conjunto [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)                                        | A política para controlar o comportamento de autenticação do Azure AD para usuários federados.                                                                                             |
| identitySecurityDefaultsEnforcementPolicy | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)                 | A política que representa os padrões de segurança que protegem contra ataques comuns.                                                                                   |
| mobileAppManagementPolicies               | [Coleção mobilityManagementPolicy](mobilitymanagementpolicy.md)                                        | A política que define a configuração de registro automático para um aplicativo de gerenciamento de mobilidade (MDM ou MAM).                                                               |
| permissionGrantPolicies                   | conjunto [permissionGrantPolicy](permissiongrantpolicy.md)                                              | A política que especifica as condições sob as quais o consentimento pode ser concedido.                                                                                            |
| roleManagementPolicies                    | [Coleção unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)                     | Representa as políticas de gerenciamento de função.                                                                                                                                |
| roleManagementPolicyAssignments           | [Coleção unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) | Representa as atribuições de política de gerenciamento de função.                                                                                                                      |
| tokenIssuancePolicies                     | coleção [tokenIssuancePolicy](tokenissuancepolicy.md)                                                  | A política que especifica as características dos tokens SAML emitidos pelo Azure AD.                                                                                        |
| tokenLifetimePolicies                     | Conjunto [tokenLifetimePolicy](tokenlifetimepolicy.md)                                                  | A política que controla o tempo de vida de um token de acesso JWT, um token de ID ou um token SAML 1.1/2.0 emitido pelo Azure AD.                                                   |

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

