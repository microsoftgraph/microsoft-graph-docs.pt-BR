---
title: Tipo de recurso relyingPartyDetailedSummary
description: Representa uma parte de confiança no AD FS.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 6e840c47ed5170f95929d686fe9ff94be54ea1ad
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962109"
---
# <a name="relyingpartydetailedsummary-resource-type"></a>Tipo de recurso relyingPartyDetailedSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma parte de confiança configurada com os Serviços de Federação do Active Directory (AD FS), seu uso agregado e se a configuração de parte de base pode ser migrada para o Azure Active Directory.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/relyingpartydetailedsummary-list.md) | [relyingPartyDetailedSummary](relyingpartydetailedsummary.md) | Recupere uma lista **de objetos relyingPartyDetailedSummary.** |


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura. Identificador exclusivo gerado no nível da API.| 
|relyingPartyId|Cadeia de caracteres|Esse identificador é usado para identificar a parte de base para este Serviço de Federação. Ele é usado ao emissão de declarações à parte de base.|
|serviceId|Cadeia de caracteres|Identifica exclusivamente a floresta do Active Directory.|
|migrationStatus|migrationStatus| Indicação de se o aplicativo pode ser movido para o Azure AD ou exigir mais investigação. Os valores possíveis são: `ready`, `needsReview`, `additionalStepsRequired`, `unknownFutureValue`.|
|migrationValidationDetails|Coleção [keyValuePair](keyvaluepair.md)|Especifica todas as validações feitas em detalhes de configuração de aplicativos para avaliar se o aplicativo está pronto para ser movido para o Azure AD.|
|relyingPartyName|Cadeia de caracteres|Nome do aplicativo ou outra entidade na Internet que usa um provedor de identidade para autenticar um usuário que deseja fazer logoff.|
|failedSignInCount|Int64| Número de falha ao entrar no Serviço de Federação do Active Directory no período especificado. |
|replyUrls|String collection|Especifica onde a parte de confiança espera receber o token.|
|signInSuccessRate|Duplo|Número de êxito / (número de bem-sucedido + número de falhas de login) no Serviço de Federação do Active Directory no período especificado.|
|successfulSignInCount|Int64|Número de logins bem-sucedidos no Serviço de Federação do Active Directory.|
|totalSignInCount|Int64|Número de logins bem-sucedidos + com falha ao entrar no Serviço de Federação do Active Directory no período especificado.|
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


