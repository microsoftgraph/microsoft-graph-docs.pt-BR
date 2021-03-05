---
title: Tipo de recurso homeRealmDiscoveryPolicy
description: Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 78fee8908291619a819b1d62108d149c39b0ae68
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444410"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a><span data-ttu-id="1c2ac-103">Tipo de recurso homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="1c2ac-103">homeRealmDiscoveryPolicy resource type</span></span>

<span data-ttu-id="1c2ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c2ac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1c2ac-105">Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados, em particular para restrições de aceleração automática e autenticação do usuário em domínios federados.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-105">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span> <span data-ttu-id="1c2ac-106">Você pode definir **homeRealmDiscoveryPolicy** para todas as entidades de serviço em sua organização ou para entidades de serviço específicas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-106">You can set **homeRealmDiscoveryPolicy** for all service principals in your organization, or for specific service principals in your organization.</span></span> <span data-ttu-id="1c2ac-107">Para obter mais detalhes de cenário e política, consulte [Configure Azure AD sign in](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) behavior for an application by using a Home Realm Discovery policy, well as [Sign-in to Azure Active Directory](/azure/active-directory/authentication/howto-authentication-use-email-signin)using email as an alternate login ID .</span><span class="sxs-lookup"><span data-stu-id="1c2ac-107">For more scenario and policy details, see [Configure Azure AD sign in behavior for an application by using a Home Realm Discovery policy](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) as well as [Sign-in to Azure Active Directory using email as an alternate login ID](/azure/active-directory/authentication/howto-authentication-use-email-signin).</span></span>

<span data-ttu-id="1c2ac-108">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1c2ac-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1c2ac-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="1c2ac-109">Methods</span></span>

