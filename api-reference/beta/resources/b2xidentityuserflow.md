---
title: tipo de recurso b2xIdentityUserFlow
description: Representa um fluxo de usuário em um locatário do Azure Active Directory.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: 85839539ae78963114ea7a9eaeac49307166a9ff
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406298"
---
# <a name="b2xidentityuserflow-resource-type"></a><span data-ttu-id="74486-103">tipo de recurso b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="74486-103">b2xIdentityUserFlow resource type</span></span>

<span data-ttu-id="74486-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74486-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74486-105">Representa um fluxo de usuário em um locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="74486-105">Represents a user flow within an Azure Active Directory tenant.</span></span>

<span data-ttu-id="74486-106">Os fluxos de usuário são usados para habilitar uma experiência de [inscrição de autoatendimento](/azure/active-directory/external-identities/self-service-sign-up-overview) para usuários convidados em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="74486-106">User flows are used to enable a [self-service sign up](/azure/active-directory/external-identities/self-service-sign-up-overview) experience for guest users on an application.</span></span> <span data-ttu-id="74486-107">Os fluxos de usuário definem a experiência que o usuário final vê ao se inscrever, inclusive quais [provedores de identidade](/azure/active-directory/external-identities/identity-providers) ele pode usar para autenticação, juntamente com quais atributos são coletados como parte do processo de inscrição.</span><span class="sxs-lookup"><span data-stu-id="74486-107">User flows define the experience the end user sees while signing up, including which [identity providers](/azure/active-directory/external-identities/identity-providers) they can use to authenticate, along with which attributes are collected as part of the sign up process.</span></span>

## <a name="methods"></a><span data-ttu-id="74486-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="74486-108">Methods</span></span>

| <span data-ttu-id="74486-109">Método</span><span class="sxs-lookup"><span data-stu-id="74486-109">Method</span></span>       | <span data-ttu-id="74486-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="74486-110">Return Type</span></span>  |<span data-ttu-id="74486-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="74486-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74486-112">Listar fluxos de usuário</span><span class="sxs-lookup"><span data-stu-id="74486-112">List user flows</span></span>](../api/identitycontainer-list-b2xuserflows.md)|<span data-ttu-id="74486-113">Coleção b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="74486-113">b2xIdentityUserFlow collection</span></span>|<span data-ttu-id="74486-114">Recupere todos os fluxos de usuário B2X.</span><span class="sxs-lookup"><span data-stu-id="74486-114">Retrieve all B2X user flows.</span></span>|
|[<span data-ttu-id="74486-115">Obter fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="74486-115">Get user flow</span></span>](../api/b2xidentityuserflow-get.md)|<span data-ttu-id="74486-116">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="74486-116">b2xIdentityUserFlow</span></span>|<span data-ttu-id="74486-117">Recupere as propriedades de um fluxo de usuário B2X.</span><span class="sxs-lookup"><span data-stu-id="74486-117">Retrieve properties of a B2X user flow.</span></span>|
|[<span data-ttu-id="74486-118">Criar fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="74486-118">Create user flow</span></span>](../api/identitycontainer-post-b2xuserflows.md)|<span data-ttu-id="74486-119">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="74486-119">b2xIdentityUserFlow</span></span>|<span data-ttu-id="74486-120">Crie um novo fluxo de usuário B2X.</span><span class="sxs-lookup"><span data-stu-id="74486-120">Create a new B2X user flow.</span></span>|
|[<span data-ttu-id="74486-121">Excluir fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="74486-121">Delete user flow</span></span>](../api/b2xidentityuserflow-delete.md)|<span data-ttu-id="74486-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74486-122">None</span></span>|<span data-ttu-id="74486-123">Exclua um fluxo de usuário B2X.</span><span class="sxs-lookup"><span data-stu-id="74486-123">Delete a B2X user flow.</span></span>|
|[<span data-ttu-id="74486-124">Listar os provedores de identidade</span><span class="sxs-lookup"><span data-stu-id="74486-124">List identity providers</span></span>](../api/b2xidentityuserflow-list-identityproviders.md)|<span data-ttu-id="74486-125">Coleção [identityProvider](../resources/identityProvider.md)</span><span class="sxs-lookup"><span data-stu-id="74486-125">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="74486-126">Recupere todos os provedores de identidade em um fluxo de usuário B2X.</span><span class="sxs-lookup"><span data-stu-id="74486-126">Retrieve all identity providers in a B2X user flow.</span></span>|
|[<span data-ttu-id="74486-127">Adicionar provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="74486-127">Add identity provider</span></span>](../api/b2xidentityuserflow-post-identityproviders.md)|<span data-ttu-id="74486-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74486-128">None</span></span>|<span data-ttu-id="74486-129">Adicione um provedor de identidade a um fluxo de usuário B2X.</span><span class="sxs-lookup"><span data-stu-id="74486-129">Add an identity provider to a B2X user flow.</span></span>|
|[<span data-ttu-id="74486-130">Remover provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="74486-130">Remove identity provider</span></span>](../api/b2xidentityuserflow-delete-identityproviders.md)|<span data-ttu-id="74486-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74486-131">None</span></span>|<span data-ttu-id="74486-132">Remova um provedor de identidade de um fluxo de usuário B2X.</span><span class="sxs-lookup"><span data-stu-id="74486-132">Remove an identity provider from a B2X user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="74486-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74486-133">Properties</span></span>

