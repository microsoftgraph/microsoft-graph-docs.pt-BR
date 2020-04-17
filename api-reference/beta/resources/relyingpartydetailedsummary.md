---
title: tipo de recurso relyingPartyDetailedSummary
description: Representa uma terceira parte confiável no AD FS.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 306c20c31120d2f130562993d8ebd2d7e4083c23
ms.sourcegitcommit: d14e2abb24d9fbab519458b1c9fec890a5e51d70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2020
ms.locfileid: "43543449"
---
# <a name="relyingpartydetailedsummary-resource-type"></a><span data-ttu-id="6e474-103">tipo de recurso relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="6e474-103">relyingPartyDetailedSummary resource type</span></span>

<span data-ttu-id="6e474-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e474-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e474-105">Representa uma terceira parte confiável configurada com o AD FS (serviços de Federação do Active Directory), seu uso agregado e se a configuração da terceira parte confiável pode ser migrada para o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6e474-105">Represents a relying party configured with Active Directory Federation Services (AD FS), its aggregated usage, and whether the relying party configuration can be migrated to Azure Active Directory.</span></span>

## <a name="methods"></a><span data-ttu-id="6e474-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6e474-106">Methods</span></span>

| <span data-ttu-id="6e474-107">Método</span><span class="sxs-lookup"><span data-stu-id="6e474-107">Method</span></span>       | <span data-ttu-id="6e474-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6e474-108">Return Type</span></span> | <span data-ttu-id="6e474-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e474-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6e474-110">List</span><span class="sxs-lookup"><span data-stu-id="6e474-110">List</span></span>](../api/relyingpartydetailedsummary-list.md) | [<span data-ttu-id="6e474-111">relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="6e474-111">relyingPartyDetailedSummary</span></span>](relyingpartydetailedsummary.md) | <span data-ttu-id="6e474-112">Recupere uma lista de objetos **relyingPartyDetailedSummary** .</span><span class="sxs-lookup"><span data-stu-id="6e474-112">Retrieve a list of **relyingPartyDetailedSummary** objects.</span></span> |


## <a name="properties"></a><span data-ttu-id="6e474-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e474-113">Properties</span></span>

