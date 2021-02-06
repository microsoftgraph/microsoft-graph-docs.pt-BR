---
title: Tipo de recurso relyingPartyDetailedSummary
description: Representa uma parte de confiança no AD FS.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c1c0195302c4b01e39a6223797567c750807e9f6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136224"
---
# <a name="relyingpartydetailedsummary-resource-type"></a>Tipo de recurso relyingPartyDetailedSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma parte de confiança configurada com os Serviços de Federação do Active Directory (AD FS), seu uso agregado e se a configuração de terceiros de confiança pode ser migrada para o Azure Active Directory.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/relyingpartydetailedsummary-list.md) | [relyingPartyDetailedSummary](relyingpartydetailedsummary.md) | Recupere uma lista de **objetos relyingPartyDetailedSummary.** |


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura. Identificador exclusivo gerado no nível da API.| 
|relyingPartyId|String|Esse identificador é usado para identificar a parte de confiança para este Serviço de Federação. Ele é usado ao emissão de declarações para a parte de confiança.|
|serviceId|String|Identifica exclusivamente a floresta do Active Directory.|
|migrationStatus|string| Indicação se o aplicativo pode ser movido para o Azure AD ou exigir mais investigação. Os valores possíveis são: `ready`, `needsReview`, `additionalStepsRequired`.|
|migrationValidationDetails|Coleção [keyValuePair](keyvaluepair.md)|Especifica todas as validações feitas nos detalhes de configuração de aplicativos para avaliar se o aplicativo está pronto para ser movido para o Azure AD. Os nomes possíveis `AdditionalWSFedEndpointCheckResult` são:  `AllowedAuthenticationClassReferencesCheckResult` , , , , , , , , , `AlwaysRequireAuthenticationCheckResult` , ,   `AutoUpdateEnabledCheckResult` , , , `ClaimsProviderNameCheckResult` `EncryptClaimsCheckResult`  `EncryptedNameIdRequiredCheckResult` , `MonitoringEnabledCheckResult` `NotBeforeSkewCheckResult`  `RequestMFAFromClaimsProvidersCheckResult` `SignedSamlRequestsRequiredCheckResult` `AdditionalAuthenticationRulesCheckResult` `TokenLifetimeCheckResult`  `DelegationAuthorizationRulesCheckResult` `IssuanceAuthorizationRulesCheckResult` `IssuanceTransformRulesCheckResult` . Os valores de resultado possíveis `0` `1` são , ou `2` . `0` quando a verificação de validação passou, `1` quando a verificação de validação falhou e quando a verificação de `2` validação é um aviso. |
|relyingPartyName|String|Nome do aplicativo ou outra entidade na Internet que usa um provedor de identidade para autenticar um usuário que deseja fazer logoff.|
|failedSignInCount|Int64| Número de falhas ao entrar no Serviço de Federação do Active Directory no período especificado. |
|replyUrls|String collection|Especifica onde a confiança espera receber o token.|
|signInSuccessRate|Duplo|Número de êxito /(número de êxito + número de falhas de logins) no Serviço de Federação do Active Directory no período especificado.|
|successfulSignInCount|Int64|Número de logins bem-sucedidos no Serviço de Federação do Active Directory.|
|totalSignInCount|Int64|Número de tentativas bem-sucedidas + falhas de logins no Serviço de Federação do Active Directory no período especificado.|
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


