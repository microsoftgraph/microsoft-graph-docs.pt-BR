---
title: tipo de recurso homeRealmDiscoveryPolicy
description: Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 62b0735fbf7d927cf7ee417a81a54a8cb5eb2473
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234119"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a><span data-ttu-id="b6f01-103">tipo de recurso homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b6f01-103">homeRealmDiscoveryPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6f01-104">Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados, em particular para as restrições de aceleração automática e autenticação de usuário em domínios federados.</span><span class="sxs-lookup"><span data-stu-id="b6f01-104">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span> <span data-ttu-id="b6f01-105">Você pode definir homeRealmDiscoveryPolicy para todas as entidades de serviço em sua organização ou para entidades de serviço específicas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="b6f01-105">You can set homeRealmDiscoveryPolicy for all service principals in your organization, or for specific service principals in your organization.</span></span>  <span data-ttu-id="b6f01-106">Para obter mais detalhes de cenário e política, confira [Configurar o comportamento de entrada do Azure ad para um aplicativo usando uma política de descoberta de realm inicial](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal).</span><span class="sxs-lookup"><span data-stu-id="b6f01-106">For more scenario and policy details see [Configure Azure AD sign in behavior for an application by using a Home Realm Discovery policy](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal).</span></span>

<span data-ttu-id="b6f01-107">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6f01-107">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b6f01-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b6f01-108">Methods</span></span>

