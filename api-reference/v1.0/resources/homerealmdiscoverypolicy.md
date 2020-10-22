---
title: tipo de recurso homeRealmDiscoveryPolicy
description: Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 94e39375648824819edb74a9707a5f1286f33087
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635184"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a><span data-ttu-id="90208-103">tipo de recurso homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="90208-103">homeRealmDiscoveryPolicy resource type</span></span>

<span data-ttu-id="90208-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90208-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90208-105">Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados, em particular para as restrições de aceleração automática e autenticação de usuário em domínios federados.</span><span class="sxs-lookup"><span data-stu-id="90208-105">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span> <span data-ttu-id="90208-106">Você pode definir **homeRealmDiscoveryPolicy** para todas as entidades de serviço em sua organização ou para entidades de serviço específicas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="90208-106">You can set **homeRealmDiscoveryPolicy** for all service principals in your organization, or for specific service principals in your organization.</span></span> <span data-ttu-id="90208-107">Para obter mais detalhes de cenário e política, consulte [Configurar o comportamento de entrada do Azure ad para um aplicativo usando uma política de descoberta de realm inicial](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) , bem como [entrar no Azure Active Directory usando email como uma ID de logon alternativa](/azure/active-directory/authentication/howto-authentication-use-email-signin).</span><span class="sxs-lookup"><span data-stu-id="90208-107">For more scenario and policy details, see [Configure Azure AD sign in behavior for an application by using a Home Realm Discovery policy](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) as well as [Sign-in to Azure Active Directory using email as an alternate login ID](/azure/active-directory/authentication/howto-authentication-use-email-signin).</span></span>

<span data-ttu-id="90208-108">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="90208-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="90208-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="90208-109">Methods</span></span>

| <span data-ttu-id="90208-110">Método</span><span class="sxs-lookup"><span data-stu-id="90208-110">Method</span></span>       | <span data-ttu-id="90208-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="90208-111">Return Type</span></span> | <span data-ttu-id="90208-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="90208-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="90208-113">Listar homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="90208-113">List homeRealmDiscoveryPolicies</span></span>](../api/homerealmdiscoverypolicy-list.md) | [<span data-ttu-id="90208-114">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="90208-114">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="90208-115">Ler propriedades e relações de objetos homeRealmDiscoveryPolicies.</span><span class="sxs-lookup"><span data-stu-id="90208-115">Read properties and relationships of homeRealmDiscoveryPolicies objects.</span></span> |
| [<span data-ttu-id="90208-116">Criar homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="90208-116">Create homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [<span data-ttu-id="90208-117">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="90208-117">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="90208-118">Criar um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="90208-118">Create a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="90208-119">Obter homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="90208-119">Get homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-get.md) | [<span data-ttu-id="90208-120">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="90208-120">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="90208-121">Ler propriedades e relações de um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="90208-121">Read properties and relationships of a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="90208-122">Atualizar homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="90208-122">Update homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-update.md) | <span data-ttu-id="90208-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90208-123">None</span></span> | <span data-ttu-id="90208-124">Atualizar um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="90208-124">Update a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="90208-125">Excluir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="90208-125">Delete homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-delete.md) | <span data-ttu-id="90208-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90208-126">None</span></span> | <span data-ttu-id="90208-127">Excluir um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="90208-127">Delete a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="90208-128">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="90208-128">List appliesTo</span></span>](../api/homerealmdiscoverypolicy-list-appliesto.md) | <span data-ttu-id="90208-129">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="90208-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="90208-130">Obtenha a lista de directoryObjects à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="90208-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="90208-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90208-131">Properties</span></span>

