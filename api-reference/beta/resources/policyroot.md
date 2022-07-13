---
title: Tipo de recurso policyRoot
description: Tipo de recurso expondo propriedades de navegação para o singleton de políticas.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d684759f79fbcf4316c97876c7ee7e11be6de2d5
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768109"
---
# <a name="policyroot-resource-type"></a>Tipo de recurso policyRoot

Namespace: microsoft.graph

Tipo de recurso expondo propriedades de navegação para o singleton de políticas.

## <a name="methods"></a>Métodos
Nenhum

## <a name="properties"></a>Propriedades
Nenhuma

## <a name="relationships"></a>Relações

| Relação                              | Tipo                                                                                                      | Descrição                                                                                                                                                          |
|:------------------------------------------|:----------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| accessReviewPolicy                        | [accessReviewPolicy](accessreviewpolicy.md)                                                               | A política que contém as configurações de revisão de acesso no nível do diretório.                                                                                                     |
| activityBasedTimeoutPolicies              | [Coleção activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md)                                    | A política que controla o tempo limite de ociosidade para sessões da Web para aplicativos.                                                                                        |
| adminConsentRequestPolicy                 | [adminConsentRequestPolicy](adminconsentrequestpolicy.md)                                                 | A política pela qual as solicitações de consentimento são criadas e gerenciadas para todo o locatário.                                                                                  |
| appManagementPolicies                     | [appManagementPolicy](appmanagementpolicy.md) collection                                                  | As políticas que impõem restrições de gerenciamento de aplicativos para aplicativos específicos e entidades de serviço, substituindo defaultAppManagementPolicy.                   |
| authenticationFlowsPolicy                 | [authenticationFlowsPolicy](authenticationflowspolicy.md)                                                 | A configuração de política da experiência de inscrição por autoatendimento de usuários externos.                                                                                   |
| authenticationMethodsPolicy               | [authenticationMethodsPolicy](authenticationmethodspolicy.md)                                             | Os métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a MFA (autenticação multifator) no Azure Active Directory (Azure AD). |
| authorizationPolicy                       | [coleção authorizationPolicy](authorizationpolicy.md)                                                  | A política que controla as Azure AD de autorização.                                                                                                            |
| b2cauthenticationmethodspolicy            | [b2cauthenticationmethodspolicy](b2cauthenticationmethodspolicy.md)                                       | As Azure AD B2C que definem como os usuários finais se registram por meio de contas locais.                                                                                     |
| claimsMappingPolicies                     | Conjunto [claimsMappingPolicy](claimsmappingpolicy.md)                                                  | As políticas de mapeamento de declaração para protocolos WS-Fed, SAML, OAuth 2.0 e OpenID Connect, para tokens emitidos para um aplicativo específico.                                   |
| conditionalAccessPolicies                 | [conditionalAccessPolicy](conditionalaccesspolicy.md)                                                     | As regras personalizadas que definem um cenário de acesso.                                                                                                                     |
| crossTenantAccessPolicy                   | [crossTenantAccessPolicy](crosstenantaccesspolicy.md)                           | As regras personalizadas que definem um cenário de acesso ao interagir com locatários de Azure AD externos.                                                                                                                     |
| defaultAppManagementPolicy                | [tenantAppManagementPolicy](tenantappmanagementpolicy.md)                                                 | A política em todo o locatário que impõe restrições de gerenciamento de aplicativos para todos os aplicativos e entidades de serviço.                                                        |
| externalIdentitiesPolicy                  | [externalIdentitiesPolicy](externalidentitiespolicy.md)                                                   | Representa a política de todo o locatário que controla se os usuários externos podem deixar um locatário Azure AD por meio de controles de autoatendimento. |
| featureRolloutPolicies                    | [Coleção featureRolloutPolicy](featurerolloutpolicy.md)                                                | A política de distribuição de recursos associada a um objeto de diretório.                                                                                                       |
| homeRealmDiscoveryPolicies                | Conjunto [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)                                        | A política para controlar o Azure AD de autenticação para usuários federados.                                                                                          |
| identitySecurityDefaultsEnforcementPolicy | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)                 | A política que representa os padrões de segurança que protegem contra ataques comuns.                                                                                |
| mobileAppManagementPolicies               | [coleção mobilityManagementPolicy](mobilitymanagementpolicy.md)                                        | A política que define a configuração de registro automático para um aplicativo de gerenciamento de mobilidade (MDM ou MAM).                                                            |
| permissionGrantPolicies                   | conjunto [permissionGrantPolicy](permissiongrantpolicy.md)                                              | A política que especifica as condições sob as quais o consentimento pode ser concedido.                                                                                         |
| roleManagementPolicies                    | [Coleção unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)                     | Representa as políticas de gerenciamento de função.                                                                                                                             |
| roleManagementPolicyAssignments           | [Coleção unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) | Representa as atribuições de política de gerenciamento de função.                                                                                                                   |
| tokenIssuancePolicies                     | coleção [tokenIssuancePolicy](tokenissuancepolicy.md)                                                  | A política que especifica as características dos tokens SAML emitidos pelo Azure AD.                                                                                     |
| tokenLifetimePolicies                     | Conjunto [tokenLifetimePolicy](tokenlifetimepolicy.md)                                                  | A política que controla o tempo de vida de um token de acesso JWT, um token de ID ou um token SAML 1.1/2.0 emitido pelo Azure AD.                                                |

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
