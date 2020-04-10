---
title: tipo de recurso synchronizationSecretKeyStringValuePair
description: Representa um único valor secreto.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b2c5929b7ba00a12cf66cd3f013dbf31446aba19
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217581"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a>tipo de recurso synchronizationSecretKeyStringValuePair

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um único valor secreto. 

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|key|Cadeia de Caracteres| Os valores possíveis são `None`: `UserName`, `Password`, `SecretToken`, `AppKey` `BaseAddress` `ClientIdentifier` `ClientSecret` `SingleSignOnType` `SyncAgentCompatibilityKey` `ValidateDomain` `TestReferences` `SyncAgentADContainer` `SyncNotificationSettings` `EnforceDomain` `Server` `PerformInboundEntitlementGrants` `HardDeletesEnabled`,, `SandboxName`,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,, `Sandbox` `Url` `Domain` `ConsumerKey` `ConsumerSecret` `TokenKey` `TokenExpiration` `Oauth2AccessToken` `Oauth2AccessTokenCreationTime` `Oauth2RefreshToken` `SyncAll` `InstanceName` `Oauth2ClientId` `Oauth2ClientSecret` `CompanyId` `UpdateKeyOnSoftDelete` `SynchronizationSchedule` `SystemOfRecord`|
|value|Cadeia de caracteres|O valor do segredo.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
}-->

```json
{
  "key": "String",
  "value": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSecretKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
