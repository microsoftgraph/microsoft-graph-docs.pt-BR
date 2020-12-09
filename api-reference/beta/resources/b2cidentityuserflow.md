---
title: tipo de recurso b2cIdentityUserFlow
description: Representa um fluxo de usuário em um locatário do Azure Active Directory B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: 61c3a206ee07eb7e8474e501f9064a20c6cc3840
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581086"
---
# <a name="b2cidentityuserflow-resource-type"></a><span data-ttu-id="11825-103">tipo de recurso b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="11825-103">b2cIdentityUserFlow resource type</span></span>

<span data-ttu-id="11825-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11825-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11825-105">Representa um fluxo de usuário em um locatário do Azure Active Directory B2C.</span><span class="sxs-lookup"><span data-stu-id="11825-105">Represents a user flow within an Azure Active Directory B2C tenant.</span></span>

<span data-ttu-id="11825-106">Para ajudar você a configurar as tarefas de identidade mais comuns para seus aplicativos, o Azure Active Directory B2C inclui políticas configuráveis e predefinidas, chamadas [fluxos de usuário](/azure/active-directory-b2c/user-flow-overview).</span><span class="sxs-lookup"><span data-stu-id="11825-106">To help you set up the most common identity tasks for your applications, Azure Active Directory B2C includes predefined, configurable policies called [user flows](/azure/active-directory-b2c/user-flow-overview).</span></span> <span data-ttu-id="11825-107">Um fluxo de usuário permite que você determine como os usuários interagem com o seu aplicativo quando eles fazem logon, inscrevem-se, editam um perfil ou redefinem uma senha.</span><span class="sxs-lookup"><span data-stu-id="11825-107">A user flow lets you determine how users interact with your application when they do things like sign in, sign up, edit a profile, or reset a password.</span></span> <span data-ttu-id="11825-108">Você pode criar muitos fluxos de usuário de tipos diferentes em seu locatário e usá-lo em seus aplicativos, conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="11825-108">You can create many user flows of different types in your tenant and use them in your applications as needed.</span></span> <span data-ttu-id="11825-109">Com os fluxos de usuário, você pode controle os seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="11825-109">With user flows, you can control the following capabilities:</span></span>

- <span data-ttu-id="11825-110">Tipos de conta usados para fazer logon, como contas sociais, como uma conta local ou do Facebook</span><span class="sxs-lookup"><span data-stu-id="11825-110">Account types used for sign-in, such as social accounts like a Facebook or local account</span></span>
- <span data-ttu-id="11825-111">Atributos a serem coletados do consumidor, como o nome, CEO e número do calçado</span><span class="sxs-lookup"><span data-stu-id="11825-111">Attributes to be collected from the consumer, such as first name, postal code, and shoe size</span></span>
- <span data-ttu-id="11825-112">Autenticação de vários fatores do Azure</span><span class="sxs-lookup"><span data-stu-id="11825-112">Azure Multi-Factor Authentication</span></span>
- <span data-ttu-id="11825-113">Personalização da interface do usuário</span><span class="sxs-lookup"><span data-stu-id="11825-113">Customization of the user interface</span></span>
- <span data-ttu-id="11825-114">Informações recebidas pelo aplicativo no token</span><span class="sxs-lookup"><span data-stu-id="11825-114">Information that the application receives in the token</span></span>

## <a name="methods"></a><span data-ttu-id="11825-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="11825-115">Methods</span></span>

