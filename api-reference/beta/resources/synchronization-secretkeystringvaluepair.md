---
title: tipo de recurso synchronizationSecretKeyStringValuePair
description: 'Representa um único valor secreto. '
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ad3348cea31567cedfca9b2626c81383ab8c6b8f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964687"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="8beb6-103">tipo de recurso synchronizationSecretKeyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="8beb6-103">synchronizationSecretKeyStringValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8beb6-104">Representa um único valor secreto.</span><span class="sxs-lookup"><span data-stu-id="8beb6-104">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="8beb6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8beb6-105">Properties</span></span>
| <span data-ttu-id="8beb6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8beb6-106">Property</span></span>     | <span data-ttu-id="8beb6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8beb6-107">Type</span></span>   |<span data-ttu-id="8beb6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8beb6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8beb6-109">key</span><span class="sxs-lookup"><span data-stu-id="8beb6-109">key</span></span>|<span data-ttu-id="8beb6-110">String</span><span class="sxs-lookup"><span data-stu-id="8beb6-110">String</span></span>| <span data-ttu-id="8beb6-111">Os valores possíveis são `None`: `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox` `Url` `Domain`,,, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken` ,,,,,,,, , `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span><span class="sxs-lookup"><span data-stu-id="8beb6-111">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="8beb6-112">value</span><span class="sxs-lookup"><span data-stu-id="8beb6-112">value</span></span>|<span data-ttu-id="8beb6-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8beb6-113">String</span></span>|<span data-ttu-id="8beb6-114">O valor do segredo.</span><span class="sxs-lookup"><span data-stu-id="8beb6-114">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8beb6-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8beb6-115">JSON representation</span></span>

<span data-ttu-id="8beb6-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8beb6-116">The following is a JSON representation of the resource.</span></span>

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
