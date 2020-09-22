---
title: Tipo de recurso b2xUserFlows
description: Representa um fluxo de usuário em um locatário do Azure Active Directory.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: 989fbb3e003acd4207740a300c1b6f5d0c926e08
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089746"
---
# <a name="b2xuserflows-resource-type"></a><span data-ttu-id="e5cc8-103">Tipo de recurso b2xUserFlows</span><span class="sxs-lookup"><span data-stu-id="e5cc8-103">b2xUserFlows resource type</span></span>

<span data-ttu-id="e5cc8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5cc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5cc8-105">Representa um fluxo de usuário em um locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-105">Represents a user flow within an Azure Active Directory tenant.</span></span>

<span data-ttu-id="e5cc8-106">Os fluxos de usuário são usados para habilitar uma experiência de [inscrição de autoatendimento](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) para usuários convidados em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-106">User flows are used to enable a [self-service sign up](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) experience for guest users on an application.</span></span> <span data-ttu-id="e5cc8-107">Os fluxos de usuário definem a experiência que o usuário final vê ao se inscrever, inclusive quais [provedores de identidade](https://docs.microsoft.com/azure/active-directory/external-identities/identity-providers) ele pode usar para autenticação, juntamente com quais atributos são coletados como parte do processo de inscrição.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-107">User flows define the experience the end user sees while signing up, including which [identity providers](https://docs.microsoft.com/azure/active-directory/external-identities/identity-providers) they can use to authenticate, along with which attributes are collected as part of the sign up process.</span></span>

## <a name="methods"></a><span data-ttu-id="e5cc8-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="e5cc8-108">Methods</span></span>

| <span data-ttu-id="e5cc8-109">Método</span><span class="sxs-lookup"><span data-stu-id="e5cc8-109">Method</span></span>       | <span data-ttu-id="e5cc8-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e5cc8-110">Return Type</span></span>  |<span data-ttu-id="e5cc8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5cc8-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e5cc8-112">Listar fluxos de usuário</span><span class="sxs-lookup"><span data-stu-id="e5cc8-112">List user flows</span></span>](../api/b2xuserflows-list.md)|<span data-ttu-id="e5cc8-113">Coleção b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="e5cc8-113">b2xUserFlow collection</span></span>|<span data-ttu-id="e5cc8-114">Recuperar todos os fluxos de usuário.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-114">Retrieve all user flows.</span></span>|
|[<span data-ttu-id="e5cc8-115">Obter fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="e5cc8-115">Get user flow</span></span>](../api/b2xuserflows-get.md)|<span data-ttu-id="e5cc8-116">b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="e5cc8-116">b2xUserFlow</span></span>|<span data-ttu-id="e5cc8-117">Recuperar as propriedades de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-117">Retrieve properties of a user flow.</span></span>|
|[<span data-ttu-id="e5cc8-118">Criar fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="e5cc8-118">Create user flow</span></span>](../api/b2xuserflow-post-b2xuserflows.md)|<span data-ttu-id="e5cc8-119">b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="e5cc8-119">b2xUserFlow</span></span>|<span data-ttu-id="e5cc8-120">Criar um novo fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-120">Create a new user flow.</span></span>|
|[<span data-ttu-id="e5cc8-121">Excluir fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="e5cc8-121">Delete user flow</span></span>](../api/b2xuserflows-delete.md)|<span data-ttu-id="e5cc8-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5cc8-122">None</span></span>|<span data-ttu-id="e5cc8-123">Excluir um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-123">Delete a user flow.</span></span>|
|[<span data-ttu-id="e5cc8-124">Listar os provedores de identidade</span><span class="sxs-lookup"><span data-stu-id="e5cc8-124">List identity providers</span></span>](../api/b2xuserflows-list-identityproviders.md)|<span data-ttu-id="e5cc8-125">Coleção [identityProvider](../resources/identityProvider.md)</span><span class="sxs-lookup"><span data-stu-id="e5cc8-125">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="e5cc8-126">Recuperar todos os provedores de identidade em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-126">Retrieve all identity providers in a user flow.</span></span>|
|[<span data-ttu-id="e5cc8-127">Adicionar provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="e5cc8-127">Add identity provider</span></span>](../api/b2xuserflows-update-identityprovider.md)|<span data-ttu-id="e5cc8-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5cc8-128">None</span></span>|<span data-ttu-id="e5cc8-129">Adicionar um provedor de identidade a um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-129">Add an identity provider to a user flow.</span></span>|
|[<span data-ttu-id="e5cc8-130">Excluir provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="e5cc8-130">Delete identity provider</span></span>](../api/b2xuserflows-delete-identityprovider.md)|<span data-ttu-id="e5cc8-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5cc8-131">None</span></span>|<span data-ttu-id="e5cc8-132">Excluir um provedor de identidade de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-132">Delete an identity provider from a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5cc8-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5cc8-133">Properties</span></span>

