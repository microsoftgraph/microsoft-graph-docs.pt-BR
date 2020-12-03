---
title: tipo de recurso relyingPartyDetailedSummary
description: Representa uma terceira parte confiável no AD FS.
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a3a6fd0ad84ce8e41902cd7c0e82a314fb1aa3ca
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524712"
---
# <a name="relyingpartydetailedsummary-resource-type"></a>tipo de recurso relyingPartyDetailedSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma terceira parte confiável configurada com o AD FS (serviços de Federação do Active Directory), seu uso agregado e se a configuração da terceira parte confiável pode ser migrada para o Azure Active Directory.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/relyingpartydetailedsummary-list.md) | [relyingPartyDetailedSummary](relyingpartydetailedsummary.md) | Recupere uma lista de objetos **relyingPartyDetailedSummary** . |


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura. Identificador exclusivo gerado no nível da API.| 
|relyingPartyId|String|Este identificador é usado para identificar a terceira parte confiável para este serviço de Federação. Ele é usado durante a emissão de declarações para a terceira parte confiável.|
|serviceId|String|Identifica exclusivamente a floresta do Active Directory.|
|migrationStatus|cadeia de caracteres| Indica se o aplicativo pode ser movido para o Azure AD ou exigir mais investigações. Os valores possíveis são: `ready`, `needsReview`, `additionalStepsRequired`.|
|migrationValidationDetails|Coleção [keyValuePair](keyvaluepair.md)|Especifica todas as validações realizadas nos detalhes de configuração de aplicativos para avaliar se o aplicativo está pronto para ser movido para o Azure AD. Os nomes possíveis são:, `AdditionalWSFedEndpointCheckResult`  `AllowedAuthenticationClassReferencesCheckResult` ,,,, `AlwaysRequireAuthenticationCheckResult`   `AutoUpdateEnabledCheckResult` `ClaimsProviderNameCheckResult` `EncryptClaimsCheckResult` ,  `EncryptedNameIdRequiredCheckResult` , `MonitoringEnabledCheckResult` , `NotBeforeSkewCheckResult` ,  `RequestMFAFromClaimsProvidersCheckResult` , `SignedSamlRequestsRequiredCheckResult` , `AdditionalAuthenticationRulesCheckResult` , `TokenLifetimeCheckResult`  `DelegationAuthorizationRulesCheckResult` `IssuanceAuthorizationRulesCheckResult` `IssuanceTransformRulesCheckResult` ,,. Os possíveis valores de resultado são `0` , `1` ou `2` . `0` Quando a verificação de validação é aprovada, `1` quando a verificação de validação falhou e `2` quando a verificação de validação é um aviso. |
|relyingPartyName|String|Nome do aplicativo ou outra entidade na Internet que usa um provedor de identidade para autenticar um usuário que deseja fazer logon.|
|failedSignInCount|Int64| Número de falhas de entrada no serviço de Federação do Active Directory no período especificado. |
|replyUrls|String collection|Especifica onde a terceira parte confiável espera receber o token.|
|signInSuccessRate|Duplo|Número de bem-sucedido/(número de êxito + número de entradas com falha) no serviço de Federação do Active Directory no período especificado.|
|successfulSignInCount|Int64|Número de entradas bem-sucedidas no serviço de Federação do Active Directory.|
|totalSignInCount|Int64|Número de tentativas com êxito + falhas de entradas no serviço de Federação do Active Directory no período especificado.|
|uniqueUserCount|Int64|Número de usuários exclusivos que entraram no aplicativo.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relyingPartyDetailedSummary",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "failedSignInCount": 10,
  "id": "String (identifier)",
  "migrationStatus": "ready | needsReview | additionalStepsRequired",
  "migrationValidationDetails": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "relyingPartyId": "String",
  "relyingPartyName": "String",
  "replyUrls": ["String"],
  "serviceId": "String (identifier)",
  "signInSuccessRate": 90.0,
  "successfulSignInCount": 90,
  "totalSignInCount": 100,
  "uniqueUserCount": 10
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "relyingPartyDetailedSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


