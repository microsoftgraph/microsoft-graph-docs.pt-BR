---
title: Tipo de recurso homeRealmDiscoveryPolicy
description: Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 56e0d5b0e47c5f3ba5b37e4cbafad2138a2a7e79
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154205"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a><span data-ttu-id="02d60-103">Tipo de recurso homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="02d60-103">homeRealmDiscoveryPolicy resource type</span></span>

<span data-ttu-id="02d60-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02d60-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="02d60-105">Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados, em particular para restrições de aceleração automática e autenticação de usuário em domínios federados.</span><span class="sxs-lookup"><span data-stu-id="02d60-105">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span> <span data-ttu-id="02d60-106">Você pode definir **homeRealmDiscoveryPolicy** para todas as entidades de serviço em sua organização ou para entidades de serviço específicas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="02d60-106">You can set **homeRealmDiscoveryPolicy** for all service principals in your organization, or for specific service principals in your organization.</span></span> <span data-ttu-id="02d60-107">Para obter mais cenários e detalhes de política, confira Configurar o comportamento de logon do [Azure AD](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) para um aplicativo usando uma política de Descoberta de Realm Inicial, bem como entrar no [Azure Active Directory](/azure/active-directory/authentication/howto-authentication-use-email-signin)usando email como uma ID de logon alternativa.</span><span class="sxs-lookup"><span data-stu-id="02d60-107">For more scenario and policy details, see [Configure Azure AD sign in behavior for an application by using a Home Realm Discovery policy](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) as well as [Sign-in to Azure Active Directory using email as an alternate login ID](/azure/active-directory/authentication/howto-authentication-use-email-signin).</span></span>

<span data-ttu-id="02d60-108">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="02d60-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="02d60-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="02d60-109">Methods</span></span>

| <span data-ttu-id="02d60-110">Método</span><span class="sxs-lookup"><span data-stu-id="02d60-110">Method</span></span>       | <span data-ttu-id="02d60-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="02d60-111">Return Type</span></span> | <span data-ttu-id="02d60-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="02d60-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="02d60-113">Listar homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="02d60-113">List homeRealmDiscoveryPolicies</span></span>](../api/homerealmdiscoverypolicy-list.md) | [<span data-ttu-id="02d60-114">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="02d60-114">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="02d60-115">Leia as propriedades e as relações dos objetos homeRealmDiscoveryPolicies.</span><span class="sxs-lookup"><span data-stu-id="02d60-115">Read properties and relationships of homeRealmDiscoveryPolicies objects.</span></span> |
| [<span data-ttu-id="02d60-116">Criar homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="02d60-116">Create homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [<span data-ttu-id="02d60-117">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="02d60-117">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="02d60-118">Crie um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="02d60-118">Create a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="02d60-119">Obter homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="02d60-119">Get homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-get.md) | [<span data-ttu-id="02d60-120">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="02d60-120">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="02d60-121">Ler propriedades e relações de um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="02d60-121">Read properties and relationships of a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="02d60-122">Atualizar homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="02d60-122">Update homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-update.md) | <span data-ttu-id="02d60-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="02d60-123">None</span></span> | <span data-ttu-id="02d60-124">Atualize um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="02d60-124">Update a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="02d60-125">Excluir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="02d60-125">Delete homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-delete.md) | <span data-ttu-id="02d60-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="02d60-126">None</span></span> | <span data-ttu-id="02d60-127">Exclua um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="02d60-127">Delete a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="02d60-128">Lista appliesTo</span><span class="sxs-lookup"><span data-stu-id="02d60-128">List appliesTo</span></span>](../api/homerealmdiscoverypolicy-list-appliesto.md) | <span data-ttu-id="02d60-129">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="02d60-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="02d60-130">Obter a lista de directoryObjects aos qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="02d60-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="02d60-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="02d60-131">Properties</span></span>

