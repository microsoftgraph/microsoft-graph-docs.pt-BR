---
title: tipo de recurso de synchronizationSecretKeyStringValuePair
description: 'Representa um único valor secreto. '
ms.openlocfilehash: 31aa5d983a0117591d3be75939b2c881a9782e7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040658"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="bcd5b-103">tipo de recurso de synchronizationSecretKeyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="bcd5b-103">synchronizationSecretKeyStringValuePair resource type</span></span>

> <span data-ttu-id="bcd5b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bcd5b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bcd5b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bcd5b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bcd5b-106">Representa um único valor secreto.</span><span class="sxs-lookup"><span data-stu-id="bcd5b-106">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="bcd5b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bcd5b-107">Properties</span></span>
| <span data-ttu-id="bcd5b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bcd5b-108">Property</span></span>     | <span data-ttu-id="bcd5b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcd5b-109">Type</span></span>   |<span data-ttu-id="bcd5b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcd5b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bcd5b-111">key</span><span class="sxs-lookup"><span data-stu-id="bcd5b-111">key</span></span>|<span data-ttu-id="bcd5b-112">String</span><span class="sxs-lookup"><span data-stu-id="bcd5b-112">String</span></span>| <span data-ttu-id="bcd5b-113">Os valores possíveis são: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken` , `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span><span class="sxs-lookup"><span data-stu-id="bcd5b-113">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="bcd5b-114">valor</span><span class="sxs-lookup"><span data-stu-id="bcd5b-114">value</span></span>|<span data-ttu-id="bcd5b-115">String</span><span class="sxs-lookup"><span data-stu-id="bcd5b-115">String</span></span>|<span data-ttu-id="bcd5b-116">O valor do segredo.</span><span class="sxs-lookup"><span data-stu-id="bcd5b-116">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bcd5b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bcd5b-117">JSON representation</span></span>

<span data-ttu-id="bcd5b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bcd5b-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSecretKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->