---
title: tipo de recurso claimsMappingPolicy
description: Representa uma política que pode controlar o tempo de vida de um token de acesso emitido pelo Azure Active Directory (Azure AD).
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a7f173cc8949dd0cf493620e08b5fdc5c61b8afb
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007007"
---
# <a name="claimsmappingpolicy-resource-type"></a><span data-ttu-id="1085f-103">tipo de recurso claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="1085f-103">claimsMappingPolicy resource type</span></span>

<span data-ttu-id="1085f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1085f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1085f-105">Representa as políticas de mapeamento de declaração para protocolos WS-Alimentad, SAML, OAuth 2,0 e OpenID Connect, para tokens emitidos para um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="1085f-105">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> <span data-ttu-id="1085f-106">Você pode usar políticas de mapeamento de declarações para:</span><span class="sxs-lookup"><span data-stu-id="1085f-106">You can use claims-mapping policies to:</span></span>

- <span data-ttu-id="1085f-107">Selecionar quais declarações são incluídas nos tokens</span><span class="sxs-lookup"><span data-stu-id="1085f-107">Select which claims are included in tokens</span></span>
- <span data-ttu-id="1085f-108">Criar tipos de declaração que ainda não existem</span><span class="sxs-lookup"><span data-stu-id="1085f-108">Create claim types that do not already exist</span></span>
- <span data-ttu-id="1085f-109">Escolha ou altere a fonte de dados emitidos em declarações específicas</span><span class="sxs-lookup"><span data-stu-id="1085f-109">Choose or change the source of data emitted in specific claims</span></span>  

