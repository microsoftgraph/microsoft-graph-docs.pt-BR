---
title: tipo de recurso homeRealmDiscoveryPolicy
description: Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5e9c5d9933c2b98a1012291f02fa7e248bd403dd
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401432"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a><span data-ttu-id="ba91a-103">tipo de recurso homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="ba91a-103">homeRealmDiscoveryPolicy resource type</span></span>

<span data-ttu-id="ba91a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba91a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba91a-105">Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados, em particular para as restrições de aceleração automática e autenticação de usuário em domínios federados.</span><span class="sxs-lookup"><span data-stu-id="ba91a-105">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span> <span data-ttu-id="ba91a-106">Você pode definir homeRealmDiscoveryPolicy para todas as entidades de serviço em sua organização ou para entidades de serviço específicas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="ba91a-106">You can set homeRealmDiscoveryPolicy for all service principals in your organization, or for specific service principals in your organization.</span></span>  <span data-ttu-id="ba91a-107">Para obter mais detalhes de cenário e política, confira [Configurar o comportamento de entrada do Azure ad para um aplicativo usando uma política de descoberta de realm inicial](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal).</span><span class="sxs-lookup"><span data-stu-id="ba91a-107">For more scenario and policy details see [Configure Azure AD sign in behavior for an application by using a Home Realm Discovery policy](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal).</span></span>

<span data-ttu-id="ba91a-108">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ba91a-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ba91a-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="ba91a-109">Methods</span></span>

