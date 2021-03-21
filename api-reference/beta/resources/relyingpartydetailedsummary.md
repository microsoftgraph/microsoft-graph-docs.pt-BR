---
title: Tipo de recurso relyingPartyDetailedSummary
description: Representa uma parte de confiança no AD FS.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 6e840c47ed5170f95929d686fe9ff94be54ea1ad
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962109"
---
# <a name="relyingpartydetailedsummary-resource-type"></a><span data-ttu-id="c14ef-103">Tipo de recurso relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="c14ef-103">relyingPartyDetailedSummary resource type</span></span>

<span data-ttu-id="c14ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c14ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c14ef-105">Representa uma parte de confiança configurada com os Serviços de Federação do Active Directory (AD FS), seu uso agregado e se a configuração de parte de base pode ser migrada para o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c14ef-105">Represents a relying party configured with Active Directory Federation Services (AD FS), its aggregated usage, and whether the relying party configuration can be migrated to Azure Active Directory.</span></span>

## <a name="methods"></a><span data-ttu-id="c14ef-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c14ef-106">Methods</span></span>

| <span data-ttu-id="c14ef-107">Método</span><span class="sxs-lookup"><span data-stu-id="c14ef-107">Method</span></span>       | <span data-ttu-id="c14ef-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c14ef-108">Return Type</span></span> | <span data-ttu-id="c14ef-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c14ef-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c14ef-110">List</span><span class="sxs-lookup"><span data-stu-id="c14ef-110">List</span></span>](../api/relyingpartydetailedsummary-list.md) | [<span data-ttu-id="c14ef-111">relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="c14ef-111">relyingPartyDetailedSummary</span></span>](relyingpartydetailedsummary.md) | <span data-ttu-id="c14ef-112">Recupere uma lista **de objetos relyingPartyDetailedSummary.**</span><span class="sxs-lookup"><span data-stu-id="c14ef-112">Retrieve a list of **relyingPartyDetailedSummary** objects.</span></span> |


## <a name="properties"></a><span data-ttu-id="c14ef-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c14ef-113">Properties</span></span>

