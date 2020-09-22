---
title: tipo de recurso homeRealmDiscoveryPolicy
description: Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ab4cde183f07235f42886bf1dcaba53def9aa0ec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013598"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a><span data-ttu-id="81b64-103">tipo de recurso homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="81b64-103">homeRealmDiscoveryPolicy resource type</span></span>

<span data-ttu-id="81b64-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81b64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81b64-105">Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados, em particular para as restrições de aceleração automática e autenticação de usuário em domínios federados.</span><span class="sxs-lookup"><span data-stu-id="81b64-105">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span> <span data-ttu-id="81b64-106">Você pode definir homeRealmDiscoveryPolicy para todas as entidades de serviço em sua organização ou para entidades de serviço específicas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="81b64-106">You can set homeRealmDiscoveryPolicy for all service principals in your organization, or for specific service principals in your organization.</span></span>  <span data-ttu-id="81b64-107">Para obter mais detalhes de cenário e política, confira [Configurar o comportamento de entrada do Azure ad para um aplicativo usando uma política de descoberta de realm inicial](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal).</span><span class="sxs-lookup"><span data-stu-id="81b64-107">For more scenario and policy details see [Configure Azure AD sign in behavior for an application by using a Home Realm Discovery policy](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal).</span></span>

<span data-ttu-id="81b64-108">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="81b64-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="81b64-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="81b64-109">Methods</span></span>

