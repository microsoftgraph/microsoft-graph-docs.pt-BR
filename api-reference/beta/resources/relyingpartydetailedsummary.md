---
title: Tipo de recurso relyingPartyDetailedSummary
description: Representa uma parte de confiança no AD FS.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a19132396f88797735801ee782c3c13e12a5e2ca
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161121"
---
# <a name="relyingpartydetailedsummary-resource-type"></a><span data-ttu-id="7fb18-103">Tipo de recurso relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="7fb18-103">relyingPartyDetailedSummary resource type</span></span>

<span data-ttu-id="7fb18-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fb18-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fb18-105">Representa uma parte de confiança configurada com os Serviços de Federação do Active Directory (AD FS), seu uso agregado e se a configuração de terceiros de confiança pode ser migrada para o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7fb18-105">Represents a relying party configured with Active Directory Federation Services (AD FS), its aggregated usage, and whether the relying party configuration can be migrated to Azure Active Directory.</span></span>

## <a name="methods"></a><span data-ttu-id="7fb18-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="7fb18-106">Methods</span></span>

| <span data-ttu-id="7fb18-107">Método</span><span class="sxs-lookup"><span data-stu-id="7fb18-107">Method</span></span>       | <span data-ttu-id="7fb18-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7fb18-108">Return Type</span></span> | <span data-ttu-id="7fb18-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fb18-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7fb18-110">List</span><span class="sxs-lookup"><span data-stu-id="7fb18-110">List</span></span>](../api/relyingpartydetailedsummary-list.md) | [<span data-ttu-id="7fb18-111">relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="7fb18-111">relyingPartyDetailedSummary</span></span>](relyingpartydetailedsummary.md) | <span data-ttu-id="7fb18-112">Recupere uma lista de **objetos relyingPartyDetailedSummary.**</span><span class="sxs-lookup"><span data-stu-id="7fb18-112">Retrieve a list of **relyingPartyDetailedSummary** objects.</span></span> |


## <a name="properties"></a><span data-ttu-id="7fb18-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7fb18-113">Properties</span></span>