|<span data-ttu-id="74486-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74486-134">Property</span></span>|<span data-ttu-id="74486-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="74486-135">Type</span></span>|<span data-ttu-id="74486-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="74486-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74486-137">id</span><span class="sxs-lookup"><span data-stu-id="74486-137">id</span></span>|<span data-ttu-id="74486-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74486-138">String</span></span>|<span data-ttu-id="74486-139">O nome do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="74486-139">The name of the user flow.</span></span> <span data-ttu-id="74486-140">Esse é um valor obrigatório e imutável após sua criação.</span><span class="sxs-lookup"><span data-stu-id="74486-140">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="74486-141">O nome será antecedido pelo valor de `B2X_1_` após a criação.</span><span class="sxs-lookup"><span data-stu-id="74486-141">The name will be prefixed with the value of `B2X_1_` after creation.</span></span>|
|<span data-ttu-id="74486-142">userFlowType</span><span class="sxs-lookup"><span data-stu-id="74486-142">userFlowType</span></span>|<span data-ttu-id="74486-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74486-143">String</span></span>|<span data-ttu-id="74486-144">O tipo de fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="74486-144">The type of user flow.</span></span> <span data-ttu-id="74486-145">Para os fluxos de usuário de inscrição de autoatendimento, o valor só poderá ser `signUpOrSignIn` e não poderá ser modificado após a criação.</span><span class="sxs-lookup"><span data-stu-id="74486-145">For self-service sign up user flows, the value can only be `signUpOrSignIn` and cannot be modified after creation.</span></span>|
|<span data-ttu-id="74486-146">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="74486-146">userFlowTypeVersion</span></span>|<span data-ttu-id="74486-147">Único</span><span class="sxs-lookup"><span data-stu-id="74486-147">Single</span></span>|<span data-ttu-id="74486-148">A versão do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="74486-148">The version of the user flow.</span></span> <span data-ttu-id="74486-149">Para fluxos de usuário B2X, a versão é sempre `1`.</span><span class="sxs-lookup"><span data-stu-id="74486-149">For B2X user flows, the version is always `1`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74486-150">Relações</span><span class="sxs-lookup"><span data-stu-id="74486-150">Relationships</span></span>

| <span data-ttu-id="74486-151">Relação</span><span class="sxs-lookup"><span data-stu-id="74486-151">Relationship</span></span>       | <span data-ttu-id="74486-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="74486-152">Type</span></span>  |<span data-ttu-id="74486-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="74486-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74486-154">identityProviders</span><span class="sxs-lookup"><span data-stu-id="74486-154">identityProviders</span></span>|<span data-ttu-id="74486-155">Coleção [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="74486-155">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="74486-156">Os provedores de identidade incluídos no fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="74486-156">The identity providers included in the user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74486-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74486-157">JSON representation</span></span>

<span data-ttu-id="74486-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74486-158">The following is a JSON representation of the resource.</span></span>

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