---
title: tipo de recurso b2xIdentityUserFlow
description: Representa um fluxo de usuário em um locatário do Azure Active Directory.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: e1051d60681e42012fd9df3fd8655a9e4cc745cd
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49580960"
---
# <a name="b2xidentityuserflow-resource-type"></a><span data-ttu-id="3bac9-103">tipo de recurso b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="3bac9-103">b2xIdentityUserFlow resource type</span></span>

<span data-ttu-id="3bac9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bac9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bac9-105">Representa um fluxo de usuário em um locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3bac9-105">Represents a user flow within an Azure Active Directory tenant.</span></span>

<span data-ttu-id="3bac9-106">Os fluxos de usuário são usados para habilitar uma experiência de [inscrição de autoatendimento](/azure/active-directory/external-identities/self-service-sign-up-overview) para usuários convidados em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3bac9-106">User flows are used to enable a [self-service sign up](/azure/active-directory/external-identities/self-service-sign-up-overview) experience for guest users on an application.</span></span> <span data-ttu-id="3bac9-107">Os fluxos de usuário definem a experiência que o usuário final vê ao se inscrever, inclusive quais [provedores de identidade](/azure/active-directory/external-identities/identity-providers) ele pode usar para autenticação, juntamente com quais atributos são coletados como parte do processo de inscrição.</span><span class="sxs-lookup"><span data-stu-id="3bac9-107">User flows define the experience the end user sees while signing up, including which [identity providers](/azure/active-directory/external-identities/identity-providers) they can use to authenticate, along with which attributes are collected as part of the sign up process.</span></span>

## <a name="methods"></a><span data-ttu-id="3bac9-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="3bac9-108">Methods</span></span>

| <span data-ttu-id="3bac9-109">Método</span><span class="sxs-lookup"><span data-stu-id="3bac9-109">Method</span></span>       | <span data-ttu-id="3bac9-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3bac9-110">Return Type</span></span>  |<span data-ttu-id="3bac9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bac9-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3bac9-112">Listar fluxos de usuário</span><span class="sxs-lookup"><span data-stu-id="3bac9-112">List user flows</span></span>](../api/identitycontainer-list-b2xuserflows.md)|<span data-ttu-id="3bac9-113">Coleção b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="3bac9-113">b2xIdentityUserFlow collection</span></span>|<span data-ttu-id="3bac9-114">Recupere todos os fluxos de usuário B2X.</span><span class="sxs-lookup"><span data-stu-id="3bac9-114">Retrieve all B2X user flows.</span></span>|
|[<span data-ttu-id="3bac9-115">Obter fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="3bac9-115">Get user flow</span></span>](../api/b2xidentityuserflow-get.md)|<span data-ttu-id="3bac9-116">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="3bac9-116">b2xIdentityUserFlow</span></span>|<span data-ttu-id="3bac9-117">Recupere as propriedades de um fluxo de usuário B2X.</span><span class="sxs-lookup"><span data-stu-id="3bac9-117">Retrieve properties of a B2X user flow.</span></span>|
|[<span data-ttu-id="3bac9-118">Criar fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="3bac9-118">Create user flow</span></span>](../api/identitycontainer-post-b2xuserflows.md)|<span data-ttu-id="3bac9-119">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="3bac9-119">b2xIdentityUserFlow</span></span>|<span data-ttu-id="3bac9-120">Crie um novo fluxo de usuário B2X.</span><span class="sxs-lookup"><span data-stu-id="3bac9-120">Create a new B2X user flow.</span></span>|
|[<span data-ttu-id="3bac9-121">Excluir fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="3bac9-121">Delete user flow</span></span>](../api/b2xidentityuserflow-delete.md)|<span data-ttu-id="3bac9-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3bac9-122">None</span></span>|<span data-ttu-id="3bac9-123">Exclua um fluxo de usuário B2X.</span><span class="sxs-lookup"><span data-stu-id="3bac9-123">Delete a B2X user flow.</span></span>|
|[<span data-ttu-id="3bac9-124">Listar os provedores de identidade</span><span class="sxs-lookup"><span data-stu-id="3bac9-124">List identity providers</span></span>](../api/b2xidentityuserflow-list-identityproviders.md)|<span data-ttu-id="3bac9-125">Coleção [identityProvider](../resources/identityProvider.md)</span><span class="sxs-lookup"><span data-stu-id="3bac9-125">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="3bac9-126">Recupere todos os provedores de identidade em um fluxo de usuário B2X.</span><span class="sxs-lookup"><span data-stu-id="3bac9-126">Retrieve all identity providers in a B2X user flow.</span></span>|
|[<span data-ttu-id="3bac9-127">Adicionar provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="3bac9-127">Add identity provider</span></span>](../api/b2xidentityuserflow-post-identityproviders.md)|<span data-ttu-id="3bac9-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3bac9-128">None</span></span>|<span data-ttu-id="3bac9-129">Adicione um provedor de identidade a um fluxo de usuário B2X.</span><span class="sxs-lookup"><span data-stu-id="3bac9-129">Add an identity provider to a B2X user flow.</span></span>|
|[<span data-ttu-id="3bac9-130">Remover provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="3bac9-130">Remove identity provider</span></span>](../api/b2xidentityuserflow-delete-identityproviders.md)|<span data-ttu-id="3bac9-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3bac9-131">None</span></span>|<span data-ttu-id="3bac9-132">Remova um provedor de identidade de um fluxo de usuário B2X.</span><span class="sxs-lookup"><span data-stu-id="3bac9-132">Remove an identity provider from a B2X user flow.</span></span>|
|[<span data-ttu-id="3bac9-133">Listar as atribuições de atributo de usuário</span><span class="sxs-lookup"><span data-stu-id="3bac9-133">List user attribute assignments</span></span>](../api/b2xidentityuserflow-list-userattributeassignments.md)|<span data-ttu-id="3bac9-134">Coleção[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) </span><span class="sxs-lookup"><span data-stu-id="3bac9-134">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) collection</span></span>|<span data-ttu-id="3bac9-135">Recupere todas as atribuições de atributos do usuário em um fluxo de usuário B2X.</span><span class="sxs-lookup"><span data-stu-id="3bac9-135">Retrieve all user attribute assignments in a B2X user flow.</span></span>|
|[<span data-ttu-id="3bac9-136">Criar uma tarefa de atributo de usuário</span><span class="sxs-lookup"><span data-stu-id="3bac9-136">Create user attribute assignment</span></span>](../api/b2xidentityuserflow-post-userattributeassignments.md)|[<span data-ttu-id="3bac9-137">identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="3bac9-137">identityUserFlowAttributeAssignment</span></span>](../resources/identityuserflowattributeassignment.md)|<span data-ttu-id="3bac9-138">Crie uma atribuição de atributo de usuário em um fluxo de usuário B2X.</span><span class="sxs-lookup"><span data-stu-id="3bac9-138">Create a user attribute assignment in a B2X user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="3bac9-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3bac9-139">Properties</span></span>

