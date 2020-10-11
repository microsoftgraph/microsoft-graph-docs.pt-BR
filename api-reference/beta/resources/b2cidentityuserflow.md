---
title: tipo de recurso b2cIdentityUserFlow
description: Representa um fluxo de usuário em um locatário do Azure Active Directory B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: af29926d77c8888cadc67c4cd7e7558fe47062d6
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406299"
---
# <a name="b2cidentityuserflow-resource-type"></a><span data-ttu-id="574d5-103">tipo de recurso b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="574d5-103">b2cIdentityUserFlow resource type</span></span>

<span data-ttu-id="574d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="574d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="574d5-105">Representa um fluxo de usuário em um locatário do Azure Active Directory B2C.</span><span class="sxs-lookup"><span data-stu-id="574d5-105">Represents a user flow within an Azure Active Directory B2C tenant.</span></span>

<span data-ttu-id="574d5-106">Para ajudar você a configurar as tarefas de identidade mais comuns para seus aplicativos, o Azure Active Directory B2C inclui políticas configuráveis e predefinidas, chamadas [fluxos de usuário](/azure/active-directory-b2c/user-flow-overview).</span><span class="sxs-lookup"><span data-stu-id="574d5-106">To help you set up the most common identity tasks for your applications, Azure Active Directory B2C includes predefined, configurable policies called [user flows](/azure/active-directory-b2c/user-flow-overview).</span></span> <span data-ttu-id="574d5-107">Um fluxo de usuário permite que você determine como os usuários interagem com o seu aplicativo quando eles fazem logon, inscrevem-se, editam um perfil ou redefinem uma senha.</span><span class="sxs-lookup"><span data-stu-id="574d5-107">A user flow lets you determine how users interact with your application when they do things like sign in, sign up, edit a profile, or reset a password.</span></span> <span data-ttu-id="574d5-108">Você pode criar muitos fluxos de usuário de tipos diferentes em seu locatário e usá-lo em seus aplicativos, conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="574d5-108">You can create many user flows of different types in your tenant and use them in your applications as needed.</span></span> <span data-ttu-id="574d5-109">Com os fluxos de usuário, você pode controle os seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="574d5-109">With user flows, you can control the following capabilities:</span></span>

- <span data-ttu-id="574d5-110">Tipos de conta usados para fazer logon, como contas sociais, como uma conta local ou do Facebook</span><span class="sxs-lookup"><span data-stu-id="574d5-110">Account types used for sign-in, such as social accounts like a Facebook or local account</span></span>
- <span data-ttu-id="574d5-111">Atributos a serem coletados do consumidor, como o nome, CEO e número do calçado</span><span class="sxs-lookup"><span data-stu-id="574d5-111">Attributes to be collected from the consumer, such as first name, postal code, and shoe size</span></span>
- <span data-ttu-id="574d5-112">Autenticação de vários fatores do Azure</span><span class="sxs-lookup"><span data-stu-id="574d5-112">Azure Multi-Factor Authentication</span></span>
- <span data-ttu-id="574d5-113">Personalização da interface do usuário</span><span class="sxs-lookup"><span data-stu-id="574d5-113">Customization of the user interface</span></span>
- <span data-ttu-id="574d5-114">Informações recebidas pelo aplicativo no token</span><span class="sxs-lookup"><span data-stu-id="574d5-114">Information that the application receives in the token</span></span>

## <a name="methods"></a><span data-ttu-id="574d5-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="574d5-115">Methods</span></span>

