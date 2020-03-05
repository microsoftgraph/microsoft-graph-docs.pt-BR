---
title: tipo de recurso synchronizationSecretKeyStringValuePair
description: 'Representa um único valor secreto. '
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 437bbd9b2f266dc8176657e670ea973904efcbe4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520111"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="7989c-103">tipo de recurso synchronizationSecretKeyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="7989c-103">synchronizationSecretKeyStringValuePair resource type</span></span>

<span data-ttu-id="7989c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7989c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7989c-105">Representa um único valor secreto.</span><span class="sxs-lookup"><span data-stu-id="7989c-105">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="7989c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7989c-106">Properties</span></span>
| <span data-ttu-id="7989c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7989c-107">Property</span></span>     | <span data-ttu-id="7989c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7989c-108">Type</span></span>   |<span data-ttu-id="7989c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7989c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7989c-110">key</span><span class="sxs-lookup"><span data-stu-id="7989c-110">key</span></span>|<span data-ttu-id="7989c-111">String</span><span class="sxs-lookup"><span data-stu-id="7989c-111">String</span></span>| <span data-ttu-id="7989c-112">Os valores possíveis são `None`: `UserName`, `Password`, `SecretToken`, `AppKey` `BaseAddress` `ClientIdentifier` `ClientSecret` `SingleSignOnType` `SyncAgentCompatibilityKey` `ValidateDomain` `TestReferences` `SyncAgentADContainer` `SyncNotificationSettings` `EnforceDomain` `Server` `PerformInboundEntitlementGrants` `HardDeletesEnabled`,, `SandboxName`,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,, `Sandbox` `Url` `Domain` `ConsumerKey` `ConsumerSecret` `TokenKey` `TokenExpiration` `Oauth2AccessToken` `Oauth2AccessTokenCreationTime` `Oauth2RefreshToken` `SyncAll` `InstanceName` `Oauth2ClientId` `Oauth2ClientSecret` `CompanyId` `UpdateKeyOnSoftDelete` `SynchronizationSchedule` `SystemOfRecord`</span><span class="sxs-lookup"><span data-stu-id="7989c-112">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="7989c-113">value</span><span class="sxs-lookup"><span data-stu-id="7989c-113">value</span></span>|<span data-ttu-id="7989c-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7989c-114">String</span></span>|<span data-ttu-id="7989c-115">O valor do segredo.</span><span class="sxs-lookup"><span data-stu-id="7989c-115">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7989c-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7989c-116">JSON representation</span></span>

<span data-ttu-id="7989c-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7989c-117">The following is a JSON representation of the resource.</span></span>

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