|<span data-ttu-id="3bac9-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3bac9-140">Property</span></span>|<span data-ttu-id="3bac9-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bac9-141">Type</span></span>|<span data-ttu-id="3bac9-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bac9-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3bac9-143">id</span><span class="sxs-lookup"><span data-stu-id="3bac9-143">id</span></span>|<span data-ttu-id="3bac9-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bac9-144">String</span></span>|<span data-ttu-id="3bac9-145">O nome do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="3bac9-145">The name of the user flow.</span></span> <span data-ttu-id="3bac9-146">Esse é um valor obrigatório e imutável após sua criação.</span><span class="sxs-lookup"><span data-stu-id="3bac9-146">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="3bac9-147">O nome será antecedido pelo valor de `B2X_1_` após a criação.</span><span class="sxs-lookup"><span data-stu-id="3bac9-147">The name will be prefixed with the value of `B2X_1_` after creation.</span></span>|
|<span data-ttu-id="3bac9-148">userFlowType</span><span class="sxs-lookup"><span data-stu-id="3bac9-148">userFlowType</span></span>|<span data-ttu-id="3bac9-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bac9-149">String</span></span>|<span data-ttu-id="3bac9-150">O tipo de fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="3bac9-150">The type of user flow.</span></span> <span data-ttu-id="3bac9-151">Para os fluxos de usuário de inscrição de autoatendimento, o valor só poderá ser `signUpOrSignIn` e não poderá ser modificado após a criação.</span><span class="sxs-lookup"><span data-stu-id="3bac9-151">For self-service sign up user flows, the value can only be `signUpOrSignIn` and cannot be modified after creation.</span></span>|
|<span data-ttu-id="3bac9-152">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="3bac9-152">userFlowTypeVersion</span></span>|<span data-ttu-id="3bac9-153">Único</span><span class="sxs-lookup"><span data-stu-id="3bac9-153">Single</span></span>|<span data-ttu-id="3bac9-154">A versão do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="3bac9-154">The version of the user flow.</span></span> <span data-ttu-id="3bac9-155">Para fluxos de usuário B2X, a versão é sempre `1`.</span><span class="sxs-lookup"><span data-stu-id="3bac9-155">For B2X user flows, the version is always `1`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3bac9-156">Relações</span><span class="sxs-lookup"><span data-stu-id="3bac9-156">Relationships</span></span>

| <span data-ttu-id="3bac9-157">Relação</span><span class="sxs-lookup"><span data-stu-id="3bac9-157">Relationship</span></span>       | <span data-ttu-id="3bac9-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bac9-158">Type</span></span>  |<span data-ttu-id="3bac9-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bac9-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3bac9-160">identityProviders</span><span class="sxs-lookup"><span data-stu-id="3bac9-160">identityProviders</span></span>|<span data-ttu-id="3bac9-161">Coleção [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="3bac9-161">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="3bac9-162">Os provedores de identidade incluídos no fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="3bac9-162">The identity providers included in the user flow.</span></span>|
|<span data-ttu-id="3bac9-163">userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="3bac9-163">userAttributeAssignments</span></span>|<span data-ttu-id="3bac9-164">Coleção[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) </span><span class="sxs-lookup"><span data-stu-id="3bac9-164">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) collection</span></span>|<span data-ttu-id="3bac9-165">As atribuições de atributo de usuário incluídas no fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="3bac9-165">The user attribute assignments included in the user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3bac9-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3bac9-166">JSON representation</span></span>

<span data-ttu-id="3bac9-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3bac9-167">The following is a JSON representation of the resource.</span></span>

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
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}],
    "userAttributeAssignments": [{"@odate.type": "microsoft.graph.identityUserFlowAttributeAssignment"}]
}
```
