---
title: tipo de recurso synchronizationSecretKeyStringValuePair
description: 'Representa um único valor secreto. '
localization_priority: Normal
ms.openlocfilehash: a937063ea04bd3726932e423a065026d51b05aa4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523226"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="bd454-103">tipo de recurso synchronizationSecretKeyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="bd454-103">synchronizationSecretKeyStringValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd454-104">Representa um único valor secreto.</span><span class="sxs-lookup"><span data-stu-id="bd454-104">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="bd454-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bd454-105">Properties</span></span>
| <span data-ttu-id="bd454-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd454-106">Property</span></span>     | <span data-ttu-id="bd454-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd454-107">Type</span></span>   |<span data-ttu-id="bd454-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd454-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd454-109">key</span><span class="sxs-lookup"><span data-stu-id="bd454-109">key</span></span>|<span data-ttu-id="bd454-110">String</span><span class="sxs-lookup"><span data-stu-id="bd454-110">String</span></span>| <span data-ttu-id="bd454-111">Os valores possíveis são `None`: `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox` `Url` `Domain`,,, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken` ,,,,,,,, , `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span><span class="sxs-lookup"><span data-stu-id="bd454-111">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="bd454-112">value</span><span class="sxs-lookup"><span data-stu-id="bd454-112">value</span></span>|<span data-ttu-id="bd454-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd454-113">String</span></span>|<span data-ttu-id="bd454-114">O valor do segredo.</span><span class="sxs-lookup"><span data-stu-id="bd454-114">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bd454-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bd454-115">JSON representation</span></span>

<span data-ttu-id="bd454-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bd454-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-secretkeystringvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