<span data-ttu-id="1085f-110">Para obter mais detalhes de cenário e configuração, consulte [como: Personalizar declarações emitidas em tokens para um aplicativo específico em um locatário](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span><span class="sxs-lookup"><span data-stu-id="1085f-110">For more scenario and configuration details see [How to: Customize claims emitted in tokens for a specific app in a tenant](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span></span>

<span data-ttu-id="1085f-111">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1085f-111">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1085f-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="1085f-112">Methods</span></span>

| <span data-ttu-id="1085f-113">Método</span><span class="sxs-lookup"><span data-stu-id="1085f-113">Method</span></span>       | <span data-ttu-id="1085f-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1085f-114">Return Type</span></span> | <span data-ttu-id="1085f-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="1085f-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1085f-116">Criar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="1085f-116">Create claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [<span data-ttu-id="1085f-117">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="1085f-117">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="1085f-118">Criar um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="1085f-118">Create a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="1085f-119">Obter claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="1085f-119">Get claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-get.md) | [<span data-ttu-id="1085f-120">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="1085f-120">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="1085f-121">Ler propriedades e relações de um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="1085f-121">Read properties and relationships of a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="1085f-122">Listar claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="1085f-122">List claimsMappingPolicies</span></span>](../api/claimsmappingpolicy-list.md) | [<span data-ttu-id="1085f-123">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="1085f-123">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="1085f-124">Ler propriedades e relações de objetos claimsMappingPolicies.</span><span class="sxs-lookup"><span data-stu-id="1085f-124">Read properties and relationships of claimsMappingPolicies objects.</span></span> |
| [<span data-ttu-id="1085f-125">Atualizar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="1085f-125">Update claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-update.md) | <span data-ttu-id="1085f-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1085f-126">None</span></span> | <span data-ttu-id="1085f-127">Atualizar um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="1085f-127">Update a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="1085f-128">Excluir claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="1085f-128">Delete claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-delete.md) | <span data-ttu-id="1085f-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1085f-129">None</span></span> | <span data-ttu-id="1085f-130">Excluir um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="1085f-130">Delete a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="1085f-131">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="1085f-131">List appliesTo</span></span>](../api/claimsmappingpolicy-list-appliesto.md) | <span data-ttu-id="1085f-132">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="1085f-132">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="1085f-133">Obtenha a lista de directoryObjects à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="1085f-133">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="1085f-134">Atribuir claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="1085f-134">Assign claimsMappingPolicy</span></span>](../api/serviceprincipal-post-claimsmappingpolicies.md) | <span data-ttu-id="1085f-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1085f-135">None</span></span> | <span data-ttu-id="1085f-136">Atribuir um claimsMappingPolicy a um objeto [servicePrincipalName](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="1085f-136">Assign a claimsMappingPolicy to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="1085f-137">Lista atribuída claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="1085f-137">List assigned claimsMappingPolicy</span></span>](../api/serviceprincipal-list-claimsmappingpolicies.md) | <span data-ttu-id="1085f-138">Conjunto [claimsMappingPolicy](claimsmappingpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1085f-138">[claimsMappingPolicy](claimsmappingpolicy.md) collection</span></span> | <span data-ttu-id="1085f-139">Lista os objetos claimsMappingPolicy que são atribuídos a um objeto [servicePrincipalName](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="1085f-139">List the claimsMappingPolicy objects that are assigned to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="1085f-140">Remover claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="1085f-140">Remove claimsMappingPolicy</span></span>](../api/serviceprincipal-delete-claimsmappingpolicies.md) | <span data-ttu-id="1085f-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1085f-141">None</span></span> | <span data-ttu-id="1085f-142">Remover um claimsMappingPolicy de um objeto [servicePrincipalName](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="1085f-142">Remove a claimsMappingPolicy from a [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1085f-143">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1085f-143">Properties</span></span>

| <span data-ttu-id="1085f-144">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1085f-144">Property</span></span>     | <span data-ttu-id="1085f-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="1085f-145">Type</span></span>        | <span data-ttu-id="1085f-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="1085f-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1085f-147">id</span><span class="sxs-lookup"><span data-stu-id="1085f-147">id</span></span>|<span data-ttu-id="1085f-148">String</span><span class="sxs-lookup"><span data-stu-id="1085f-148">String</span></span>| <span data-ttu-id="1085f-149">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="1085f-149">Unique identifier for this policy.</span></span> <span data-ttu-id="1085f-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1085f-150">Read-only.</span></span>|
|<span data-ttu-id="1085f-151">definir</span><span class="sxs-lookup"><span data-stu-id="1085f-151">definition</span></span>|<span data-ttu-id="1085f-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1085f-152">String collection</span></span>| <span data-ttu-id="1085f-153">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="1085f-153">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="1085f-154">Veja mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="1085f-154">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="1085f-155">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1085f-155">Required.</span></span>|
|<span data-ttu-id="1085f-156">description</span><span class="sxs-lookup"><span data-stu-id="1085f-156">description</span></span>|<span data-ttu-id="1085f-157">String</span><span class="sxs-lookup"><span data-stu-id="1085f-157">String</span></span>| <span data-ttu-id="1085f-158">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="1085f-158">Description for this policy.</span></span>|
|<span data-ttu-id="1085f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1085f-159">displayName</span></span>|<span data-ttu-id="1085f-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1085f-160">String</span></span>| <span data-ttu-id="1085f-161">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="1085f-161">Display name for this policy.</span></span> <span data-ttu-id="1085f-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1085f-162">Required.</span></span>|
|<span data-ttu-id="1085f-163">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="1085f-163">isOrganizationDefault</span></span>|<span data-ttu-id="1085f-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="1085f-164">Boolean</span></span>|<span data-ttu-id="1085f-165">Ignore essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="1085f-165">Ignore this property.</span></span> <span data-ttu-id="1085f-166">A política de mapeamento de declarações só pode ser aplicada a entidades de serviço e não pode ser definida globalmente para a organização.</span><span class="sxs-lookup"><span data-stu-id="1085f-166">The claims-mapping policy can only be applied to service principals and can't be set globally for the organization.</span></span>|

### <a name="properties-of-a-claims-mapping-policy-definition"></a><span data-ttu-id="1085f-167">Propriedades de uma definição de política de mapeamento de declarações</span><span class="sxs-lookup"><span data-stu-id="1085f-167">Properties of a claims-mapping policy definition</span></span>

<span data-ttu-id="1085f-168">As propriedades abaixo formam o objeto JSON que representa uma política de mapeamento de declarações.</span><span class="sxs-lookup"><span data-stu-id="1085f-168">The properties below form the JSON object that represents a claims-mapping policy.</span></span> <span data-ttu-id="1085f-169">Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** .</span><span class="sxs-lookup"><span data-stu-id="1085f-169">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="1085f-170">Alguns exemplos de definição são mostrados abaixo:</span><span class="sxs-lookup"><span data-stu-id="1085f-170">A few definition examples are shown below:</span></span>

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a><span data-ttu-id="1085f-171">Exemplo: **definição** para incluir o EmployeeID e TenantCountry como declarações em tokens</span><span class="sxs-lookup"><span data-stu-id="1085f-171">Example: **definition** to include the EmployeeID and TenantCountry as claims in tokens</span></span>
<!-- {
  "blockType": "ignored"
}-->
``` json
{
  "definition": [
    "{\"ClaimsMappingPolicy\":{
      \"Version\":1,
      \"IncludeBasicClaimSet\":\"true\", 
      \"ClaimsSchema\": [
        {\"Source\":\"user\",\"ID\":\"employeeid\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/name\",\"JwtClaimType\":\"name\"},{\"Source\":\"company\",\"ID\":\"tenantcountry\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/country\",\"JwtClaimType\":\"country\"}
        ]
      }
    }"
  ]
}
```

#### <a name="example-definition-that-uses-a-claims-transformation"></a><span data-ttu-id="1085f-172">Exemplo: **definição** que usa uma transformação de declarações</span><span class="sxs-lookup"><span data-stu-id="1085f-172">Example: **definition** that uses a claims transformation</span></span>
<!-- {
  "blockType": "ignored"
}-->
``` json
{
  "definition": [
    "{\"ClaimsMappingPolicy\":{
      \"Version\":1,
      \"IncludeBasicClaimSet\":\"true\", 
      \"ClaimsSchema\":[
        {\"Source\":\"user\",\"ID\":\"extensionattribute1\"},{\"Source\":\"transformation\",\"ID\":\"DataJoin\",\"TransformationId\":\"JoinTheData\",\"JwtClaimType\":\"JoinedData\"}
        ],
      \"ClaimsTransformation\":[
        {\"ID\":\"JoinTheData\",\"TransformationMethod\":\"Join\",\"InputClaims\":[{\"ClaimTypeReferenceId\":\"extensionattribute1\",\"TransformationClaimType\":\"string1\"}], \"InputParameters\": [{\"ID\":\"string2\",\"Value\":\"sandbox\"},{\"ID\":\"separator\",\"Value\":\".\"}],\"OutputClaims\":[{\"ClaimTypeReferenceId\":\"DataJoin\",\"TransformationClaimType\":\"outputClaim\"}]}
        ]
      }
    }"
  ]
}
```

| <span data-ttu-id="1085f-173">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1085f-173">Property</span></span>     | <span data-ttu-id="1085f-174">Tipo</span><span class="sxs-lookup"><span data-stu-id="1085f-174">Type</span></span>   |<span data-ttu-id="1085f-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="1085f-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1085f-176">Versão</span><span class="sxs-lookup"><span data-stu-id="1085f-176">Version</span></span>|<span data-ttu-id="1085f-177">Número inteiro</span><span class="sxs-lookup"><span data-stu-id="1085f-177">Integer</span></span>|<span data-ttu-id="1085f-178">Defina o valor 1.</span><span class="sxs-lookup"><span data-stu-id="1085f-178">Set value of 1.</span></span> <span data-ttu-id="1085f-179">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1085f-179">Required.</span></span>|
|<span data-ttu-id="1085f-180">IncludeBasicClaimSet</span><span class="sxs-lookup"><span data-stu-id="1085f-180">IncludeBasicClaimSet</span></span>|<span data-ttu-id="1085f-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="1085f-181">Boolean</span></span>|<span data-ttu-id="1085f-182">Se for definido como true, todas as declarações no conjunto de declarações básicas serão emitidas em tokens afetados pela política.</span><span class="sxs-lookup"><span data-stu-id="1085f-182">If set to true, all claims in the basic claim set are emitted in tokens affected by the policy.</span></span> <span data-ttu-id="1085f-183">Se definido como false, as declarações no conjunto de declarações básicas não estão nos tokens, a menos que sejam individualmente adicionadas à propriedade ClaimsSchema da mesma política.</span><span class="sxs-lookup"><span data-stu-id="1085f-183">If set to false, claims in the basic claim set are not in the tokens, unless they are individually added in the ClaimsSchema property of the same policy.</span></span>|
|<span data-ttu-id="1085f-184">ClaimsSchema</span><span class="sxs-lookup"><span data-stu-id="1085f-184">ClaimsSchema</span></span>|<span data-ttu-id="1085f-185">Objeto JSON</span><span class="sxs-lookup"><span data-stu-id="1085f-185">JSON object</span></span>|<span data-ttu-id="1085f-186">Define quais declarações estão presentes nos tokens afetados pela política, além do conjunto de declarações básico e o conjunto de declarações principal.</span><span class="sxs-lookup"><span data-stu-id="1085f-186">Defines which claims are present in the tokens affected by the policy, in addition to the basic claim set and the core claim set.</span></span> <span data-ttu-id="1085f-187">Para cada entrada de esquema de declaração definida nessa propriedade, determinadas informações são necessárias.</span><span class="sxs-lookup"><span data-stu-id="1085f-187">For each claim schema entry defined in this property, certain information is required.</span></span> <span data-ttu-id="1085f-188">Especifique onde os dados vêm vindo (par de valor ou código-fonte/ID) e quais declarações os dados são emitidos como (tipo de declaração).</span><span class="sxs-lookup"><span data-stu-id="1085f-188">Specify where the data is coming from (Value or Source/ID pair), and which claim the data is emitted as (Claim Type).</span></span> <span data-ttu-id="1085f-189">Mais detalhes estão disponíveis na [definição ClaimsSchema](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span><span class="sxs-lookup"><span data-stu-id="1085f-189">Further details are available in the [ClaimsSchema definition](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span></span>|
|<span data-ttu-id="1085f-190">ClaimsTransformation</span><span class="sxs-lookup"><span data-stu-id="1085f-190">ClaimsTransformation</span></span>|<span data-ttu-id="1085f-191">Objeto JSON</span><span class="sxs-lookup"><span data-stu-id="1085f-191">JSON object</span></span>| <span data-ttu-id="1085f-192">Define transformações comuns que podem ser aplicadas aos dados de origem, para gerar os dados de saída para declarações especificadas no ClaimsSchema.</span><span class="sxs-lookup"><span data-stu-id="1085f-192">Defines common transformations that can be applied to source data, to generate the output data for claims specified in the ClaimsSchema.</span></span> <span data-ttu-id="1085f-193">Mais detalhes estão disponíveis na [definição ClaimsTransformation](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span><span class="sxs-lookup"><span data-stu-id="1085f-193">Further details are available in the [ClaimsTransformation definition](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span></span>|


## <a name="relationships"></a><span data-ttu-id="1085f-194">Relações</span><span class="sxs-lookup"><span data-stu-id="1085f-194">Relationships</span></span>

| <span data-ttu-id="1085f-195">Relação</span><span class="sxs-lookup"><span data-stu-id="1085f-195">Relationship</span></span> | <span data-ttu-id="1085f-196">Tipo</span><span class="sxs-lookup"><span data-stu-id="1085f-196">Type</span></span>        | <span data-ttu-id="1085f-197">Descrição</span><span class="sxs-lookup"><span data-stu-id="1085f-197">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1085f-198">appliesTo</span><span class="sxs-lookup"><span data-stu-id="1085f-198">appliesTo</span></span>|<span data-ttu-id="1085f-199">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="1085f-199">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="1085f-200">A coleção [directoryobject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="1085f-200">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="1085f-201">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1085f-201">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1085f-202">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1085f-202">JSON representation</span></span>

<span data-ttu-id="1085f-203">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1085f-203">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.claimsMappingPolicy",
  "baseType": "microsoft.graph.stsPolicy",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": false,
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "claimsMappingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->