|<span data-ttu-id="e5cc8-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5cc8-134">Property</span></span>|<span data-ttu-id="e5cc8-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5cc8-135">Type</span></span>|<span data-ttu-id="e5cc8-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5cc8-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5cc8-137">id</span><span class="sxs-lookup"><span data-stu-id="e5cc8-137">id</span></span>|<span data-ttu-id="e5cc8-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5cc8-138">String</span></span>|<span data-ttu-id="e5cc8-139">O nome do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-139">The name of the user flow.</span></span> <span data-ttu-id="e5cc8-140">Esse é um valor obrigatório e imutável após sua criação.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-140">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="e5cc8-141">O nome será antecedido pelo valor de `B2X_1_` após a criação.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-141">The name will be prefixed with the value of `B2X_1_` after creation.</span></span>|
|<span data-ttu-id="e5cc8-142">userFlowType</span><span class="sxs-lookup"><span data-stu-id="e5cc8-142">userFlowType</span></span>|<span data-ttu-id="e5cc8-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5cc8-143">String</span></span>|<span data-ttu-id="e5cc8-144">O tipo de fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-144">The type of user flow.</span></span> <span data-ttu-id="e5cc8-145">Para os fluxos de usuário de inscrição de autoatendimento, o valor só poderá ser `signUpOrSignIn` e não poderá ser modificado após a criação.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-145">For self-service sign up user flows, the value can only be `signUpOrSignIn` and cannot be modified after creation.</span></span>|
|<span data-ttu-id="e5cc8-146">userFlowVersion</span><span class="sxs-lookup"><span data-stu-id="e5cc8-146">userFlowVersion</span></span>|<span data-ttu-id="e5cc8-147">Único</span><span class="sxs-lookup"><span data-stu-id="e5cc8-147">Single</span></span>|<span data-ttu-id="e5cc8-148">A versão do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-148">The version of the user flow.</span></span> <span data-ttu-id="e5cc8-149">Para fluxos de usuário B2X, a versão é sempre `1`.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-149">For B2X user flows, the version is always `1`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5cc8-150">Relações</span><span class="sxs-lookup"><span data-stu-id="e5cc8-150">Relationships</span></span>

| <span data-ttu-id="e5cc8-151">Relação</span><span class="sxs-lookup"><span data-stu-id="e5cc8-151">Relationship</span></span>       | <span data-ttu-id="e5cc8-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5cc8-152">Type</span></span>  |<span data-ttu-id="e5cc8-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5cc8-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5cc8-154">identityProviders</span><span class="sxs-lookup"><span data-stu-id="e5cc8-154">identityProviders</span></span>|<span data-ttu-id="e5cc8-155">Coleção [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="e5cc8-155">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="e5cc8-156">Os provedores de identidade incluídos no fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-156">The identity providers included in the user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5cc8-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5cc8-157">JSON representation</span></span>

<span data-ttu-id="e5cc8-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5cc8-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow",
  "optionalProperties": [],
  "keyProperty": "id"
} -->

```json
{
    "id": "String (identifier)",
    "userFlowType": "String",
    "userFlowTypeVersion": "Single",
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}]
}
```