| <span data-ttu-id="7fb18-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7fb18-114">Property</span></span>     | <span data-ttu-id="7fb18-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="7fb18-115">Type</span></span>        | <span data-ttu-id="7fb18-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fb18-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7fb18-117">id</span><span class="sxs-lookup"><span data-stu-id="7fb18-117">id</span></span>|<span data-ttu-id="7fb18-118">String</span><span class="sxs-lookup"><span data-stu-id="7fb18-118">String</span></span>| <span data-ttu-id="7fb18-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7fb18-119">Read-only.</span></span> <span data-ttu-id="7fb18-120">Identificador exclusivo gerado no nível da API.</span><span class="sxs-lookup"><span data-stu-id="7fb18-120">Unique Identifier generated at API level.</span></span>| 
|<span data-ttu-id="7fb18-121">relyingPartyId</span><span class="sxs-lookup"><span data-stu-id="7fb18-121">relyingPartyId</span></span>|<span data-ttu-id="7fb18-122">String</span><span class="sxs-lookup"><span data-stu-id="7fb18-122">String</span></span>|<span data-ttu-id="7fb18-123">Esse identificador é usado para identificar a parte de confiança para este Serviço de Federação.</span><span class="sxs-lookup"><span data-stu-id="7fb18-123">This identifier is used to identify the relying party to this Federation Service.</span></span> <span data-ttu-id="7fb18-124">Ele é usado ao emissão de declarações para a parte de confiança.</span><span class="sxs-lookup"><span data-stu-id="7fb18-124">It is used when issuing claims to the relying party.</span></span>|
|<span data-ttu-id="7fb18-125">serviceId</span><span class="sxs-lookup"><span data-stu-id="7fb18-125">serviceId</span></span>|<span data-ttu-id="7fb18-126">String</span><span class="sxs-lookup"><span data-stu-id="7fb18-126">String</span></span>|<span data-ttu-id="7fb18-127">Identifica exclusivamente a floresta do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7fb18-127">Uniquely identifies the Active Directory forest.</span></span>|
|<span data-ttu-id="7fb18-128">migrationStatus</span><span class="sxs-lookup"><span data-stu-id="7fb18-128">migrationStatus</span></span>|<span data-ttu-id="7fb18-129">string</span><span class="sxs-lookup"><span data-stu-id="7fb18-129">string</span></span>| <span data-ttu-id="7fb18-130">Indicação se o aplicativo pode ser movido para o Azure AD ou exigir mais investigação.</span><span class="sxs-lookup"><span data-stu-id="7fb18-130">Indication of whether the application can be moved to Azure AD or require more investigation.</span></span> <span data-ttu-id="7fb18-131">Os valores possíveis são: `ready`, `needsReview`, `additionalStepsRequired`.</span><span class="sxs-lookup"><span data-stu-id="7fb18-131">Possible values are: `ready`, `needsReview`, `additionalStepsRequired`.</span></span>|
|<span data-ttu-id="7fb18-132">migrationValidationDetails</span><span class="sxs-lookup"><span data-stu-id="7fb18-132">migrationValidationDetails</span></span>|<span data-ttu-id="7fb18-133">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="7fb18-133">[keyValuePair](keyvaluepair.md) collection</span></span>|<span data-ttu-id="7fb18-134">Especifica todas as validações feitas nos detalhes de configuração de aplicativos para avaliar se o aplicativo está pronto para ser movido para o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7fb18-134">Specifies all the validations check done on applications configuration details to evaluate if the application is ready to be moved to Azure AD.</span></span> <span data-ttu-id="7fb18-135">Os nomes possíveis `AdditionalWSFedEndpointCheckResult` são:  `AllowedAuthenticationClassReferencesCheckResult` , , , , , , , , , `AlwaysRequireAuthenticationCheckResult` , ,   `AutoUpdateEnabledCheckResult` , , , `ClaimsProviderNameCheckResult` `EncryptClaimsCheckResult`  `EncryptedNameIdRequiredCheckResult` , `MonitoringEnabledCheckResult` `NotBeforeSkewCheckResult`  `RequestMFAFromClaimsProvidersCheckResult` `SignedSamlRequestsRequiredCheckResult` `AdditionalAuthenticationRulesCheckResult` `TokenLifetimeCheckResult`  `DelegationAuthorizationRulesCheckResult` `IssuanceAuthorizationRulesCheckResult` `IssuanceTransformRulesCheckResult` .</span><span class="sxs-lookup"><span data-stu-id="7fb18-135">Possible names are: `AdditionalWSFedEndpointCheckResult`,  `AllowedAuthenticationClassReferencesCheckResult`, `AlwaysRequireAuthenticationCheckResult`,   `AutoUpdateEnabledCheckResult`, `ClaimsProviderNameCheckResult`, `EncryptClaimsCheckResult`,  `EncryptedNameIdRequiredCheckResult`, `MonitoringEnabledCheckResult`,`NotBeforeSkewCheckResult`,  `RequestMFAFromClaimsProvidersCheckResult`, `SignedSamlRequestsRequiredCheckResult`, `AdditionalAuthenticationRulesCheckResult`, `TokenLifetimeCheckResult`,  `DelegationAuthorizationRulesCheckResult`, `IssuanceAuthorizationRulesCheckResult`, `IssuanceTransformRulesCheckResult`.</span></span> <span data-ttu-id="7fb18-136">Os valores de resultado possíveis `0` `1` são , ou `2` .</span><span class="sxs-lookup"><span data-stu-id="7fb18-136">Possible result values are `0`, `1`, or `2`.</span></span> <span data-ttu-id="7fb18-137">`0` quando a verificação de validação passou, `1` quando a verificação de validação falhou e quando a verificação de `2` validação é um aviso.</span><span class="sxs-lookup"><span data-stu-id="7fb18-137">`0` when the validation check passed, `1` when the validation check failed and `2` when the validation check is a warning.</span></span> |
|<span data-ttu-id="7fb18-138">relyingPartyName</span><span class="sxs-lookup"><span data-stu-id="7fb18-138">relyingPartyName</span></span>|<span data-ttu-id="7fb18-139">String</span><span class="sxs-lookup"><span data-stu-id="7fb18-139">String</span></span>|<span data-ttu-id="7fb18-140">Nome do aplicativo ou outra entidade na Internet que usa um provedor de identidade para autenticar um usuário que deseja fazer logoff.</span><span class="sxs-lookup"><span data-stu-id="7fb18-140">Name of application or other entity on the internet that uses an identity provider to authenticate a user who wants to log in.</span></span>|
|<span data-ttu-id="7fb18-141">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="7fb18-141">failedSignInCount</span></span>|<span data-ttu-id="7fb18-142">Int64</span><span class="sxs-lookup"><span data-stu-id="7fb18-142">Int64</span></span>| <span data-ttu-id="7fb18-143">Número de falhas ao entrar no Serviço de Federação do Active Directory no período especificado.</span><span class="sxs-lookup"><span data-stu-id="7fb18-143">Number of failed sign in on Active Directory Federation Service in the period specified.</span></span> |
|<span data-ttu-id="7fb18-144">replyUrls</span><span class="sxs-lookup"><span data-stu-id="7fb18-144">replyUrls</span></span>|<span data-ttu-id="7fb18-145">String collection</span><span class="sxs-lookup"><span data-stu-id="7fb18-145">String collection</span></span>|<span data-ttu-id="7fb18-146">Especifica onde a confiança espera receber o token.</span><span class="sxs-lookup"><span data-stu-id="7fb18-146">Specifies where the relying party expects to receive the token.</span></span>|
|<span data-ttu-id="7fb18-147">signInSuccessRate</span><span class="sxs-lookup"><span data-stu-id="7fb18-147">signInSuccessRate</span></span>|<span data-ttu-id="7fb18-148">Duplo</span><span class="sxs-lookup"><span data-stu-id="7fb18-148">Double</span></span>|<span data-ttu-id="7fb18-149">Número de êxito /(número de êxito + número de falhas de logins) no Serviço de Federação do Active Directory no período especificado.</span><span class="sxs-lookup"><span data-stu-id="7fb18-149">Number of successful / (number of successful + number of failed sign ins) on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="7fb18-150">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="7fb18-150">successfulSignInCount</span></span>|<span data-ttu-id="7fb18-151">Int64</span><span class="sxs-lookup"><span data-stu-id="7fb18-151">Int64</span></span>|<span data-ttu-id="7fb18-152">Número de logins bem-sucedidos no Serviço de Federação do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7fb18-152">Number of successful sign ins on Active Directory Federation Service.</span></span>|
|<span data-ttu-id="7fb18-153">totalSignInCount</span><span class="sxs-lookup"><span data-stu-id="7fb18-153">totalSignInCount</span></span>|<span data-ttu-id="7fb18-154">Int64</span><span class="sxs-lookup"><span data-stu-id="7fb18-154">Int64</span></span>|<span data-ttu-id="7fb18-155">Número de tentativas bem-sucedidas + falhas de logins no Serviço de Federação do Active Directory no período especificado.</span><span class="sxs-lookup"><span data-stu-id="7fb18-155">Number of successful + failed sign ins failed sign ins on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="7fb18-156">uniqueUserCount</span><span class="sxs-lookup"><span data-stu-id="7fb18-156">uniqueUserCount</span></span>|<span data-ttu-id="7fb18-157">Int64</span><span class="sxs-lookup"><span data-stu-id="7fb18-157">Int64</span></span>|<span data-ttu-id="7fb18-158">Número de usuários exclusivos que entraram no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7fb18-158">Number of unique users that have signed into the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fb18-159">Relações</span><span class="sxs-lookup"><span data-stu-id="7fb18-159">Relationships</span></span>

<span data-ttu-id="7fb18-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7fb18-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7fb18-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7fb18-161">JSON representation</span></span>

<span data-ttu-id="7fb18-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7fb18-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relyingPartyDetailedSummary",
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


