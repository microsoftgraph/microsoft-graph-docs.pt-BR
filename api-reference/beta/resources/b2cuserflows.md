---
title: tipo de recurso b2cUserFlows
description: Representa um fluxo de usuário em um locatário do Azure Active Directory B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: e540f5b6ff21efd4ba904ddaf4dcb4868df75eff
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319658"
---
# <a name="b2cuserflows-resource-type"></a><span data-ttu-id="4b1bc-103">tipo de recurso b2cUserFlows</span><span class="sxs-lookup"><span data-stu-id="4b1bc-103">b2cUserFlows resource type</span></span>

<span data-ttu-id="4b1bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b1bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b1bc-105">Representa um fluxo de usuário em um locatário do Azure Active Directory B2C.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-105">Represents a user flow within an Azure Active Directory B2C tenant.</span></span>

<span data-ttu-id="4b1bc-106">Para ajudar você a configurar as tarefas de identidade mais comuns para seus aplicativos, o Azure Active Directory B2C inclui políticas configuráveis e predefinidas, chamadas [fluxos de usuário](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-overview).</span><span class="sxs-lookup"><span data-stu-id="4b1bc-106">To help you set up the most common identity tasks for your applications, Azure Active Directory B2C includes predefined, configurable policies called [user flows](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-overview).</span></span> <span data-ttu-id="4b1bc-107">Um fluxo de usuário permite que você determine como os usuário interagem com o seu aplicativo quando eles fazem logon, inscrevem-se, editam um perfil ou redefinem uma senha.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-107">A user flow lets you determine how users interact with your application when they do things like sign in, sign up, edit a profile, or reset a password.</span></span> <span data-ttu-id="4b1bc-108">Você pode criar muitos fluxos de usuário de tipos diferentes em seu locatário e usá-lo em seus aplicativos, conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-108">You can create many user flows of different types in your tenant and use them in your applications as needed.</span></span> <span data-ttu-id="4b1bc-109">Com os fluxos de usuário, você pode controle os seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="4b1bc-109">With user flows, you can control the following capabilities:</span></span>

- <span data-ttu-id="4b1bc-110">Tipos de conta usados para fazer logon, como contas sociais, como uma conta local ou do Facebook</span><span class="sxs-lookup"><span data-stu-id="4b1bc-110">Account types used for sign-in, such as social accounts like a Facebook or local account</span></span>
- <span data-ttu-id="4b1bc-111">Atributos a serem coletados do consumidor, como o nome, CEO e número do calçado</span><span class="sxs-lookup"><span data-stu-id="4b1bc-111">Attributes to be collected from the consumer, such as first name, postal code, and shoe size</span></span>
- <span data-ttu-id="4b1bc-112">Autenticação de vários fatores do Azure</span><span class="sxs-lookup"><span data-stu-id="4b1bc-112">Azure Multi-Factor Authentication</span></span>
- <span data-ttu-id="4b1bc-113">Personalização da interface do usuário</span><span class="sxs-lookup"><span data-stu-id="4b1bc-113">Customization of the user interface</span></span>
- <span data-ttu-id="4b1bc-114">Informações recebidas pelo aplicativo no token</span><span class="sxs-lookup"><span data-stu-id="4b1bc-114">Information that the application receives in the token</span></span>

## <a name="methods"></a><span data-ttu-id="4b1bc-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="4b1bc-115">Methods</span></span>

