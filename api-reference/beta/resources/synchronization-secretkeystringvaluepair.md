---
title: tipo de recurso synchronizationSecretKeyStringValuePair
description: 'Representa um único valor secreto. '
localization_priority: Normal
ms.openlocfilehash: 36ec5ababb6c972bad336b3cfa8da4d34ba66c55
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342871"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="d851c-103">tipo de recurso synchronizationSecretKeyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="d851c-103">synchronizationSecretKeyStringValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d851c-104">Representa um único valor secreto.</span><span class="sxs-lookup"><span data-stu-id="d851c-104">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="d851c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d851c-105">Properties</span></span>
| <span data-ttu-id="d851c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d851c-106">Property</span></span>     | <span data-ttu-id="d851c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d851c-107">Type</span></span>   |<span data-ttu-id="d851c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d851c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d851c-109">key</span><span class="sxs-lookup"><span data-stu-id="d851c-109">key</span></span>|<span data-ttu-id="d851c-110">String</span><span class="sxs-lookup"><span data-stu-id="d851c-110">String</span></span>| <span data-ttu-id="d851c-111">Os valores possíveis são `None`: `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox` `Url` `Domain`,,, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken` ,,,,,,,, , `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span><span class="sxs-lookup"><span data-stu-id="d851c-111">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="d851c-112">value</span><span class="sxs-lookup"><span data-stu-id="d851c-112">value</span></span>|<span data-ttu-id="d851c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d851c-113">String</span></span>|<span data-ttu-id="d851c-114">O valor do segredo.</span><span class="sxs-lookup"><span data-stu-id="d851c-114">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d851c-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d851c-115">JSON representation</span></span>

<span data-ttu-id="d851c-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d851c-116">The following is a JSON representation of the resource.</span></span>

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