| <span data-ttu-id="1c2ac-110">Método</span><span class="sxs-lookup"><span data-stu-id="1c2ac-110">Method</span></span>       | <span data-ttu-id="1c2ac-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1c2ac-111">Return Type</span></span> | <span data-ttu-id="1c2ac-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c2ac-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1c2ac-113">Listar homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="1c2ac-113">List homeRealmDiscoveryPolicies</span></span>](../api/homerealmdiscoverypolicy-list.md) | [<span data-ttu-id="1c2ac-114">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="1c2ac-114">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="1c2ac-115">Ler propriedades e relações de objetos homeRealmDiscoveryPolicies.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-115">Read properties and relationships of homeRealmDiscoveryPolicies objects.</span></span> |
| [<span data-ttu-id="1c2ac-116">Criar homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="1c2ac-116">Create homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [<span data-ttu-id="1c2ac-117">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="1c2ac-117">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="1c2ac-118">Crie um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-118">Create a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="1c2ac-119">Obter homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="1c2ac-119">Get homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-get.md) | [<span data-ttu-id="1c2ac-120">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="1c2ac-120">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="1c2ac-121">Leia propriedades e relações de um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-121">Read properties and relationships of a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="1c2ac-122">Atualizar homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="1c2ac-122">Update homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-update.md) | <span data-ttu-id="1c2ac-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1c2ac-123">None</span></span> | <span data-ttu-id="1c2ac-124">Atualize um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-124">Update a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="1c2ac-125">Excluir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="1c2ac-125">Delete homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-delete.md) | <span data-ttu-id="1c2ac-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1c2ac-126">None</span></span> | <span data-ttu-id="1c2ac-127">Exclua um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-127">Delete a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="1c2ac-128">Lista appliesTo</span><span class="sxs-lookup"><span data-stu-id="1c2ac-128">List appliesTo</span></span>](../api/homerealmdiscoverypolicy-list-appliesto.md) | <span data-ttu-id="1c2ac-129">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="1c2ac-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="1c2ac-130">Obter a lista de directoryObjects aos qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="1c2ac-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1c2ac-131">Properties</span></span>

| <span data-ttu-id="1c2ac-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c2ac-132">Property</span></span>     | <span data-ttu-id="1c2ac-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c2ac-133">Type</span></span>        | <span data-ttu-id="1c2ac-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c2ac-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1c2ac-135">id</span><span class="sxs-lookup"><span data-stu-id="1c2ac-135">id</span></span>|<span data-ttu-id="1c2ac-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c2ac-136">String</span></span>| <span data-ttu-id="1c2ac-137">Identificador exclusivo dessa política.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-137">Unique identifier for this policy.</span></span> <span data-ttu-id="1c2ac-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-138">Read-only.</span></span>|
|<span data-ttu-id="1c2ac-139">definition</span><span class="sxs-lookup"><span data-stu-id="1c2ac-139">definition</span></span>|<span data-ttu-id="1c2ac-140">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c2ac-140">String collection</span></span>| <span data-ttu-id="1c2ac-141">Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-141">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="1c2ac-142">Consulte abaixo para obter mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-142">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="1c2ac-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-143">Required.</span></span>|
|<span data-ttu-id="1c2ac-144">description</span><span class="sxs-lookup"><span data-stu-id="1c2ac-144">description</span></span>|<span data-ttu-id="1c2ac-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c2ac-145">String</span></span>| <span data-ttu-id="1c2ac-146">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-146">Description for this policy.</span></span>|
|<span data-ttu-id="1c2ac-147">displayName</span><span class="sxs-lookup"><span data-stu-id="1c2ac-147">displayName</span></span>|<span data-ttu-id="1c2ac-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c2ac-148">String</span></span>| <span data-ttu-id="1c2ac-149">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-149">Display name for this policy.</span></span> <span data-ttu-id="1c2ac-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-150">Required.</span></span>|
|<span data-ttu-id="1c2ac-151">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="1c2ac-151">isOrganizationDefault</span></span>|<span data-ttu-id="1c2ac-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c2ac-152">Boolean</span></span>|<span data-ttu-id="1c2ac-153">Se definido como true, ativa essa política.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-153">If set to true, activates this policy.</span></span> <span data-ttu-id="1c2ac-154">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-154">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="1c2ac-155">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-155">Optional, default value is false.</span></span>|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a><span data-ttu-id="1c2ac-156">Propriedades de uma definição de política de descoberta de domínio inicial</span><span class="sxs-lookup"><span data-stu-id="1c2ac-156">Properties of a home realm discovery policy definition</span></span>
<span data-ttu-id="1c2ac-157">As propriedades abaixo formam o objeto JSON que representa uma política de vida útil do token.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-157">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="1c2ac-158">Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com** aspas que escapam para serem inseridas na propriedade **definition.**</span><span class="sxs-lookup"><span data-stu-id="1c2ac-158">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="1c2ac-159">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="1c2ac-159">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"HomeRealmDiscoveryPolicy\":
     {\"AccelerateToFederatedDomain\":true,
      \"PreferredDomain\":\"federated.example.edu\",
      \"AlternateIdLogin\":{\"Enabled\":true}}}"
  ]
```

| <span data-ttu-id="1c2ac-160">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c2ac-160">Property</span></span>     | <span data-ttu-id="1c2ac-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c2ac-161">Type</span></span>   |<span data-ttu-id="1c2ac-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c2ac-162">Description</span></span>| 
|:---------------|:--------|:----------|
|<span data-ttu-id="1c2ac-163">AccelerateToFederatedDomain</span><span class="sxs-lookup"><span data-stu-id="1c2ac-163">AccelerateToFederatedDomain</span></span>|<span data-ttu-id="1c2ac-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c2ac-164">Boolean</span></span>| <span data-ttu-id="1c2ac-165">Definir como `true` para aceleração automática (ignorar descoberta de domínio inicial).</span><span class="sxs-lookup"><span data-stu-id="1c2ac-165">Set to `true` for auto-acceleration (bypass home realm discovery).</span></span> <span data-ttu-id="1c2ac-166">Se e houver apenas um domínio verificado e federado no locatário, os usuários serão levados diretamente para o provedor de identidade `true` federado (como ADFS) para entrar.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-166">If `true` and there is only one verified and federated domain in the tenant, then users will be taken straight to the federated identity provider (such as ADFS) for sign in.</span></span> <span data-ttu-id="1c2ac-167">Se `true` e houver mais de um domínio verificado no locatário, **PreferredDomain** deve ser especificado.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-167">If `true` and there is more than one verified domain in the tenant, **PreferredDomain** must be specified.</span></span> <span data-ttu-id="1c2ac-168">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-168">Optional.</span></span>|
|<span data-ttu-id="1c2ac-169">PreferredDomain</span><span class="sxs-lookup"><span data-stu-id="1c2ac-169">PreferredDomain</span></span>|<span data-ttu-id="1c2ac-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c2ac-170">String</span></span>| <span data-ttu-id="1c2ac-171">Especifica um domínio para acelerar a login.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-171">Specifies a domain to accelerate sign-in to.</span></span> <span data-ttu-id="1c2ac-172">Ele pode ser omitido se o locatário tiver apenas um domínio federado.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-172">It can be omitted if the tenant has only one federated domain.</span></span> <span data-ttu-id="1c2ac-173">Se for omitido e houver mais de um domínio federado verificado, essa política não terá efeito.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-173">If it is omitted, and there is more than one verified federated domain, this policy has no effect.</span></span> <span data-ttu-id="1c2ac-174">Obrigatório se **AccelerateToFederatedDomain** for `true` .</span><span class="sxs-lookup"><span data-stu-id="1c2ac-174">Required if **AccelerateToFederatedDomain** is `true`.</span></span>|
|<span data-ttu-id="1c2ac-175">AllowCloudPasswordValidation</span><span class="sxs-lookup"><span data-stu-id="1c2ac-175">AllowCloudPasswordValidation</span></span>|<span data-ttu-id="1c2ac-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c2ac-176">Boolean</span></span>| <span data-ttu-id="1c2ac-177">De acordo com a opção de permitir que um aplicativo autenture um usuário federado apresentando credenciais de nome de usuário/senha diretamente para o ponto de extremidade do token do `true` Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-177">Set to `true` to allow an application to authenticate a federated user by presenting username/password credentials directly to the Azure Active Directory token endpoint.</span></span> <span data-ttu-id="1c2ac-178">Só funciona se a Sincronização de Hash de Senha estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-178">Only works if Password Hash Sync is enabled.</span></span> <span data-ttu-id="1c2ac-179">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-179">Optional.</span></span>|
|<span data-ttu-id="1c2ac-180">AlternateIdLogin</span><span class="sxs-lookup"><span data-stu-id="1c2ac-180">AlternateIdLogin</span></span>| <span data-ttu-id="1c2ac-181">Json</span><span class="sxs-lookup"><span data-stu-id="1c2ac-181">Json</span></span> |<span data-ttu-id="1c2ac-182">De acordo com {"Enabled": true} para permitir a logon do Azure AD usando o email como uma [ID de logon alternativa.](/azure/active-directory/authentication/howto-authentication-use-email-signin)</span><span class="sxs-lookup"><span data-stu-id="1c2ac-182">Set to {"Enabled": true} to allow Azure AD sign-in using email as [an alternate login ID](/azure/active-directory/authentication/howto-authentication-use-email-signin).</span></span> <span data-ttu-id="1c2ac-183">Só funciona quando **IsOrganizationDefault** é definido como `true` .</span><span class="sxs-lookup"><span data-stu-id="1c2ac-183">Only works when **IsOrganizationDefault** is set to `true`.</span></span> <span data-ttu-id="1c2ac-184">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-184">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c2ac-185">Relações</span><span class="sxs-lookup"><span data-stu-id="1c2ac-185">Relationships</span></span>

| <span data-ttu-id="1c2ac-186">Relação</span><span class="sxs-lookup"><span data-stu-id="1c2ac-186">Relationship</span></span> | <span data-ttu-id="1c2ac-187">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c2ac-187">Type</span></span>        | <span data-ttu-id="1c2ac-188">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c2ac-188">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1c2ac-189">appliesTo</span><span class="sxs-lookup"><span data-stu-id="1c2ac-189">appliesTo</span></span>|<span data-ttu-id="1c2ac-190">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="1c2ac-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="1c2ac-191">A [coleção directoryObject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-191">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="1c2ac-192">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-192">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1c2ac-193">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1c2ac-193">JSON representation</span></span>

<span data-ttu-id="1c2ac-194">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1c2ac-194">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "homeRealmDiscoveryPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