| <span data-ttu-id="02d60-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02d60-132">Property</span></span>     | <span data-ttu-id="02d60-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="02d60-133">Type</span></span>        | <span data-ttu-id="02d60-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="02d60-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="02d60-135">id</span><span class="sxs-lookup"><span data-stu-id="02d60-135">id</span></span>|<span data-ttu-id="02d60-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02d60-136">String</span></span>| <span data-ttu-id="02d60-137">Identificador exclusivo desta política.</span><span class="sxs-lookup"><span data-stu-id="02d60-137">Unique identifier for this policy.</span></span> <span data-ttu-id="02d60-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="02d60-138">Read-only.</span></span>|
|<span data-ttu-id="02d60-139">definição</span><span class="sxs-lookup"><span data-stu-id="02d60-139">definition</span></span>|<span data-ttu-id="02d60-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="02d60-140">String collection</span></span>| <span data-ttu-id="02d60-141">Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política.</span><span class="sxs-lookup"><span data-stu-id="02d60-141">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="02d60-142">Veja abaixo para obter mais detalhes sobre o esquema JSON para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="02d60-142">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="02d60-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02d60-143">Required.</span></span>|
|<span data-ttu-id="02d60-144">description</span><span class="sxs-lookup"><span data-stu-id="02d60-144">description</span></span>|<span data-ttu-id="02d60-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02d60-145">String</span></span>| <span data-ttu-id="02d60-146">Descrição desta política.</span><span class="sxs-lookup"><span data-stu-id="02d60-146">Description for this policy.</span></span>|
|<span data-ttu-id="02d60-147">displayName</span><span class="sxs-lookup"><span data-stu-id="02d60-147">displayName</span></span>|<span data-ttu-id="02d60-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02d60-148">String</span></span>| <span data-ttu-id="02d60-149">Nome para exibição desta política.</span><span class="sxs-lookup"><span data-stu-id="02d60-149">Display name for this policy.</span></span> <span data-ttu-id="02d60-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02d60-150">Required.</span></span>|
|<span data-ttu-id="02d60-151">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="02d60-151">isOrganizationDefault</span></span>|<span data-ttu-id="02d60-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="02d60-152">Boolean</span></span>|<span data-ttu-id="02d60-153">Se definido como true, ativa essa política.</span><span class="sxs-lookup"><span data-stu-id="02d60-153">If set to true, activates this policy.</span></span> <span data-ttu-id="02d60-154">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="02d60-154">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="02d60-155">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="02d60-155">Optional, default value is false.</span></span>|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a><span data-ttu-id="02d60-156">Propriedades de uma definição de política de descoberta de realm inicial</span><span class="sxs-lookup"><span data-stu-id="02d60-156">Properties of a home realm discovery policy definition</span></span>
<span data-ttu-id="02d60-157">As propriedades abaixo formam o objeto JSON que representa uma política de tempo de vida do token.</span><span class="sxs-lookup"><span data-stu-id="02d60-157">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="02d60-158">Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas que** não devem ser inseridas na propriedade de **definição.**</span><span class="sxs-lookup"><span data-stu-id="02d60-158">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="02d60-159">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="02d60-159">An example is shown below in JSON format:</span></span>

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