| <span data-ttu-id="574d5-116">Método</span><span class="sxs-lookup"><span data-stu-id="574d5-116">Method</span></span>       | <span data-ttu-id="574d5-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="574d5-117">Return Type</span></span>  |<span data-ttu-id="574d5-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="574d5-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="574d5-119">Listar fluxos de usuário</span><span class="sxs-lookup"><span data-stu-id="574d5-119">List user flows</span></span>](../api/identitycontainer-list-b2cuserflows.md)|<span data-ttu-id="574d5-120">Coleção b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="574d5-120">b2cIdentityUserFlow collection</span></span>|<span data-ttu-id="574d5-121">Recupere todos os fluxos de usuário B2C.</span><span class="sxs-lookup"><span data-stu-id="574d5-121">Retrieve all B2C user flows.</span></span>|
|[<span data-ttu-id="574d5-122">Obter fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="574d5-122">Get user flow</span></span>](../api/b2cidentityuserflow-get.md)|<span data-ttu-id="574d5-123">b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="574d5-123">b2cIdentityUserFlow</span></span>|<span data-ttu-id="574d5-124">Recupere as propriedades de um fluxo de usuário B2C.</span><span class="sxs-lookup"><span data-stu-id="574d5-124">Retrieve properties of a B2C user flow.</span></span>|
|[<span data-ttu-id="574d5-125">Criar fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="574d5-125">Create user flow</span></span>](../api/identitycontainer-post-b2cuserflows.md)|<span data-ttu-id="574d5-126">b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="574d5-126">b2cIdentityUserFlow</span></span>|<span data-ttu-id="574d5-127">Crie um novo fluxo de usuário B2C.</span><span class="sxs-lookup"><span data-stu-id="574d5-127">Create a new B2C user flow.</span></span>|
|[<span data-ttu-id="574d5-128">Excluir fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="574d5-128">Delete user flow</span></span>](../api/b2cidentityuserflow-delete.md)|<span data-ttu-id="574d5-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="574d5-129">None</span></span>|<span data-ttu-id="574d5-130">Exclua um fluxo de usuário B2C.</span><span class="sxs-lookup"><span data-stu-id="574d5-130">Delete a B2C user flow.</span></span>|
|[<span data-ttu-id="574d5-131">Listar os provedores de identidade</span><span class="sxs-lookup"><span data-stu-id="574d5-131">List identity providers</span></span>](../api/b2cidentityuserflow-list-identityproviders.md)|<span data-ttu-id="574d5-132">Coleção [identityProvider](../resources/identityProvider.md)</span><span class="sxs-lookup"><span data-stu-id="574d5-132">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="574d5-133">Recupere todos os provedores de identidade em um fluxo de usuário B2C.</span><span class="sxs-lookup"><span data-stu-id="574d5-133">Retrieve all identity providers in a B2C user flow.</span></span>|
|[<span data-ttu-id="574d5-134">Adicionar provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="574d5-134">Add identity provider</span></span>](../api/b2cidentityuserflow-post-identityproviders.md)|<span data-ttu-id="574d5-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="574d5-135">None</span></span>|<span data-ttu-id="574d5-136">Adicione um provedor de identidade a um fluxo de usuário B2C.</span><span class="sxs-lookup"><span data-stu-id="574d5-136">Add an identity provider to a B2C user flow.</span></span>|
|[<span data-ttu-id="574d5-137">Remover provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="574d5-137">Remove identity provider</span></span>](../api/b2cidentityuserflow-delete-identityproviders.md)|<span data-ttu-id="574d5-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="574d5-138">None</span></span>|<span data-ttu-id="574d5-139">Remova um provedor de identidade de um fluxo de usuário B2C.</span><span class="sxs-lookup"><span data-stu-id="574d5-139">Remove an identity provider from a B2C user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="574d5-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="574d5-140">Properties</span></span>

|<span data-ttu-id="574d5-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="574d5-141">Property</span></span>|<span data-ttu-id="574d5-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="574d5-142">Type</span></span>|<span data-ttu-id="574d5-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="574d5-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="574d5-144">id</span><span class="sxs-lookup"><span data-stu-id="574d5-144">id</span></span>|<span data-ttu-id="574d5-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="574d5-145">String</span></span>|<span data-ttu-id="574d5-146">O nome do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="574d5-146">The name of the user flow.</span></span> <span data-ttu-id="574d5-147">Esse é um valor obrigatório e imutável após sua criação.</span><span class="sxs-lookup"><span data-stu-id="574d5-147">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="574d5-148">O nome será antecedido pelo valor de `B2C_1_` após a criação.</span><span class="sxs-lookup"><span data-stu-id="574d5-148">The name will be prefixed with the value of `B2C_1_` after creation.</span></span>|
|<span data-ttu-id="574d5-149">userFlowType</span><span class="sxs-lookup"><span data-stu-id="574d5-149">userFlowType</span></span>|<span data-ttu-id="574d5-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="574d5-150">String</span></span>|<span data-ttu-id="574d5-151">O [tipo de fluxo de usuário](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-versions).</span><span class="sxs-lookup"><span data-stu-id="574d5-151">The [type of user flow](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-versions).</span></span> <span data-ttu-id="574d5-152">Os valores com suporte para **userFlowType** são:</span><span class="sxs-lookup"><span data-stu-id="574d5-152">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwnerPasswordCredentialSignIn`</li>|
|<span data-ttu-id="574d5-153">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="574d5-153">userFlowTypeVersion</span></span>|<span data-ttu-id="574d5-154">Único</span><span class="sxs-lookup"><span data-stu-id="574d5-154">Single</span></span>|<span data-ttu-id="574d5-155">A versão do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="574d5-155">The version of the user flow.</span></span>|

## <a name="relationships"></a><span data-ttu-id="574d5-156">Relações</span><span class="sxs-lookup"><span data-stu-id="574d5-156">Relationships</span></span>

| <span data-ttu-id="574d5-157">Relação</span><span class="sxs-lookup"><span data-stu-id="574d5-157">Relationship</span></span>       | <span data-ttu-id="574d5-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="574d5-158">Type</span></span>  |<span data-ttu-id="574d5-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="574d5-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="574d5-160">identityProviders</span><span class="sxs-lookup"><span data-stu-id="574d5-160">identityProviders</span></span>|<span data-ttu-id="574d5-161">Coleção [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="574d5-161">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="574d5-162">Os provedores de identidade incluídos no fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="574d5-162">The identity providers included in the user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="574d5-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="574d5-163">JSON representation</span></span>

<span data-ttu-id="574d5-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="574d5-164">The following is a JSON representation of the resource.</span></span>

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
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}]
}
```