| <span data-ttu-id="b6f01-109">Método</span><span class="sxs-lookup"><span data-stu-id="b6f01-109">Method</span></span>       | <span data-ttu-id="b6f01-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b6f01-110">Return Type</span></span> | <span data-ttu-id="b6f01-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6f01-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b6f01-112">Criar homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b6f01-112">Create homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [<span data-ttu-id="b6f01-113">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b6f01-113">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="b6f01-114">Criar um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="b6f01-114">Create a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="b6f01-115">Obter homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b6f01-115">Get homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-get.md) | [<span data-ttu-id="b6f01-116">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b6f01-116">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="b6f01-117">Ler propriedades e relações de um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="b6f01-117">Read properties and relationships of a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="b6f01-118">Listar homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="b6f01-118">List homeRealmDiscoveryPolicies</span></span>](../api/homerealmdiscoverypolicy-list.md) | [<span data-ttu-id="b6f01-119">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b6f01-119">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="b6f01-120">Ler propriedades e relações de objetos homeRealmDiscoveryPolicies.</span><span class="sxs-lookup"><span data-stu-id="b6f01-120">Read properties and relationships of homeRealmDiscoveryPolicies objects.</span></span> |
| [<span data-ttu-id="b6f01-121">Atualizar homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b6f01-121">Update homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-update.md) | <span data-ttu-id="b6f01-122">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b6f01-122">None</span></span> | <span data-ttu-id="b6f01-123">Atualizar um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="b6f01-123">Update a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="b6f01-124">Excluir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b6f01-124">Delete homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-delete.md) | <span data-ttu-id="b6f01-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b6f01-125">None</span></span> | <span data-ttu-id="b6f01-126">Excluir um objeto homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="b6f01-126">Delete a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="b6f01-127">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="b6f01-127">List appliesTo</span></span>](../api/homerealmdiscoverypolicy-list-appliesto.md) | <span data-ttu-id="b6f01-128">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="b6f01-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="b6f01-129">Obtenha a lista de directoryObjects à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="b6f01-129">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="b6f01-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6f01-130">Properties</span></span>

| <span data-ttu-id="b6f01-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6f01-131">Property</span></span>     | <span data-ttu-id="b6f01-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6f01-132">Type</span></span>        | <span data-ttu-id="b6f01-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6f01-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b6f01-134">id</span><span class="sxs-lookup"><span data-stu-id="b6f01-134">id</span></span>|<span data-ttu-id="b6f01-135">String</span><span class="sxs-lookup"><span data-stu-id="b6f01-135">String</span></span>| <span data-ttu-id="b6f01-136">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="b6f01-136">Unique identifier for this policy.</span></span> <span data-ttu-id="b6f01-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b6f01-137">Read-only.</span></span>|
|<span data-ttu-id="b6f01-138">definir</span><span class="sxs-lookup"><span data-stu-id="b6f01-138">definition</span></span>|<span data-ttu-id="b6f01-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6f01-139">String collection</span></span>| <span data-ttu-id="b6f01-140">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="b6f01-140">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="b6f01-141">Veja mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="b6f01-141">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="b6f01-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6f01-142">Required.</span></span>|
|<span data-ttu-id="b6f01-143">description</span><span class="sxs-lookup"><span data-stu-id="b6f01-143">description</span></span>|<span data-ttu-id="b6f01-144">String</span><span class="sxs-lookup"><span data-stu-id="b6f01-144">String</span></span>| <span data-ttu-id="b6f01-145">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="b6f01-145">Description for this policy.</span></span>|
|<span data-ttu-id="b6f01-146">displayName</span><span class="sxs-lookup"><span data-stu-id="b6f01-146">displayName</span></span>|<span data-ttu-id="b6f01-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6f01-147">String</span></span>| <span data-ttu-id="b6f01-148">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="b6f01-148">Display name for this policy.</span></span> <span data-ttu-id="b6f01-149">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6f01-149">Required.</span></span>|
|<span data-ttu-id="b6f01-150">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="b6f01-150">isOrganizationDefault</span></span>|<span data-ttu-id="b6f01-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6f01-151">Boolean</span></span>|<span data-ttu-id="b6f01-152">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="b6f01-152">If set to true, activates this policy.</span></span> <span data-ttu-id="b6f01-153">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="b6f01-153">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="b6f01-154">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="b6f01-154">Optional, default value is false.</span></span>|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a><span data-ttu-id="b6f01-155">Propriedades de uma definição de política de descoberta de realm inicial</span><span class="sxs-lookup"><span data-stu-id="b6f01-155">Properties of a home realm discovery policy definition</span></span>
<span data-ttu-id="b6f01-156">As propriedades abaixo formam o objeto JSON que representa uma política de tempo de vida do token.</span><span class="sxs-lookup"><span data-stu-id="b6f01-156">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="b6f01-157">Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** .</span><span class="sxs-lookup"><span data-stu-id="b6f01-157">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="b6f01-158">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="b6f01-158">An example is shown below in JSON format:</span></span>

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

| <span data-ttu-id="b6f01-159">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6f01-159">Property</span></span>     | <span data-ttu-id="b6f01-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6f01-160">Type</span></span>   |<span data-ttu-id="b6f01-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6f01-161">Description</span></span>| 
|:---------------|:--------|:----------|
|<span data-ttu-id="b6f01-162">AccelerateToFederatedDomain</span><span class="sxs-lookup"><span data-stu-id="b6f01-162">AccelerateToFederatedDomain</span></span>|<span data-ttu-id="b6f01-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6f01-163">Boolean</span></span>| <span data-ttu-id="b6f01-164">Defina como `true` para aceleração automática (bypass da descoberta de realm inicial).</span><span class="sxs-lookup"><span data-stu-id="b6f01-164">Set to `true` for auto-acceleration (bypass home realm discovery).</span></span> <span data-ttu-id="b6f01-165">Se `true` e houver apenas um domínio verificado e federado no locatário, os usuários serão levados diretamente para o provedor de identidade federada (como ADFS) para entrar.</span><span class="sxs-lookup"><span data-stu-id="b6f01-165">If `true` and there is only one verified and federated domain in the tenant, then users will be taken straight to the federated identity provider (such as ADFS) for sign in.</span></span> <span data-ttu-id="b6f01-166">Se `true` houver mais de um domínio verificado no locatário, **PreferredDomain** deverá ser especificado.</span><span class="sxs-lookup"><span data-stu-id="b6f01-166">If `true` and there is more than one verified domain in the tenant, **PreferredDomain** must be specified.</span></span> <span data-ttu-id="b6f01-167">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b6f01-167">Optional.</span></span>|
|<span data-ttu-id="b6f01-168">PreferredDomain</span><span class="sxs-lookup"><span data-stu-id="b6f01-168">PreferredDomain</span></span>|<span data-ttu-id="b6f01-169">String</span><span class="sxs-lookup"><span data-stu-id="b6f01-169">String</span></span>| <span data-ttu-id="b6f01-170">Especifica um domínio para o qual acelerar o logon.</span><span class="sxs-lookup"><span data-stu-id="b6f01-170">Specifies a domain to accelerate sign-in to.</span></span> <span data-ttu-id="b6f01-171">Ele pode ser omitido se o locatário tiver apenas um domínio federado.</span><span class="sxs-lookup"><span data-stu-id="b6f01-171">It can be omitted if the tenant has only one federated domain.</span></span> <span data-ttu-id="b6f01-172">Se for omitido e houver mais de um domínio federado verificado, essa política não terá efeito.</span><span class="sxs-lookup"><span data-stu-id="b6f01-172">If it is omitted, and there is more than one verified federated domain, this policy has no effect.</span></span> <span data-ttu-id="b6f01-173">Obrigatório se **AccelerateToFederatedDomain** for `true`.</span><span class="sxs-lookup"><span data-stu-id="b6f01-173">Required if **AccelerateToFederatedDomain** is `true`.</span></span>|
|<span data-ttu-id="b6f01-174">AllowCloudPasswordValidation</span><span class="sxs-lookup"><span data-stu-id="b6f01-174">AllowCloudPasswordValidation</span></span>|<span data-ttu-id="b6f01-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6f01-175">Boolean</span></span>| <span data-ttu-id="b6f01-176">Defina como `true` para permitir que um aplicativo autentique um usuário federado, apresentando credenciais de nome de usuário/senha diretamente para o ponto de extremidade de token do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b6f01-176">Set to `true` to allow an application to authenticate a federated user by presenting username/password credentials directly to the Azure Active Directory token endpoint.</span></span> <span data-ttu-id="b6f01-177">Funcionará somente se a sincronização de hash de senha estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="b6f01-177">Only works if Password Hash Sync is enabled.</span></span> <span data-ttu-id="b6f01-178">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b6f01-178">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6f01-179">Relações</span><span class="sxs-lookup"><span data-stu-id="b6f01-179">Relationships</span></span>

| <span data-ttu-id="b6f01-180">Relação</span><span class="sxs-lookup"><span data-stu-id="b6f01-180">Relationship</span></span> | <span data-ttu-id="b6f01-181">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6f01-181">Type</span></span>        | <span data-ttu-id="b6f01-182">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6f01-182">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b6f01-183">appliesTo</span><span class="sxs-lookup"><span data-stu-id="b6f01-183">appliesTo</span></span>|<span data-ttu-id="b6f01-184">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="b6f01-184">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="b6f01-185">A coleção [directoryobject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="b6f01-185">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="b6f01-186">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b6f01-186">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b6f01-187">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6f01-187">JSON representation</span></span>

<span data-ttu-id="b6f01-188">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6f01-188">The following is a JSON representation of the resource.</span></span>

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