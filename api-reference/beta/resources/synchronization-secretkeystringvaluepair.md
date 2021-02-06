---
title: Tipo de recurso synchronizationSecretKeyStringValuePair
description: Representa um valor secreto único.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: da408988c61ffa8d608fe7f36b5925107731d714
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129364"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="dfe35-103">Tipo de recurso synchronizationSecretKeyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="dfe35-103">synchronizationSecretKeyStringValuePair resource type</span></span>

<span data-ttu-id="dfe35-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfe35-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfe35-105">Representa um valor secreto único.</span><span class="sxs-lookup"><span data-stu-id="dfe35-105">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="dfe35-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dfe35-106">Properties</span></span>
| <span data-ttu-id="dfe35-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dfe35-107">Property</span></span>     | <span data-ttu-id="dfe35-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfe35-108">Type</span></span>   |<span data-ttu-id="dfe35-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfe35-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfe35-110">key</span><span class="sxs-lookup"><span data-stu-id="dfe35-110">key</span></span>|<span data-ttu-id="dfe35-111">String</span><span class="sxs-lookup"><span data-stu-id="dfe35-111">String</span></span>| <span data-ttu-id="dfe35-112">Os valores possíveis são: `None` , , , , , , `UserName` `Password` `SecretToken` `AppKey` `BaseAddress` `ClientIdentifier` `ClientSecret` `SingleSignOnType` `Sandbox` `Url` `Domain` , `ConsumerKey` `ConsumerSecret` , `TokenKey` `TokenExpiration` `Oauth2AccessToken` `Oauth2AccessTokenCreationTime` `Oauth2RefreshToken` , `SyncAll` `InstanceName` `Oauth2ClientId` `Oauth2ClientSecret` `CompanyId` `UpdateKeyOnSoftDelete` `SynchronizationSchedule` `SystemOfRecord` `SandboxName` `EnforceDomain` `SyncNotificationSettings` `Server` `PerformInboundEntitlementGrants` `HardDeletesEnabled` `SyncAgentCompatibilityKey` , `SyncAgentADContainer` `ValidateDomain` `TestReferences` .</span><span class="sxs-lookup"><span data-stu-id="dfe35-112">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="dfe35-113">value</span><span class="sxs-lookup"><span data-stu-id="dfe35-113">value</span></span>|<span data-ttu-id="dfe35-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dfe35-114">String</span></span>|<span data-ttu-id="dfe35-115">O valor do segredo.</span><span class="sxs-lookup"><span data-stu-id="dfe35-115">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dfe35-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dfe35-116">JSON representation</span></span>

<span data-ttu-id="dfe35-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dfe35-117">The following is a JSON representation of the resource.</span></span>

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