| <span data-ttu-id="ba91a-110">Método</span><span class="sxs-lookup"><span data-stu-id="ba91a-110">Method</span></span>       | <span data-ttu-id="ba91a-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ba91a-111">Return Type</span></span> | <span data-ttu-id="ba91a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba91a-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ba91a-113">Criar homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="ba91a-113">Create homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [<span data-ttu-id="ba91a-114">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="ba91a-114">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="ba91a-115">Criar um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="ba91a-115">Create a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="ba91a-116">Obter homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="ba91a-116">Get homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-get.md) | [<span data-ttu-id="ba91a-117">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="ba91a-117">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="ba91a-118">Ler propriedades e relações de um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="ba91a-118">Read properties and relationships of a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="ba91a-119">Listar homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="ba91a-119">List homeRealmDiscoveryPolicies</span></span>](../api/homerealmdiscoverypolicy-list.md) | [<span data-ttu-id="ba91a-120">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="ba91a-120">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="ba91a-121">Ler propriedades e relações de objetos homeRealmDiscoveryPolicies.</span><span class="sxs-lookup"><span data-stu-id="ba91a-121">Read properties and relationships of homeRealmDiscoveryPolicies objects.</span></span> |
| [<span data-ttu-id="ba91a-122">Atualizar homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="ba91a-122">Update homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-update.md) | <span data-ttu-id="ba91a-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ba91a-123">None</span></span> | <span data-ttu-id="ba91a-124">Atualizar um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="ba91a-124">Update a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="ba91a-125">Excluir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="ba91a-125">Delete homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-delete.md) | <span data-ttu-id="ba91a-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ba91a-126">None</span></span> | <span data-ttu-id="ba91a-127">Excluir um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="ba91a-127">Delete a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="ba91a-128">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="ba91a-128">List appliesTo</span></span>](../api/homerealmdiscoverypolicy-list-appliesto.md) | <span data-ttu-id="ba91a-129">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ba91a-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="ba91a-130">Obtenha a lista de directoryObjects à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="ba91a-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="ba91a-131">Atribuir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="ba91a-131">Assign homeRealmDiscoveryPolicy</span></span>](../api/serviceprincipal-post-homerealmdiscoverypolicies.md) | <span data-ttu-id="ba91a-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ba91a-132">None</span></span> | <span data-ttu-id="ba91a-133">Atribuir um objeto homeRealmDiscoveryPolicy a um objeto [servicePrincipalName](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="ba91a-133">Assign a homeRealmDiscoveryPolicy object to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="ba91a-134">Lista atribuída homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="ba91a-134">List assigned homeRealmDiscoveryPolicy</span></span>](../api/serviceprincipal-list-homerealmdiscoverypolicies.md) | <span data-ttu-id="ba91a-135">Conjunto [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ba91a-135">[homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) collection</span></span> | <span data-ttu-id="ba91a-136">Lista os objetos homeRealmDiscoveryPolicy que são atribuídos a um objeto [servicePrincipalName](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="ba91a-136">List the homeRealmDiscoveryPolicy objects that are assigned to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="ba91a-137">Remover homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="ba91a-137">Remove homeRealmDiscoveryPolicy</span></span>](../api/serviceprincipal-delete-homerealmdiscoverypolicies.md) | <span data-ttu-id="ba91a-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ba91a-138">None</span></span> | <span data-ttu-id="ba91a-139">Remover um objeto homeRealmDiscoveryPolicy de um objeto [servicePrincipalName](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="ba91a-139">Remove a homeRealmDiscoveryPolicy object from a [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ba91a-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba91a-140">Properties</span></span>

| <span data-ttu-id="ba91a-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba91a-141">Property</span></span>     | <span data-ttu-id="ba91a-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba91a-142">Type</span></span>        | <span data-ttu-id="ba91a-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba91a-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ba91a-144">id</span><span class="sxs-lookup"><span data-stu-id="ba91a-144">id</span></span>|<span data-ttu-id="ba91a-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba91a-145">String</span></span>| <span data-ttu-id="ba91a-146">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="ba91a-146">Unique identifier for this policy.</span></span> <span data-ttu-id="ba91a-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ba91a-147">Read-only.</span></span>|
|<span data-ttu-id="ba91a-148">definir</span><span class="sxs-lookup"><span data-stu-id="ba91a-148">definition</span></span>|<span data-ttu-id="ba91a-149">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba91a-149">String collection</span></span>| <span data-ttu-id="ba91a-150">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="ba91a-150">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="ba91a-151">Veja mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="ba91a-151">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="ba91a-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba91a-152">Required.</span></span>|
|<span data-ttu-id="ba91a-153">description</span><span class="sxs-lookup"><span data-stu-id="ba91a-153">description</span></span>|<span data-ttu-id="ba91a-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba91a-154">String</span></span>| <span data-ttu-id="ba91a-155">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="ba91a-155">Description for this policy.</span></span>|
|<span data-ttu-id="ba91a-156">displayName</span><span class="sxs-lookup"><span data-stu-id="ba91a-156">displayName</span></span>|<span data-ttu-id="ba91a-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba91a-157">String</span></span>| <span data-ttu-id="ba91a-158">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="ba91a-158">Display name for this policy.</span></span> <span data-ttu-id="ba91a-159">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba91a-159">Required.</span></span>|
|<span data-ttu-id="ba91a-160">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="ba91a-160">isOrganizationDefault</span></span>|<span data-ttu-id="ba91a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba91a-161">Boolean</span></span>|<span data-ttu-id="ba91a-162">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="ba91a-162">If set to true, activates this policy.</span></span> <span data-ttu-id="ba91a-163">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="ba91a-163">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="ba91a-164">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="ba91a-164">Optional, default value is false.</span></span>|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a><span data-ttu-id="ba91a-165">Propriedades de uma definição de política de descoberta de realm inicial</span><span class="sxs-lookup"><span data-stu-id="ba91a-165">Properties of a home realm discovery policy definition</span></span>
<span data-ttu-id="ba91a-166">As propriedades abaixo formam o objeto JSON que representa uma política de tempo de vida do token.</span><span class="sxs-lookup"><span data-stu-id="ba91a-166">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="ba91a-167">Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** .</span><span class="sxs-lookup"><span data-stu-id="ba91a-167">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="ba91a-168">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="ba91a-168">An example is shown below in JSON format:</span></span>

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

| <span data-ttu-id="ba91a-169">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba91a-169">Property</span></span>     | <span data-ttu-id="ba91a-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba91a-170">Type</span></span>   |<span data-ttu-id="ba91a-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba91a-171">Description</span></span>| 
|:---------------|:--------|:----------|
|<span data-ttu-id="ba91a-172">AccelerateToFederatedDomain</span><span class="sxs-lookup"><span data-stu-id="ba91a-172">AccelerateToFederatedDomain</span></span>|<span data-ttu-id="ba91a-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba91a-173">Boolean</span></span>| <span data-ttu-id="ba91a-174">Defina como `true` para aceleração automática (bypass da descoberta de realm inicial).</span><span class="sxs-lookup"><span data-stu-id="ba91a-174">Set to `true` for auto-acceleration (bypass home realm discovery).</span></span> <span data-ttu-id="ba91a-175">Se `true` e houver apenas um domínio verificado e federado no locatário, os usuários serão levados diretamente para o provedor de identidade federada (como ADFS) para entrar.</span><span class="sxs-lookup"><span data-stu-id="ba91a-175">If `true` and there is only one verified and federated domain in the tenant, then users will be taken straight to the federated identity provider (such as ADFS) for sign in.</span></span> <span data-ttu-id="ba91a-176">Se `true` houver mais de um domínio verificado no locatário, **PreferredDomain** deverá ser especificado.</span><span class="sxs-lookup"><span data-stu-id="ba91a-176">If `true` and there is more than one verified domain in the tenant, **PreferredDomain** must be specified.</span></span> <span data-ttu-id="ba91a-177">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ba91a-177">Optional.</span></span>|
|<span data-ttu-id="ba91a-178">PreferredDomain</span><span class="sxs-lookup"><span data-stu-id="ba91a-178">PreferredDomain</span></span>|<span data-ttu-id="ba91a-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba91a-179">String</span></span>| <span data-ttu-id="ba91a-180">Especifica um domínio para o qual acelerar o logon.</span><span class="sxs-lookup"><span data-stu-id="ba91a-180">Specifies a domain to accelerate sign-in to.</span></span> <span data-ttu-id="ba91a-181">Ele pode ser omitido se o locatário tiver apenas um domínio federado.</span><span class="sxs-lookup"><span data-stu-id="ba91a-181">It can be omitted if the tenant has only one federated domain.</span></span> <span data-ttu-id="ba91a-182">Se for omitido e houver mais de um domínio federado verificado, essa política não terá efeito.</span><span class="sxs-lookup"><span data-stu-id="ba91a-182">If it is omitted, and there is more than one verified federated domain, this policy has no effect.</span></span> <span data-ttu-id="ba91a-183">Obrigatório se **AccelerateToFederatedDomain** for `true` .</span><span class="sxs-lookup"><span data-stu-id="ba91a-183">Required if **AccelerateToFederatedDomain** is `true`.</span></span>|
|<span data-ttu-id="ba91a-184">AllowCloudPasswordValidation</span><span class="sxs-lookup"><span data-stu-id="ba91a-184">AllowCloudPasswordValidation</span></span>|<span data-ttu-id="ba91a-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba91a-185">Boolean</span></span>| <span data-ttu-id="ba91a-186">Defina como `true` para permitir que um aplicativo autentique um usuário federado, apresentando credenciais de nome de usuário/senha diretamente para o ponto de extremidade de token do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ba91a-186">Set to `true` to allow an application to authenticate a federated user by presenting username/password credentials directly to the Azure Active Directory token endpoint.</span></span> <span data-ttu-id="ba91a-187">Funcionará somente se a sincronização de hash de senha estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="ba91a-187">Only works if Password Hash Sync is enabled.</span></span> <span data-ttu-id="ba91a-188">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ba91a-188">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba91a-189">Relações</span><span class="sxs-lookup"><span data-stu-id="ba91a-189">Relationships</span></span>

| <span data-ttu-id="ba91a-190">Relação</span><span class="sxs-lookup"><span data-stu-id="ba91a-190">Relationship</span></span> | <span data-ttu-id="ba91a-191">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba91a-191">Type</span></span>        | <span data-ttu-id="ba91a-192">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba91a-192">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ba91a-193">appliesTo</span><span class="sxs-lookup"><span data-stu-id="ba91a-193">appliesTo</span></span>|<span data-ttu-id="ba91a-194">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ba91a-194">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="ba91a-195">A coleção [directoryobject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="ba91a-195">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="ba91a-196">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ba91a-196">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba91a-197">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba91a-197">JSON representation</span></span>

<span data-ttu-id="ba91a-198">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba91a-198">The following is a JSON representation of the resource.</span></span>

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