| <span data-ttu-id="90208-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90208-132">Property</span></span>     | <span data-ttu-id="90208-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="90208-133">Type</span></span>        | <span data-ttu-id="90208-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="90208-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="90208-135">id</span><span class="sxs-lookup"><span data-stu-id="90208-135">id</span></span>|<span data-ttu-id="90208-136">String</span><span class="sxs-lookup"><span data-stu-id="90208-136">String</span></span>| <span data-ttu-id="90208-137">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="90208-137">Unique identifier for this policy.</span></span> <span data-ttu-id="90208-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90208-138">Read-only.</span></span>|
|<span data-ttu-id="90208-139">definir</span><span class="sxs-lookup"><span data-stu-id="90208-139">definition</span></span>|<span data-ttu-id="90208-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="90208-140">String collection</span></span>| <span data-ttu-id="90208-141">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="90208-141">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="90208-142">Veja mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="90208-142">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="90208-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90208-143">Required.</span></span>|
|<span data-ttu-id="90208-144">description</span><span class="sxs-lookup"><span data-stu-id="90208-144">description</span></span>|<span data-ttu-id="90208-145">String</span><span class="sxs-lookup"><span data-stu-id="90208-145">String</span></span>| <span data-ttu-id="90208-146">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="90208-146">Description for this policy.</span></span>|
|<span data-ttu-id="90208-147">displayName</span><span class="sxs-lookup"><span data-stu-id="90208-147">displayName</span></span>|<span data-ttu-id="90208-148">String</span><span class="sxs-lookup"><span data-stu-id="90208-148">String</span></span>| <span data-ttu-id="90208-149">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="90208-149">Display name for this policy.</span></span> <span data-ttu-id="90208-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90208-150">Required.</span></span>|
|<span data-ttu-id="90208-151">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="90208-151">isOrganizationDefault</span></span>|<span data-ttu-id="90208-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="90208-152">Boolean</span></span>|<span data-ttu-id="90208-153">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="90208-153">If set to true, activates this policy.</span></span> <span data-ttu-id="90208-154">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="90208-154">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="90208-155">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="90208-155">Optional, default value is false.</span></span>|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a><span data-ttu-id="90208-156">Propriedades de uma definição de política de descoberta de realm inicial</span><span class="sxs-lookup"><span data-stu-id="90208-156">Properties of a home realm discovery policy definition</span></span>
<span data-ttu-id="90208-157">As propriedades abaixo formam o objeto JSON que representa uma política de tempo de vida do token.</span><span class="sxs-lookup"><span data-stu-id="90208-157">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="90208-158">Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** .</span><span class="sxs-lookup"><span data-stu-id="90208-158">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="90208-159">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="90208-159">An example is shown below in JSON format:</span></span>

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