| <span data-ttu-id="81b64-110">Método</span><span class="sxs-lookup"><span data-stu-id="81b64-110">Method</span></span>       | <span data-ttu-id="81b64-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="81b64-111">Return Type</span></span> | <span data-ttu-id="81b64-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="81b64-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="81b64-113">Criar homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="81b64-113">Create homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [<span data-ttu-id="81b64-114">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="81b64-114">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="81b64-115">Criar um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="81b64-115">Create a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="81b64-116">Obter homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="81b64-116">Get homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-get.md) | [<span data-ttu-id="81b64-117">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="81b64-117">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="81b64-118">Ler propriedades e relações de um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="81b64-118">Read properties and relationships of a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="81b64-119">Listar homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="81b64-119">List homeRealmDiscoveryPolicies</span></span>](../api/homerealmdiscoverypolicy-list.md) | [<span data-ttu-id="81b64-120">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="81b64-120">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="81b64-121">Ler propriedades e relações de objetos homeRealmDiscoveryPolicies.</span><span class="sxs-lookup"><span data-stu-id="81b64-121">Read properties and relationships of homeRealmDiscoveryPolicies objects.</span></span> |
| [<span data-ttu-id="81b64-122">Atualizar homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="81b64-122">Update homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-update.md) | <span data-ttu-id="81b64-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81b64-123">None</span></span> | <span data-ttu-id="81b64-124">Atualizar um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="81b64-124">Update a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="81b64-125">Excluir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="81b64-125">Delete homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-delete.md) | <span data-ttu-id="81b64-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81b64-126">None</span></span> | <span data-ttu-id="81b64-127">Excluir um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="81b64-127">Delete a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="81b64-128">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="81b64-128">List appliesTo</span></span>](../api/homerealmdiscoverypolicy-list-appliesto.md) | <span data-ttu-id="81b64-129">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="81b64-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="81b64-130">Obtenha a lista de directoryObjects à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="81b64-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="81b64-131">Atribuir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="81b64-131">Assign homeRealmDiscoveryPolicy</span></span>](../api/serviceprincipal-post-homerealmdiscoverypolicies.md) | <span data-ttu-id="81b64-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81b64-132">None</span></span> | <span data-ttu-id="81b64-133">Atribuir um objeto homeRealmDiscoveryPolicy a um objeto [servicePrincipalName](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="81b64-133">Assign a homeRealmDiscoveryPolicy object to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="81b64-134">Lista atribuída homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="81b64-134">List assigned homeRealmDiscoveryPolicy</span></span>](../api/serviceprincipal-list-homerealmdiscoverypolicies.md) | <span data-ttu-id="81b64-135">Conjunto [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81b64-135">[homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) collection</span></span> | <span data-ttu-id="81b64-136">Lista os objetos homeRealmDiscoveryPolicy que são atribuídos a um objeto [servicePrincipalName](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="81b64-136">List the homeRealmDiscoveryPolicy objects that are assigned to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="81b64-137">Remover homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="81b64-137">Remove homeRealmDiscoveryPolicy</span></span>](../api/serviceprincipal-delete-homerealmdiscoverypolicies.md) | <span data-ttu-id="81b64-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81b64-138">None</span></span> | <span data-ttu-id="81b64-139">Remover um objeto homeRealmDiscoveryPolicy de um objeto [servicePrincipalName](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="81b64-139">Remove a homeRealmDiscoveryPolicy object from a [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="81b64-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81b64-140">Properties</span></span>

| <span data-ttu-id="81b64-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81b64-141">Property</span></span>     | <span data-ttu-id="81b64-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="81b64-142">Type</span></span>        | <span data-ttu-id="81b64-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="81b64-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="81b64-144">id</span><span class="sxs-lookup"><span data-stu-id="81b64-144">id</span></span>|<span data-ttu-id="81b64-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81b64-145">String</span></span>| <span data-ttu-id="81b64-146">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="81b64-146">Unique identifier for this policy.</span></span> <span data-ttu-id="81b64-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81b64-147">Read-only.</span></span>|
|<span data-ttu-id="81b64-148">definir</span><span class="sxs-lookup"><span data-stu-id="81b64-148">definition</span></span>|<span data-ttu-id="81b64-149">String collection</span><span class="sxs-lookup"><span data-stu-id="81b64-149">String collection</span></span>| <span data-ttu-id="81b64-150">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="81b64-150">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="81b64-151">Veja mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="81b64-151">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="81b64-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81b64-152">Required.</span></span>|
|<span data-ttu-id="81b64-153">description</span><span class="sxs-lookup"><span data-stu-id="81b64-153">description</span></span>|<span data-ttu-id="81b64-154">String</span><span class="sxs-lookup"><span data-stu-id="81b64-154">String</span></span>| <span data-ttu-id="81b64-155">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="81b64-155">Description for this policy.</span></span>|
|<span data-ttu-id="81b64-156">displayName</span><span class="sxs-lookup"><span data-stu-id="81b64-156">displayName</span></span>|<span data-ttu-id="81b64-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81b64-157">String</span></span>| <span data-ttu-id="81b64-158">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="81b64-158">Display name for this policy.</span></span> <span data-ttu-id="81b64-159">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81b64-159">Required.</span></span>|
|<span data-ttu-id="81b64-160">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="81b64-160">isOrganizationDefault</span></span>|<span data-ttu-id="81b64-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="81b64-161">Boolean</span></span>|<span data-ttu-id="81b64-162">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="81b64-162">If set to true, activates this policy.</span></span> <span data-ttu-id="81b64-163">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="81b64-163">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="81b64-164">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="81b64-164">Optional, default value is false.</span></span>|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a><span data-ttu-id="81b64-165">Propriedades de uma definição de política de descoberta de realm inicial</span><span class="sxs-lookup"><span data-stu-id="81b64-165">Properties of a home realm discovery policy definition</span></span>
<span data-ttu-id="81b64-166">As propriedades abaixo formam o objeto JSON que representa uma política de tempo de vida do token.</span><span class="sxs-lookup"><span data-stu-id="81b64-166">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="81b64-167">Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** .</span><span class="sxs-lookup"><span data-stu-id="81b64-167">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="81b64-168">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="81b64-168">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"HomeRealmDiscoveryPolicy\":
     {\"AccelerateToFederatedDomain\":true,
      \"PreferredDomain\":\"federated.example.edu\"}}"
  ]
```

| <span data-ttu-id="81b64-169">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81b64-169">Property</span></span>     | <span data-ttu-id="81b64-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="81b64-170">Type</span></span>   |<span data-ttu-id="81b64-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="81b64-171">Description</span></span>| 
|:---------------|:--------|:----------|
|<span data-ttu-id="81b64-172">AccelerateToFederatedDomain</span><span class="sxs-lookup"><span data-stu-id="81b64-172">AccelerateToFederatedDomain</span></span>|<span data-ttu-id="81b64-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="81b64-173">Boolean</span></span>| <span data-ttu-id="81b64-174">Defina como `true` para aceleração automática (bypass da descoberta de realm inicial).</span><span class="sxs-lookup"><span data-stu-id="81b64-174">Set to `true` for auto-acceleration (bypass home realm discovery).</span></span> <span data-ttu-id="81b64-175">Se `true` e houver apenas um domínio verificado e federado no locatário, os usuários serão levados diretamente para o provedor de identidade federada (como ADFS) para entrar.</span><span class="sxs-lookup"><span data-stu-id="81b64-175">If `true` and there is only one verified and federated domain in the tenant, then users will be taken straight to the federated identity provider (such as ADFS) for sign in.</span></span> <span data-ttu-id="81b64-176">Se `true` houver mais de um domínio verificado no locatário, **PreferredDomain** deverá ser especificado.</span><span class="sxs-lookup"><span data-stu-id="81b64-176">If `true` and there is more than one verified domain in the tenant, **PreferredDomain** must be specified.</span></span> <span data-ttu-id="81b64-177">Opcional.</span><span class="sxs-lookup"><span data-stu-id="81b64-177">Optional.</span></span>|
|<span data-ttu-id="81b64-178">PreferredDomain</span><span class="sxs-lookup"><span data-stu-id="81b64-178">PreferredDomain</span></span>|<span data-ttu-id="81b64-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81b64-179">String</span></span>| <span data-ttu-id="81b64-180">Especifica um domínio para o qual acelerar o logon.</span><span class="sxs-lookup"><span data-stu-id="81b64-180">Specifies a domain to accelerate sign-in to.</span></span> <span data-ttu-id="81b64-181">Ele pode ser omitido se o locatário tiver apenas um domínio federado.</span><span class="sxs-lookup"><span data-stu-id="81b64-181">It can be omitted if the tenant has only one federated domain.</span></span> <span data-ttu-id="81b64-182">Se for omitido e houver mais de um domínio federado verificado, essa política não terá efeito.</span><span class="sxs-lookup"><span data-stu-id="81b64-182">If it is omitted, and there is more than one verified federated domain, this policy has no effect.</span></span> <span data-ttu-id="81b64-183">Obrigatório se **AccelerateToFederatedDomain** for `true` .</span><span class="sxs-lookup"><span data-stu-id="81b64-183">Required if **AccelerateToFederatedDomain** is `true`.</span></span>|
|<span data-ttu-id="81b64-184">AllowCloudPasswordValidation</span><span class="sxs-lookup"><span data-stu-id="81b64-184">AllowCloudPasswordValidation</span></span>|<span data-ttu-id="81b64-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="81b64-185">Boolean</span></span>| <span data-ttu-id="81b64-186">Defina como `true` para permitir que um aplicativo autentique um usuário federado, apresentando credenciais de nome de usuário/senha diretamente para o ponto de extremidade de token do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="81b64-186">Set to `true` to allow an application to authenticate a federated user by presenting username/password credentials directly to the Azure Active Directory token endpoint.</span></span> <span data-ttu-id="81b64-187">Funcionará somente se a sincronização de hash de senha estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="81b64-187">Only works if Password Hash Sync is enabled.</span></span> <span data-ttu-id="81b64-188">Opcional.</span><span class="sxs-lookup"><span data-stu-id="81b64-188">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81b64-189">Relações</span><span class="sxs-lookup"><span data-stu-id="81b64-189">Relationships</span></span>

| <span data-ttu-id="81b64-190">Relação</span><span class="sxs-lookup"><span data-stu-id="81b64-190">Relationship</span></span> | <span data-ttu-id="81b64-191">Tipo</span><span class="sxs-lookup"><span data-stu-id="81b64-191">Type</span></span>        | <span data-ttu-id="81b64-192">Descrição</span><span class="sxs-lookup"><span data-stu-id="81b64-192">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="81b64-193">appliesTo</span><span class="sxs-lookup"><span data-stu-id="81b64-193">appliesTo</span></span>|<span data-ttu-id="81b64-194">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="81b64-194">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="81b64-195">A coleção [directoryobject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="81b64-195">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="81b64-196">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81b64-196">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81b64-197">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81b64-197">JSON representation</span></span>

<span data-ttu-id="81b64-198">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81b64-198">The following is a JSON representation of the resource.</span></span>

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