| <span data-ttu-id="4b1bc-116">Método</span><span class="sxs-lookup"><span data-stu-id="4b1bc-116">Method</span></span>       | <span data-ttu-id="4b1bc-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4b1bc-117">Return Type</span></span>  |<span data-ttu-id="4b1bc-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b1bc-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4b1bc-119">Listar fluxos de usuário</span><span class="sxs-lookup"><span data-stu-id="4b1bc-119">List user flows</span></span>](../api/b2cuserflows-list.md)|<span data-ttu-id="4b1bc-120">coleção b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="4b1bc-120">b2cUserFlow collection</span></span>|<span data-ttu-id="4b1bc-121">Recuperar todos os fluxos de usuário.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-121">Retrieve all user flows.</span></span>|
|[<span data-ttu-id="4b1bc-122">Obter fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="4b1bc-122">Get user flow</span></span>](../api/b2cuserflows-get.md)|<span data-ttu-id="4b1bc-123">b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="4b1bc-123">b2cUserFlow</span></span>|<span data-ttu-id="4b1bc-124">Recuperar as propriedades de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-124">Retrieve properties of a user flow.</span></span>|
|[<span data-ttu-id="4b1bc-125">Criar fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="4b1bc-125">Create user flow</span></span>](../api/b2cuserflow-post-b2cuserflows.md)|<span data-ttu-id="4b1bc-126">b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="4b1bc-126">b2cUserFlow</span></span>|<span data-ttu-id="4b1bc-127">Criar um novo fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-127">Create a new user flow.</span></span>|
|[<span data-ttu-id="4b1bc-128">Excluir fluxo de usuário</span><span class="sxs-lookup"><span data-stu-id="4b1bc-128">Delete user flow</span></span>](../api/b2cuserflows-delete.md)|<span data-ttu-id="4b1bc-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b1bc-129">None</span></span>|<span data-ttu-id="4b1bc-130">Excluir um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-130">Delete a user flow.</span></span>|
|[<span data-ttu-id="4b1bc-131">Listar os provedores de identidade</span><span class="sxs-lookup"><span data-stu-id="4b1bc-131">List identity providers</span></span>](../api/b2cuserflows-list-identityproviders.md)|<span data-ttu-id="4b1bc-132">coleção [identityProvider](../resources/identityProvider.md)</span><span class="sxs-lookup"><span data-stu-id="4b1bc-132">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="4b1bc-133">Recuperar todos os provedores de identidade em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-133">Retrieve all identity providers in a user flow.</span></span>|
|[<span data-ttu-id="4b1bc-134">Adicionar provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="4b1bc-134">Add identity provider</span></span>](../api/b2cuserflows-update-identityprovider.md)|<span data-ttu-id="4b1bc-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b1bc-135">None</span></span>|<span data-ttu-id="4b1bc-136">Adicionar um provedor de identidade a um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-136">Add an identity provider to a user flow.</span></span>|
|[<span data-ttu-id="4b1bc-137">Excluir provedor de identidade</span><span class="sxs-lookup"><span data-stu-id="4b1bc-137">Delete identity provider</span></span>](../api/b2cuserflows-delete-identityprovider.md)|<span data-ttu-id="4b1bc-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b1bc-138">None</span></span>|<span data-ttu-id="4b1bc-139">Excluir um provedor de identidade de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-139">Delete an identity provider from a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="4b1bc-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b1bc-140">Properties</span></span>

|<span data-ttu-id="4b1bc-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b1bc-141">Property</span></span>|<span data-ttu-id="4b1bc-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b1bc-142">Type</span></span>|<span data-ttu-id="4b1bc-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b1bc-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b1bc-144">id</span><span class="sxs-lookup"><span data-stu-id="4b1bc-144">id</span></span>|<span data-ttu-id="4b1bc-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b1bc-145">String</span></span>|<span data-ttu-id="4b1bc-146">O nome do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-146">The name of the user flow.</span></span> <span data-ttu-id="4b1bc-147">Esse é um valor obrigatório e imutável após sua criação.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-147">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="4b1bc-148">O nome será antecedido pelo valor de `B2C_1_` após a criação.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-148">The name will be prefixed with the value of `B2C_1_` after creation.</span></span>|
|<span data-ttu-id="4b1bc-149">userFlowType</span><span class="sxs-lookup"><span data-stu-id="4b1bc-149">userFlowType</span></span>|<span data-ttu-id="4b1bc-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b1bc-150">String</span></span>|<span data-ttu-id="4b1bc-151">O [tipo de fluxo de usuário](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-versions).</span><span class="sxs-lookup"><span data-stu-id="4b1bc-151">The [type of user flow](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-versions).</span></span> <span data-ttu-id="4b1bc-152">Os valores com suporte para **userFlowType** são:</span><span class="sxs-lookup"><span data-stu-id="4b1bc-152">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwnerPasswordCredentialSignIn`</li>|
|<span data-ttu-id="4b1bc-153">userFlowVersion</span><span class="sxs-lookup"><span data-stu-id="4b1bc-153">userFlowVersion</span></span>|<span data-ttu-id="4b1bc-154">Único</span><span class="sxs-lookup"><span data-stu-id="4b1bc-154">Single</span></span>|<span data-ttu-id="4b1bc-155">A versão do fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-155">The version of the user flow.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b1bc-156">Relações</span><span class="sxs-lookup"><span data-stu-id="4b1bc-156">Relationships</span></span>

| <span data-ttu-id="4b1bc-157">Relação</span><span class="sxs-lookup"><span data-stu-id="4b1bc-157">Relationship</span></span>       | <span data-ttu-id="4b1bc-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b1bc-158">Type</span></span>  |<span data-ttu-id="4b1bc-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b1bc-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b1bc-160">identityProviders</span><span class="sxs-lookup"><span data-stu-id="4b1bc-160">identityProviders</span></span>|<span data-ttu-id="4b1bc-161">coleção [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="4b1bc-161">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="4b1bc-162">Os provedores de identidade incluídos no fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-162">The identity providers included in the user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b1bc-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b1bc-163">JSON representation</span></span>

<span data-ttu-id="4b1bc-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-164">The following is a JSON representation of the resource.</span></span>

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
