---
title: Tipo de recurso policyRoot
description: Tipo de recurso expondo propriedades de navegação para o singleton de políticas.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: dc54d92a520961441545962fa996efd39fa8ca3d
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604479"
---
# <a name="policyroot-resource-type"></a>Tipo de recurso policyRoot

Namespace: microsoft.graph

Tipo de recurso expondo propriedades de navegação para o singleton de políticas. Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
Nenhum

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da política. Herdado da [entidade](../resources/entity.md).|


## <a name="relationships"></a>Relações
| Relação                              | Tipo                                                                                                      | Descrição                                                                                                                                                          |
|:------------------------------------------|:----------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| activityBasedTimeoutPolicies              | [Coleção activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md)                                    | A política que controla o tempo limite de ociosidade para sessões da Web para aplicativos.                                                                                        |
| adminConsentRequestPolicy                 | [adminConsentRequestPolicy](adminconsentrequestpolicy.md)                                                 | A política pela qual as solicitações de consentimento são criadas e gerenciadas para todo o locatário.                                                                                  |
| authenticationFlowsPolicy                 | [authenticationFlowsPolicy](authenticationflowspolicy.md)                                                 | A configuração de política da experiência de inscrição por autoatendimento de usuários externos.                                                                                   |
| authenticationMethodsPolicy               | [authenticationMethodsPolicy](authenticationmethodspolicy.md)                                             | Os métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a MFA (autenticação multifator) no Azure Active Directory (Azure AD). |
| authorizationPolicy                       | [coleção authorizationPolicy](authorizationpolicy.md)                                                  | A política que controla as Azure AD de autorização.                                                                                                            |
| claimsMappingPolicies                     | Conjunto [claimsMappingPolicy](claimsmappingpolicy.md)                                                  | As políticas de mapeamento de declaração para protocolos WS-Fed, SAML, OAuth 2.0 e OpenID Connect, para tokens emitidos para um aplicativo específico.                                   |
| crossTenantAccessPolicy                   | [crossTenantAccessPolicy](crosstenantaccesspolicy.md)                           | As regras personalizadas que definem um cenário de acesso ao interagir com locatários de Azure AD externos.                                                                                                                     |
| conditionalAccessPolicies                 | [conditionalAccessPolicy](conditionalaccesspolicy.md)                                                     | As regras personalizadas que definem um cenário de acesso.                                                                                                                     |
| featureRolloutPolicies                    | [Coleção featureRolloutPolicy](featurerolloutpolicy.md)                                                | A política de distribuição de recursos associada a um objeto de diretório.                                                                                                       |
| homeRealmDiscoveryPolicies                | Conjunto [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)                                        | A política para controlar o Azure AD de autenticação para usuários federados.                                                                                          |
| identitySecurityDefaultsEnforcementPolicy | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)                 | A política que representa os padrões de segurança que protegem contra ataques comuns.                                                                                |
| permissionGrantPolicies                   | conjunto [permissionGrantPolicy](permissiongrantpolicy.md)                                              | A política que especifica as condições sob as quais o consentimento pode ser concedido.                                                                                         |
|roleManagementPolicies|[Coleção unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)| Especifica as várias políticas associadas a escopos e funções. |
|roleManagementPolicyAssignments|[Coleção unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)| A atribuição de uma política de gerenciamento de função a um objeto de definição de função. |
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
  "@odata.type": "#microsoft.graph.policyRoot",
  "id": "String (identifier)"
}
```

