---
title: Tipo de recurso keyValuePair
description: Par de valores principais para parâmetros de ação.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 8897ea3d3788ce3fa846d845cb0854101b0b2ce7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960419"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="593a6-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="593a6-103">keyValuePair resource type</span></span>

<span data-ttu-id="593a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="593a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="593a6-105">Par de valores principais para parâmetros de ação.</span><span class="sxs-lookup"><span data-stu-id="593a6-105">Key value pair for action parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="593a6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="593a6-106">Properties</span></span>

| <span data-ttu-id="593a6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="593a6-107">Property</span></span>     | <span data-ttu-id="593a6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="593a6-108">Type</span></span>        | <span data-ttu-id="593a6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="593a6-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="593a6-110">nome</span><span class="sxs-lookup"><span data-stu-id="593a6-110">name</span></span>|<span data-ttu-id="593a6-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="593a6-111">String</span></span>|<span data-ttu-id="593a6-112">Nome desse par de valores-chave.</span><span class="sxs-lookup"><span data-stu-id="593a6-112">Name for this key-value pair.</span></span> <span data-ttu-id="593a6-113">Os nomes possíveis são: `AdditionalWSFedEndpointCheckResult` , , , , , , ,  `AllowedAuthenticationClassReferencesCheckResult` , , , `AlwaysRequireAuthenticationCheckResult` , ,   `AutoUpdateEnabledCheckResult` , , , `ClaimsProviderNameCheckResult` `EncryptClaimsCheckResult`  `EncryptedNameIdRequiredCheckResult` , `MonitoringEnabledCheckResult` `NotBeforeSkewCheckResult`  `RequestMFAFromClaimsProvidersCheckResult` `SignedSamlRequestsRequiredCheckResult` `AdditionalAuthenticationRulesCheckResult` `TokenLifetimeCheckResult`  `DelegationAuthorizationRulesCheckResult` `IssuanceAuthorizationRulesCheckResult` `IssuanceTransformRulesCheckResult` .</span><span class="sxs-lookup"><span data-stu-id="593a6-113">Possible names are: `AdditionalWSFedEndpointCheckResult`,  `AllowedAuthenticationClassReferencesCheckResult`, `AlwaysRequireAuthenticationCheckResult`,   `AutoUpdateEnabledCheckResult`, `ClaimsProviderNameCheckResult`, `EncryptClaimsCheckResult`,  `EncryptedNameIdRequiredCheckResult`, `MonitoringEnabledCheckResult`,`NotBeforeSkewCheckResult`,  `RequestMFAFromClaimsProvidersCheckResult`, `SignedSamlRequestsRequiredCheckResult`, `AdditionalAuthenticationRulesCheckResult`, `TokenLifetimeCheckResult`,  `DelegationAuthorizationRulesCheckResult`, `IssuanceAuthorizationRulesCheckResult`, `IssuanceTransformRulesCheckResult`.</span></span>|
|<span data-ttu-id="593a6-114">value</span><span class="sxs-lookup"><span data-stu-id="593a6-114">value</span></span>|<span data-ttu-id="593a6-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="593a6-115">String</span></span>|<span data-ttu-id="593a6-116">Valor para esse par de valores-chave.</span><span class="sxs-lookup"><span data-stu-id="593a6-116">Value for this key-value pair.</span></span> <span data-ttu-id="593a6-117">Os valores de resultados possíveis são (quando a verificação de validação passou), (quando a verificação de validação falhou) ou (quando a verificação de validação `0` `1` é um `2` aviso).</span><span class="sxs-lookup"><span data-stu-id="593a6-117">Possible result values are `0` (when the validation check passed), `1` (when the validation check failed), or `2` (when the validation check is a warning).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="593a6-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="593a6-118">JSON representation</span></span>

<span data-ttu-id="593a6-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="593a6-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValuePair",
  "baseType": null
}-->

```json
{
  "name": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

