---
title: tipo de recurso synchronizationSecretKeyStringValuePair
description: Representa um único valor secreto.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: abe0e071c94de399cf351aecea32b51ea9c09d51
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023867"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="b36d3-103">tipo de recurso synchronizationSecretKeyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="b36d3-103">synchronizationSecretKeyStringValuePair resource type</span></span>

<span data-ttu-id="b36d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b36d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b36d3-105">Representa um único valor secreto.</span><span class="sxs-lookup"><span data-stu-id="b36d3-105">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="b36d3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b36d3-106">Properties</span></span>
| <span data-ttu-id="b36d3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b36d3-107">Property</span></span>     | <span data-ttu-id="b36d3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b36d3-108">Type</span></span>   |<span data-ttu-id="b36d3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b36d3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b36d3-110">key</span><span class="sxs-lookup"><span data-stu-id="b36d3-110">key</span></span>|<span data-ttu-id="b36d3-111">String</span><span class="sxs-lookup"><span data-stu-id="b36d3-111">String</span></span>| <span data-ttu-id="b36d3-112">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,, `None` `UserName` `Password` `SecretToken` `AppKey` `BaseAddress` `ClientIdentifier` `ClientSecret` `SingleSignOnType` `Sandbox` `Url` `Domain` `ConsumerKey` `ConsumerSecret` `TokenKey` `TokenExpiration` `Oauth2AccessToken` `Oauth2AccessTokenCreationTime` `Oauth2RefreshToken` `SyncAll` `InstanceName` `Oauth2ClientId` `Oauth2ClientSecret` `CompanyId` `UpdateKeyOnSoftDelete` `SynchronizationSchedule` `SystemOfRecord` `SandboxName` `EnforceDomain` `SyncNotificationSettings` `Server` `PerformInboundEntitlementGrants` `HardDeletesEnabled` `SyncAgentCompatibilityKey` `SyncAgentADContainer` , `ValidateDomain` `TestReferences` ,,,,,,,,,,,,,,,</span><span class="sxs-lookup"><span data-stu-id="b36d3-112">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="b36d3-113">value</span><span class="sxs-lookup"><span data-stu-id="b36d3-113">value</span></span>|<span data-ttu-id="b36d3-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b36d3-114">String</span></span>|<span data-ttu-id="b36d3-115">O valor do segredo.</span><span class="sxs-lookup"><span data-stu-id="b36d3-115">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b36d3-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b36d3-116">JSON representation</span></span>

<span data-ttu-id="b36d3-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b36d3-117">The following is a JSON representation of the resource.</span></span>

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