| <span data-ttu-id="90208-160">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90208-160">Property</span></span>     | <span data-ttu-id="90208-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="90208-161">Type</span></span>   |<span data-ttu-id="90208-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="90208-162">Description</span></span>| 
|:---------------|:--------|:----------|
|<span data-ttu-id="90208-163">AccelerateToFederatedDomain</span><span class="sxs-lookup"><span data-stu-id="90208-163">AccelerateToFederatedDomain</span></span>|<span data-ttu-id="90208-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="90208-164">Boolean</span></span>| <span data-ttu-id="90208-165">Defina como `true` para aceleração automática (bypass da descoberta de realm inicial).</span><span class="sxs-lookup"><span data-stu-id="90208-165">Set to `true` for auto-acceleration (bypass home realm discovery).</span></span> <span data-ttu-id="90208-166">Se `true` e houver apenas um domínio verificado e federado no locatário, os usuários serão levados diretamente para o provedor de identidade federada (como ADFS) para entrar.</span><span class="sxs-lookup"><span data-stu-id="90208-166">If `true` and there is only one verified and federated domain in the tenant, then users will be taken straight to the federated identity provider (such as ADFS) for sign in.</span></span> <span data-ttu-id="90208-167">Se `true` houver mais de um domínio verificado no locatário, **PreferredDomain** deverá ser especificado.</span><span class="sxs-lookup"><span data-stu-id="90208-167">If `true` and there is more than one verified domain in the tenant, **PreferredDomain** must be specified.</span></span> <span data-ttu-id="90208-168">Opcional.</span><span class="sxs-lookup"><span data-stu-id="90208-168">Optional.</span></span>|
|<span data-ttu-id="90208-169">PreferredDomain</span><span class="sxs-lookup"><span data-stu-id="90208-169">PreferredDomain</span></span>|<span data-ttu-id="90208-170">String</span><span class="sxs-lookup"><span data-stu-id="90208-170">String</span></span>| <span data-ttu-id="90208-171">Especifica um domínio para o qual acelerar o logon.</span><span class="sxs-lookup"><span data-stu-id="90208-171">Specifies a domain to accelerate sign-in to.</span></span> <span data-ttu-id="90208-172">Ele pode ser omitido se o locatário tiver apenas um domínio federado.</span><span class="sxs-lookup"><span data-stu-id="90208-172">It can be omitted if the tenant has only one federated domain.</span></span> <span data-ttu-id="90208-173">Se for omitido e houver mais de um domínio federado verificado, essa política não terá efeito.</span><span class="sxs-lookup"><span data-stu-id="90208-173">If it is omitted, and there is more than one verified federated domain, this policy has no effect.</span></span> <span data-ttu-id="90208-174">Obrigatório se **AccelerateToFederatedDomain** for `true` .</span><span class="sxs-lookup"><span data-stu-id="90208-174">Required if **AccelerateToFederatedDomain** is `true`.</span></span>|
|<span data-ttu-id="90208-175">AllowCloudPasswordValidation</span><span class="sxs-lookup"><span data-stu-id="90208-175">AllowCloudPasswordValidation</span></span>|<span data-ttu-id="90208-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="90208-176">Boolean</span></span>| <span data-ttu-id="90208-177">Defina como `true` para permitir que um aplicativo autentique um usuário federado, apresentando credenciais de nome de usuário/senha diretamente para o ponto de extremidade de token do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="90208-177">Set to `true` to allow an application to authenticate a federated user by presenting username/password credentials directly to the Azure Active Directory token endpoint.</span></span> <span data-ttu-id="90208-178">Funcionará somente se a sincronização de hash de senha estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="90208-178">Only works if Password Hash Sync is enabled.</span></span> <span data-ttu-id="90208-179">Opcional.</span><span class="sxs-lookup"><span data-stu-id="90208-179">Optional.</span></span>|
|<span data-ttu-id="90208-180">AlternateIdLogin</span><span class="sxs-lookup"><span data-stu-id="90208-180">AlternateIdLogin</span></span>| <span data-ttu-id="90208-181">Json</span><span class="sxs-lookup"><span data-stu-id="90208-181">Json</span></span> |<span data-ttu-id="90208-182">Defina como {"Enabled": true} para permitir a entrada do Azure AD usando email como [uma ID de logon alternativa](https://docs.microsoft.com/azure/active-directory/authentication/howto-authentication-use-email-signin).</span><span class="sxs-lookup"><span data-stu-id="90208-182">Set to {"Enabled": true} to allow Azure AD sign-in using email as [an alternate login ID](https://docs.microsoft.com/azure/active-directory/authentication/howto-authentication-use-email-signin).</span></span> <span data-ttu-id="90208-183">Só funciona quando **IsOrganizationDefault** está definido como `true` .</span><span class="sxs-lookup"><span data-stu-id="90208-183">Only works when **IsOrganizationDefault** is set to `true`.</span></span> <span data-ttu-id="90208-184">Opcional.</span><span class="sxs-lookup"><span data-stu-id="90208-184">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90208-185">Relações</span><span class="sxs-lookup"><span data-stu-id="90208-185">Relationships</span></span>

| <span data-ttu-id="90208-186">Relação</span><span class="sxs-lookup"><span data-stu-id="90208-186">Relationship</span></span> | <span data-ttu-id="90208-187">Tipo</span><span class="sxs-lookup"><span data-stu-id="90208-187">Type</span></span>        | <span data-ttu-id="90208-188">Descrição</span><span class="sxs-lookup"><span data-stu-id="90208-188">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="90208-189">appliesTo</span><span class="sxs-lookup"><span data-stu-id="90208-189">appliesTo</span></span>|<span data-ttu-id="90208-190">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="90208-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="90208-191">A coleção [directoryobject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="90208-191">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="90208-192">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90208-192">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90208-193">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90208-193">JSON representation</span></span>

<span data-ttu-id="90208-194">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90208-194">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true,
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