| <span data-ttu-id="11825-116">Método</span><span class="sxs-lookup"><span data-stu-id="11825-116">Method</span></span>       | <span data-ttu-id="11825-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="11825-117">Return Type</span></span>  |<span data-ttu-id="11825-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="11825-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="11825-119">Listar fluxos de usuário</span><span class="sxs-lookup"><span data-stu-id="11825-119">List user flows</span></span>](../api/identitycontainer-list-b2cuserflows.md)|<span data-ttu-id="11825-120">Coleção b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="11825-120">b2cIdentityUserFlow collection</span></span>|<span data-ttu-id="11825-121">Recupere todos os fluxos de usuário B2C.</span><span class="sxs-lookup"><span data-stu-id="11825-121">Retrieve all B2C user flows.</span></span>|
|[<span data-ttu-id="11825-122">Obter fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="11825-122">Get user flow</span></span>](../api/b2cidentityuserflow-get.md)|<span data-ttu-id="11825-123">b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="11825-123">b2cIdentityUserFlow</span></span>|<span data-ttu-id="11825-124">Recupere as propriedades de um fluxo de usuário B2C.</span><span class="sxs-lookup"><span data-stu-id="11825-124">Retrieve properties of a B2C user flow.</span></span>|
|[<span data-ttu-id="11825-125">Criar fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="11825-125">Create user flow</span></span>](../api/identitycontainer-post-b2cuserflows.md)|<span data-ttu-id="11825-126">b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="11825-126">b2cIdentityUserFlow</span></span>|<span data-ttu-id="11825-127">Crie um novo fluxo de usuário B2C.</span><span class="sxs-lookup"><span data-stu-id="11825-127">Create a new B2C user flow.</span></span>|
|[<span data-ttu-id="11825-128">Excluir fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="11825-128">Delete user flow</span></span>](../api/b2cidentityuserflow-delete.md)|<span data-ttu-id="11825-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11825-129">None</span></span>|<span data-ttu-id="11825-130">Exclua um fluxo de usuário B2C.</span><span class="sxs-lookup"><span data-stu-id="11825-130">Delete a B2C user flow.</span></span>|
|[<span data-ttu-id="11825-131">Listar os provedores de identidade</span><span class="sxs-lookup"><span data-stu-id="11825-131">List identity providers</span></span>](../api/b2cidentityuserflow-list-identityproviders.md)|<span data-ttu-id="11825-132">Coleção [identityProvider](../resources/identityProvider.md)</span><span class="sxs-lookup"><span data-stu-id="11825-132">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="11825-133">Recupere todos os provedores de identidade em um fluxo de usuário B2C.</span><span class="sxs-lookup"><span data-stu-id="11825-133">Retrieve all identity providers in a B2C user flow.</span></span>|
|[<span data-ttu-id="11825-134">Adicionar provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="11825-134">Add identity provider</span></span>](../api/b2cidentityuserflow-post-identityproviders.md)|<span data-ttu-id="11825-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11825-135">None</span></span>|<span data-ttu-id="11825-136">Adicione um provedor de identidade a um fluxo de usuário B2C.</span><span class="sxs-lookup"><span data-stu-id="11825-136">Add an identity provider to a B2C user flow.</span></span>|
|[<span data-ttu-id="11825-137">Remover provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="11825-137">Remove identity provider</span></span>](../api/b2cidentityuserflow-delete-identityproviders.md)|<span data-ttu-id="11825-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11825-138">None</span></span>|<span data-ttu-id="11825-139">Remova um provedor de identidade de um fluxo de usuário B2C.</span><span class="sxs-lookup"><span data-stu-id="11825-139">Remove an identity provider from a B2C user flow.</span></span>|
|[<span data-ttu-id="11825-140">Listar as atribuições de atributo de usuário</span><span class="sxs-lookup"><span data-stu-id="11825-140">List user attribute assignments</span></span>](../api/b2cidentityuserflow-list-userattributeassignments.md)|<span data-ttu-id="11825-141">Coleção[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) </span><span class="sxs-lookup"><span data-stu-id="11825-141">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) collection</span></span>|<span data-ttu-id="11825-142">Recupere todas as atribuições de atributos do usuário em um fluxo de usuário B2C.</span><span class="sxs-lookup"><span data-stu-id="11825-142">Retrieve all user attribute assignments in a B2C user flow.</span></span>|
|[<span data-ttu-id="11825-143">Criar uma tarefa de atributo de usuário</span><span class="sxs-lookup"><span data-stu-id="11825-143">Create user attribute assignment</span></span>](../api/b2cidentityuserflow-post-userattributeassignments.md)|[<span data-ttu-id="11825-144">identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="11825-144">identityUserFlowAttributeAssignment</span></span>](../resources/identityuserflowattributeassignment.md)|<span data-ttu-id="11825-145">Crie uma atribuição de atributo de usuário em um fluxo de usuário B2C.</span><span class="sxs-lookup"><span data-stu-id="11825-145">Create a user attribute assignment in a B2C user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="11825-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11825-146">Properties</span></span>

|<span data-ttu-id="11825-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11825-147">Property</span></span>|<span data-ttu-id="11825-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="11825-148">Type</span></span>|<span data-ttu-id="11825-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="11825-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11825-150">id</span><span class="sxs-lookup"><span data-stu-id="11825-150">id</span></span>|<span data-ttu-id="11825-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11825-151">String</span></span>|<span data-ttu-id="11825-152">O nome do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="11825-152">The name of the user flow.</span></span> <span data-ttu-id="11825-153">Esse é um valor obrigatório e imutável após sua criação.</span><span class="sxs-lookup"><span data-stu-id="11825-153">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="11825-154">O nome será antecedido pelo valor de `B2C_1_` após a criação.</span><span class="sxs-lookup"><span data-stu-id="11825-154">The name will be prefixed with the value of `B2C_1_` after creation.</span></span>|
|<span data-ttu-id="11825-155">userFlowType</span><span class="sxs-lookup"><span data-stu-id="11825-155">userFlowType</span></span>|<span data-ttu-id="11825-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11825-156">String</span></span>|<span data-ttu-id="11825-157">O [tipo de fluxo de usuário](/azure/active-directory-b2c/user-flow-versions).</span><span class="sxs-lookup"><span data-stu-id="11825-157">The [type of user flow](/azure/active-directory-b2c/user-flow-versions).</span></span> <span data-ttu-id="11825-158">Os valores com suporte para **userFlowType** são:</span><span class="sxs-lookup"><span data-stu-id="11825-158">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwner`</li>|
|<span data-ttu-id="11825-159">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="11825-159">userFlowTypeVersion</span></span>|<span data-ttu-id="11825-160">Único</span><span class="sxs-lookup"><span data-stu-id="11825-160">Single</span></span>|<span data-ttu-id="11825-161">A versão do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="11825-161">The version of the user flow.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11825-162">Relações</span><span class="sxs-lookup"><span data-stu-id="11825-162">Relationships</span></span>

| <span data-ttu-id="11825-163">Relação</span><span class="sxs-lookup"><span data-stu-id="11825-163">Relationship</span></span>       | <span data-ttu-id="11825-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="11825-164">Type</span></span>  |<span data-ttu-id="11825-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="11825-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11825-166">identityProviders</span><span class="sxs-lookup"><span data-stu-id="11825-166">identityProviders</span></span>|<span data-ttu-id="11825-167">Coleção [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="11825-167">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="11825-168">Os provedores de identidade incluídos no fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="11825-168">The identity providers included in the user flow.</span></span>|
|<span data-ttu-id="11825-169">userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="11825-169">userAttributeAssignments</span></span>|<span data-ttu-id="11825-170">Coleção[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) </span><span class="sxs-lookup"><span data-stu-id="11825-170">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) collection</span></span>|<span data-ttu-id="11825-171">As atribuições de atributo de usuário incluídas no fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="11825-171">The user attribute assignments included in the user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11825-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11825-172">JSON representation</span></span>

<span data-ttu-id="11825-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11825-173">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow",
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