| <span data-ttu-id="c14ef-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c14ef-114">Property</span></span>     | <span data-ttu-id="c14ef-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="c14ef-115">Type</span></span>        | <span data-ttu-id="c14ef-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="c14ef-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c14ef-117">id</span><span class="sxs-lookup"><span data-stu-id="c14ef-117">id</span></span>|<span data-ttu-id="c14ef-118">String</span><span class="sxs-lookup"><span data-stu-id="c14ef-118">String</span></span>| <span data-ttu-id="c14ef-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c14ef-119">Read-only.</span></span> <span data-ttu-id="c14ef-120">Identificador exclusivo gerado no nível da API.</span><span class="sxs-lookup"><span data-stu-id="c14ef-120">Unique Identifier generated at API level.</span></span>| 
|<span data-ttu-id="c14ef-121">relyingPartyId</span><span class="sxs-lookup"><span data-stu-id="c14ef-121">relyingPartyId</span></span>|<span data-ttu-id="c14ef-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c14ef-122">String</span></span>|<span data-ttu-id="c14ef-123">Esse identificador é usado para identificar a parte de base para este Serviço de Federação.</span><span class="sxs-lookup"><span data-stu-id="c14ef-123">This identifier is used to identify the relying party to this Federation Service.</span></span> <span data-ttu-id="c14ef-124">Ele é usado ao emissão de declarações à parte de base.</span><span class="sxs-lookup"><span data-stu-id="c14ef-124">It is used when issuing claims to the relying party.</span></span>|
|<span data-ttu-id="c14ef-125">serviceId</span><span class="sxs-lookup"><span data-stu-id="c14ef-125">serviceId</span></span>|<span data-ttu-id="c14ef-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c14ef-126">String</span></span>|<span data-ttu-id="c14ef-127">Identifica exclusivamente a floresta do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c14ef-127">Uniquely identifies the Active Directory forest.</span></span>|
|<span data-ttu-id="c14ef-128">migrationStatus</span><span class="sxs-lookup"><span data-stu-id="c14ef-128">migrationStatus</span></span>|<span data-ttu-id="c14ef-129">migrationStatus</span><span class="sxs-lookup"><span data-stu-id="c14ef-129">migrationStatus</span></span>| <span data-ttu-id="c14ef-130">Indicação de se o aplicativo pode ser movido para o Azure AD ou exigir mais investigação.</span><span class="sxs-lookup"><span data-stu-id="c14ef-130">Indication of whether the application can be moved to Azure AD or require more investigation.</span></span> <span data-ttu-id="c14ef-131">Os valores possíveis são: `ready`, `needsReview`, `additionalStepsRequired`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c14ef-131">Possible values are: `ready`, `needsReview`, `additionalStepsRequired`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c14ef-132">migrationValidationDetails</span><span class="sxs-lookup"><span data-stu-id="c14ef-132">migrationValidationDetails</span></span>|<span data-ttu-id="c14ef-133">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c14ef-133">[keyValuePair](keyvaluepair.md) collection</span></span>|<span data-ttu-id="c14ef-134">Especifica todas as validações feitas em detalhes de configuração de aplicativos para avaliar se o aplicativo está pronto para ser movido para o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c14ef-134">Specifies all the validations check done on applications configuration details to evaluate if the application is ready to be moved to Azure AD.</span></span>|
|<span data-ttu-id="c14ef-135">relyingPartyName</span><span class="sxs-lookup"><span data-stu-id="c14ef-135">relyingPartyName</span></span>|<span data-ttu-id="c14ef-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c14ef-136">String</span></span>|<span data-ttu-id="c14ef-137">Nome do aplicativo ou outra entidade na Internet que usa um provedor de identidade para autenticar um usuário que deseja fazer logoff.</span><span class="sxs-lookup"><span data-stu-id="c14ef-137">Name of application or other entity on the internet that uses an identity provider to authenticate a user who wants to log in.</span></span>|
|<span data-ttu-id="c14ef-138">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="c14ef-138">failedSignInCount</span></span>|<span data-ttu-id="c14ef-139">Int64</span><span class="sxs-lookup"><span data-stu-id="c14ef-139">Int64</span></span>| <span data-ttu-id="c14ef-140">Número de falha ao entrar no Serviço de Federação do Active Directory no período especificado.</span><span class="sxs-lookup"><span data-stu-id="c14ef-140">Number of failed sign in on Active Directory Federation Service in the period specified.</span></span> |
|<span data-ttu-id="c14ef-141">replyUrls</span><span class="sxs-lookup"><span data-stu-id="c14ef-141">replyUrls</span></span>|<span data-ttu-id="c14ef-142">String collection</span><span class="sxs-lookup"><span data-stu-id="c14ef-142">String collection</span></span>|<span data-ttu-id="c14ef-143">Especifica onde a parte de confiança espera receber o token.</span><span class="sxs-lookup"><span data-stu-id="c14ef-143">Specifies where the relying party expects to receive the token.</span></span>|
|<span data-ttu-id="c14ef-144">signInSuccessRate</span><span class="sxs-lookup"><span data-stu-id="c14ef-144">signInSuccessRate</span></span>|<span data-ttu-id="c14ef-145">Duplo</span><span class="sxs-lookup"><span data-stu-id="c14ef-145">Double</span></span>|<span data-ttu-id="c14ef-146">Número de êxito / (número de bem-sucedido + número de falhas de login) no Serviço de Federação do Active Directory no período especificado.</span><span class="sxs-lookup"><span data-stu-id="c14ef-146">Number of successful / (number of successful + number of failed sign ins) on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="c14ef-147">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="c14ef-147">successfulSignInCount</span></span>|<span data-ttu-id="c14ef-148">Int64</span><span class="sxs-lookup"><span data-stu-id="c14ef-148">Int64</span></span>|<span data-ttu-id="c14ef-149">Número de logins bem-sucedidos no Serviço de Federação do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c14ef-149">Number of successful sign ins on Active Directory Federation Service.</span></span>|
|<span data-ttu-id="c14ef-150">totalSignInCount</span><span class="sxs-lookup"><span data-stu-id="c14ef-150">totalSignInCount</span></span>|<span data-ttu-id="c14ef-151">Int64</span><span class="sxs-lookup"><span data-stu-id="c14ef-151">Int64</span></span>|<span data-ttu-id="c14ef-152">Número de logins bem-sucedidos + com falha ao entrar no Serviço de Federação do Active Directory no período especificado.</span><span class="sxs-lookup"><span data-stu-id="c14ef-152">Number of successful + failed sign ins failed sign ins on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="c14ef-153">uniqueUserCount</span><span class="sxs-lookup"><span data-stu-id="c14ef-153">uniqueUserCount</span></span>|<span data-ttu-id="c14ef-154">Int64</span><span class="sxs-lookup"><span data-stu-id="c14ef-154">Int64</span></span>|<span data-ttu-id="c14ef-155">Número de usuários exclusivos que entraram no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c14ef-155">Number of unique users that have signed into the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c14ef-156">Relações</span><span class="sxs-lookup"><span data-stu-id="c14ef-156">Relationships</span></span>

<span data-ttu-id="c14ef-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c14ef-157">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c14ef-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c14ef-158">JSON representation</span></span>

<span data-ttu-id="c14ef-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c14ef-159">The following is a JSON representation of the resource.</span></span>

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