| <span data-ttu-id="6e474-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e474-114">Property</span></span>     | <span data-ttu-id="6e474-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e474-115">Type</span></span>        | <span data-ttu-id="6e474-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e474-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6e474-117">id</span><span class="sxs-lookup"><span data-stu-id="6e474-117">id</span></span>|<span data-ttu-id="6e474-118">String</span><span class="sxs-lookup"><span data-stu-id="6e474-118">String</span></span>| <span data-ttu-id="6e474-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6e474-119">Read-only.</span></span> <span data-ttu-id="6e474-120">Identificador exclusivo gerado no nível da API.</span><span class="sxs-lookup"><span data-stu-id="6e474-120">Unique Identifier generated at API level.</span></span>| 
|<span data-ttu-id="6e474-121">relyingPartyId</span><span class="sxs-lookup"><span data-stu-id="6e474-121">relyingPartyId</span></span>|<span data-ttu-id="6e474-122">String</span><span class="sxs-lookup"><span data-stu-id="6e474-122">String</span></span>|<span data-ttu-id="6e474-123">Este identificador é usado para identificar a terceira parte confiável para este serviço de Federação.</span><span class="sxs-lookup"><span data-stu-id="6e474-123">This identifier is used to identify the relying party to this Federation Service.</span></span> <span data-ttu-id="6e474-124">Ele é usado durante a emissão de declarações para a terceira parte confiável.</span><span class="sxs-lookup"><span data-stu-id="6e474-124">It is used when issuing claims to the relying party.</span></span>|
|<span data-ttu-id="6e474-125">serviceId</span><span class="sxs-lookup"><span data-stu-id="6e474-125">serviceId</span></span>|<span data-ttu-id="6e474-126">String</span><span class="sxs-lookup"><span data-stu-id="6e474-126">String</span></span>|<span data-ttu-id="6e474-127">Identifica exclusivamente a floresta do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6e474-127">Uniquely identifies the Active Directory forest.</span></span>|
|<span data-ttu-id="6e474-128">migrationStatus</span><span class="sxs-lookup"><span data-stu-id="6e474-128">migrationStatus</span></span>|<span data-ttu-id="6e474-129">string</span><span class="sxs-lookup"><span data-stu-id="6e474-129">string</span></span>| <span data-ttu-id="6e474-130">Indica se o aplicativo pode ser movido para o Azure AD ou exigir mais investigações.</span><span class="sxs-lookup"><span data-stu-id="6e474-130">Indication of whether the application can be moved to Azure AD or require more investigation.</span></span> <span data-ttu-id="6e474-131">Os valores possíveis são: `ready`, `needsReview`, `additionalStepsRequired`.</span><span class="sxs-lookup"><span data-stu-id="6e474-131">Possible values are: `ready`, `needsReview`, `additionalStepsRequired`.</span></span>|
|<span data-ttu-id="6e474-132">migrationValidationDetails</span><span class="sxs-lookup"><span data-stu-id="6e474-132">migrationValidationDetails</span></span>|<span data-ttu-id="6e474-133">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6e474-133">[keyValuePair](keyvaluepair.md) collection</span></span>|<span data-ttu-id="6e474-134">Especifica todas as validações realizadas nos detalhes de configuração de aplicativos para avaliar se o aplicativo está pronto para ser movido para o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6e474-134">Specifies all the validations check done on applications configuration details to evaluate if the application is ready to be moved to Azure AD.</span></span> <span data-ttu-id="6e474-135">Os nomes possíveis são `AdditionalWSFedEndpointCheckResult`: `AllowedAuthenticationClassReferencesCheckResult`, `AlwaysRequireAuthenticationCheckResult`, `AutoUpdateEnabledCheckResult`, `ClaimsProviderNameCheckResult`, `EncryptClaimsCheckResult`, `EncryptedNameIdRequiredCheckResult`, `MonitoringEnabledCheckResult`,`NotBeforeSkewCheckResult`, `RequestMFAFromClaimsProvidersCheckResult`, `SignedSamlRequestsRequiredCheckResult`, `AdditionalAuthenticationRulesCheckResult`, `TokenLifetimeCheckResult`, `DelegationAuthorizationRulesCheckResult` `IssuanceAuthorizationRulesCheckResult`,, `IssuanceTransformRulesCheckResult`.</span><span class="sxs-lookup"><span data-stu-id="6e474-135">Possible names are: `AdditionalWSFedEndpointCheckResult`,  `AllowedAuthenticationClassReferencesCheckResult`, `AlwaysRequireAuthenticationCheckResult`,   `AutoUpdateEnabledCheckResult`, `ClaimsProviderNameCheckResult`, `EncryptClaimsCheckResult`,  `EncryptedNameIdRequiredCheckResult`, `MonitoringEnabledCheckResult`,`NotBeforeSkewCheckResult`,  `RequestMFAFromClaimsProvidersCheckResult`, `SignedSamlRequestsRequiredCheckResult`, `AdditionalAuthenticationRulesCheckResult`, `TokenLifetimeCheckResult`,  `DelegationAuthorizationRulesCheckResult`, `IssuanceAuthorizationRulesCheckResult`, `IssuanceTransformRulesCheckResult`.</span></span> <span data-ttu-id="6e474-136">Os possíveis valores de `0`resultado `1`são, `2`ou.</span><span class="sxs-lookup"><span data-stu-id="6e474-136">Possible result values are `0`, `1`, or `2`.</span></span> <span data-ttu-id="6e474-137">`0`Quando a verificação de validação é `1` aprovada, quando a verificação de `2` validação falhou e quando a verificação de validação é um aviso.</span><span class="sxs-lookup"><span data-stu-id="6e474-137">`0` when the validation check passed, `1` when the validation check failed and `2` when the validation check is a warning.</span></span> |
|<span data-ttu-id="6e474-138">relyingPartyName</span><span class="sxs-lookup"><span data-stu-id="6e474-138">relyingPartyName</span></span>|<span data-ttu-id="6e474-139">String</span><span class="sxs-lookup"><span data-stu-id="6e474-139">String</span></span>|<span data-ttu-id="6e474-140">Nome do aplicativo ou outra entidade na Internet que usa um provedor de identidade para autenticar um usuário que deseja fazer logon.</span><span class="sxs-lookup"><span data-stu-id="6e474-140">Name of application or other entity on the internet that uses an identity provider to authenticate a user who wants to log in.</span></span>|
|<span data-ttu-id="6e474-141">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="6e474-141">failedSignInCount</span></span>|<span data-ttu-id="6e474-142">Int64</span><span class="sxs-lookup"><span data-stu-id="6e474-142">Int64</span></span>| <span data-ttu-id="6e474-143">Número de falhas de entrada no serviço de Federação do Active Directory no período especificado.</span><span class="sxs-lookup"><span data-stu-id="6e474-143">Number of failed sign in on Active Directory Federation Service in the period specified.</span></span> |
|<span data-ttu-id="6e474-144">replyUrls</span><span class="sxs-lookup"><span data-stu-id="6e474-144">replyUrls</span></span>|<span data-ttu-id="6e474-145">String collection</span><span class="sxs-lookup"><span data-stu-id="6e474-145">String collection</span></span>|<span data-ttu-id="6e474-146">Especifica onde a terceira parte confiável espera receber o token.</span><span class="sxs-lookup"><span data-stu-id="6e474-146">Specifies where the relying party expects to receive the token.</span></span>|
|<span data-ttu-id="6e474-147">signInSuccessRate</span><span class="sxs-lookup"><span data-stu-id="6e474-147">signInSuccessRate</span></span>|<span data-ttu-id="6e474-148">Duplo</span><span class="sxs-lookup"><span data-stu-id="6e474-148">Double</span></span>|<span data-ttu-id="6e474-149">Número de bem-sucedido/(número de êxito + número de entradas com falha) no serviço de Federação do Active Directory no período especificado.</span><span class="sxs-lookup"><span data-stu-id="6e474-149">Number of successful / (number of successful + number of failed sign ins) on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="6e474-150">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="6e474-150">successfulSignInCount</span></span>|<span data-ttu-id="6e474-151">Int64</span><span class="sxs-lookup"><span data-stu-id="6e474-151">Int64</span></span>|<span data-ttu-id="6e474-152">Número de entradas bem-sucedidas no serviço de Federação do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6e474-152">Number of successful sign ins on Active Directory Federation Service.</span></span>|
|<span data-ttu-id="6e474-153">totalSignInCount</span><span class="sxs-lookup"><span data-stu-id="6e474-153">totalSignInCount</span></span>|<span data-ttu-id="6e474-154">Int64</span><span class="sxs-lookup"><span data-stu-id="6e474-154">Int64</span></span>|<span data-ttu-id="6e474-155">Número de tentativas com êxito + falhas de entradas no serviço de Federação do Active Directory no período especificado.</span><span class="sxs-lookup"><span data-stu-id="6e474-155">Number of successful + failed sign ins failed sign ins on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="6e474-156">uniqueUserCount</span><span class="sxs-lookup"><span data-stu-id="6e474-156">uniqueUserCount</span></span>|<span data-ttu-id="6e474-157">Int64</span><span class="sxs-lookup"><span data-stu-id="6e474-157">Int64</span></span>|<span data-ttu-id="6e474-158">Número de usuários exclusivos que entraram no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6e474-158">Number of unique users that have signed into the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e474-159">Relações</span><span class="sxs-lookup"><span data-stu-id="6e474-159">Relationships</span></span>

<span data-ttu-id="6e474-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e474-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e474-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e474-161">JSON representation</span></span>

<span data-ttu-id="6e474-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e474-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relyingPartyDetailedSummary",
  "baseType": "",
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