| <span data-ttu-id="02d60-160">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02d60-160">Property</span></span>     | <span data-ttu-id="02d60-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="02d60-161">Type</span></span>   |<span data-ttu-id="02d60-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="02d60-162">Description</span></span>| 
|:---------------|:--------|:----------|
|<span data-ttu-id="02d60-163">AccelerateToFederatedDomain</span><span class="sxs-lookup"><span data-stu-id="02d60-163">AccelerateToFederatedDomain</span></span>|<span data-ttu-id="02d60-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="02d60-164">Boolean</span></span>| <span data-ttu-id="02d60-165">Definido como `true` para aceleração automática (ignorar descoberta de realm inicial).</span><span class="sxs-lookup"><span data-stu-id="02d60-165">Set to `true` for auto-acceleration (bypass home realm discovery).</span></span> <span data-ttu-id="02d60-166">Se e houver apenas um domínio verificado e federado no locatário, os usuários serão levados diretamente para o provedor de identidade `true` federado (como a ADFS) para entrar.</span><span class="sxs-lookup"><span data-stu-id="02d60-166">If `true` and there is only one verified and federated domain in the tenant, then users will be taken straight to the federated identity provider (such as ADFS) for sign in.</span></span> <span data-ttu-id="02d60-167">Se `true` houver mais de um domínio verificado no locatário, **PreferredDomain** deverá ser especificado.</span><span class="sxs-lookup"><span data-stu-id="02d60-167">If `true` and there is more than one verified domain in the tenant, **PreferredDomain** must be specified.</span></span> <span data-ttu-id="02d60-168">Opcional.</span><span class="sxs-lookup"><span data-stu-id="02d60-168">Optional.</span></span>|
|<span data-ttu-id="02d60-169">PreferredDomain</span><span class="sxs-lookup"><span data-stu-id="02d60-169">PreferredDomain</span></span>|<span data-ttu-id="02d60-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02d60-170">String</span></span>| <span data-ttu-id="02d60-171">Especifica um domínio para acelerar a login.</span><span class="sxs-lookup"><span data-stu-id="02d60-171">Specifies a domain to accelerate sign-in to.</span></span> <span data-ttu-id="02d60-172">Ele poderá ser omitido se o locatário tiver apenas um domínio federado.</span><span class="sxs-lookup"><span data-stu-id="02d60-172">It can be omitted if the tenant has only one federated domain.</span></span> <span data-ttu-id="02d60-173">Se for omitida e houver mais de um domínio federado verificado, essa política não terá efeito.</span><span class="sxs-lookup"><span data-stu-id="02d60-173">If it is omitted, and there is more than one verified federated domain, this policy has no effect.</span></span> <span data-ttu-id="02d60-174">Obrigatório se **AccelerateToFederatedDomain** for `true` .</span><span class="sxs-lookup"><span data-stu-id="02d60-174">Required if **AccelerateToFederatedDomain** is `true`.</span></span>|
|<span data-ttu-id="02d60-175">AllowCloudPasswordValidation</span><span class="sxs-lookup"><span data-stu-id="02d60-175">AllowCloudPasswordValidation</span></span>|<span data-ttu-id="02d60-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="02d60-176">Boolean</span></span>| <span data-ttu-id="02d60-177">Definido para permitir que um aplicativo autenti um usuário federado apresentando credenciais de nome de usuário/senha diretamente para o ponto de extremidade de token do `true` Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="02d60-177">Set to `true` to allow an application to authenticate a federated user by presenting username/password credentials directly to the Azure Active Directory token endpoint.</span></span> <span data-ttu-id="02d60-178">Só funcionará se a Sincronização de Hash de Senha estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="02d60-178">Only works if Password Hash Sync is enabled.</span></span> <span data-ttu-id="02d60-179">Opcional.</span><span class="sxs-lookup"><span data-stu-id="02d60-179">Optional.</span></span>|
|<span data-ttu-id="02d60-180">AlternateIdLogin</span><span class="sxs-lookup"><span data-stu-id="02d60-180">AlternateIdLogin</span></span>| <span data-ttu-id="02d60-181">Json</span><span class="sxs-lookup"><span data-stu-id="02d60-181">Json</span></span> |<span data-ttu-id="02d60-182">De definida como {"Enabled": true} para permitir que o Azure AD entre usando email como uma [ID de logon alternativa.](/azure/active-directory/authentication/howto-authentication-use-email-signin)</span><span class="sxs-lookup"><span data-stu-id="02d60-182">Set to {"Enabled": true} to allow Azure AD sign-in using email as [an alternate login ID](/azure/active-directory/authentication/howto-authentication-use-email-signin).</span></span> <span data-ttu-id="02d60-183">Só funciona quando **IsOrganizationDefault** está definido como `true` .</span><span class="sxs-lookup"><span data-stu-id="02d60-183">Only works when **IsOrganizationDefault** is set to `true`.</span></span> <span data-ttu-id="02d60-184">Opcional.</span><span class="sxs-lookup"><span data-stu-id="02d60-184">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02d60-185">Relações</span><span class="sxs-lookup"><span data-stu-id="02d60-185">Relationships</span></span>

| <span data-ttu-id="02d60-186">Relação</span><span class="sxs-lookup"><span data-stu-id="02d60-186">Relationship</span></span> | <span data-ttu-id="02d60-187">Tipo</span><span class="sxs-lookup"><span data-stu-id="02d60-187">Type</span></span>        | <span data-ttu-id="02d60-188">Descrição</span><span class="sxs-lookup"><span data-stu-id="02d60-188">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="02d60-189">appliesTo</span><span class="sxs-lookup"><span data-stu-id="02d60-189">appliesTo</span></span>|<span data-ttu-id="02d60-190">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="02d60-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="02d60-191">A [coleção directoryObject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="02d60-191">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="02d60-192">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="02d60-192">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02d60-193">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="02d60-193">JSON representation</span></span>

<span data-ttu-id="02d60-194">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="02d60-194">The following is a JSON representation of the resource.</span></span>

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
