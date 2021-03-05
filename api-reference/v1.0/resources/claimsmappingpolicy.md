---
title: tipo de recurso claimsMappingPolicy
description: Representa as políticas de mapeamento de declaração para protocolos WS-Fed, SAML, OAuth 2.0 e OpenID Connect para tokens emitidos para um aplicativo específico.
localization_priority: Normal
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9d75b442d77155636cda6834abaea99f4a40a3e2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448036"
---
# <a name="claimsmappingpolicy-resource-type"></a><span data-ttu-id="9fb4b-103">tipo de recurso claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="9fb4b-103">claimsMappingPolicy resource type</span></span>

<span data-ttu-id="9fb4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fb4b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9fb4b-105">Representa as políticas de mapeamento de declaração para protocolos WS-Fed, SAML, OAuth 2.0 e OpenID Connect para tokens emitidos para um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-105">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> <span data-ttu-id="9fb4b-106">Você pode usar políticas de mapeamento de declarações para:</span><span class="sxs-lookup"><span data-stu-id="9fb4b-106">You can use claims-mapping policies to:</span></span>

- <span data-ttu-id="9fb4b-107">Selecione quais declarações estão incluídas em tokens</span><span class="sxs-lookup"><span data-stu-id="9fb4b-107">Select which claims are included in tokens</span></span>
- <span data-ttu-id="9fb4b-108">Criar tipos de declaração que ainda não existem</span><span class="sxs-lookup"><span data-stu-id="9fb4b-108">Create claim types that do not already exist</span></span>
- <span data-ttu-id="9fb4b-109">Escolher ou alterar a fonte de dados emitidos em declarações específicas</span><span class="sxs-lookup"><span data-stu-id="9fb4b-109">Choose or change the source of data emitted in specific claims</span></span>  

<span data-ttu-id="9fb4b-110">Para obter mais detalhes de cenário e configuração, consulte [How to: Customize claims emitted in tokens for a specific app in a tenant](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span><span class="sxs-lookup"><span data-stu-id="9fb4b-110">For more scenario and configuration details see [How to: Customize claims emitted in tokens for a specific app in a tenant](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span></span>

<span data-ttu-id="9fb4b-111">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9fb4b-111">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9fb4b-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="9fb4b-112">Methods</span></span>

| <span data-ttu-id="9fb4b-113">Método</span><span class="sxs-lookup"><span data-stu-id="9fb4b-113">Method</span></span>       | <span data-ttu-id="9fb4b-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9fb4b-114">Return Type</span></span> | <span data-ttu-id="9fb4b-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fb4b-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9fb4b-116">Criar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="9fb4b-116">Create claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [<span data-ttu-id="9fb4b-117">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="9fb4b-117">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="9fb4b-118">Crie um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-118">Create a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="9fb4b-119">Obter claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="9fb4b-119">Get claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-get.md) | [<span data-ttu-id="9fb4b-120">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="9fb4b-120">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="9fb4b-121">Leia propriedades e relações de um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-121">Read properties and relationships of a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="9fb4b-122">Listar claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="9fb4b-122">List claimsMappingPolicies</span></span>](../api/claimsmappingpolicy-list.md) | [<span data-ttu-id="9fb4b-123">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="9fb4b-123">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="9fb4b-124">Ler propriedades e relações de objetos claimsMappingPolicies.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-124">Read properties and relationships of claimsMappingPolicies objects.</span></span> |
| [<span data-ttu-id="9fb4b-125">Update claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="9fb4b-125">Update claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-update.md) | <span data-ttu-id="9fb4b-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9fb4b-126">None</span></span> | <span data-ttu-id="9fb4b-127">Atualize um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-127">Update a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="9fb4b-128">Excluir claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="9fb4b-128">Delete claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-delete.md) | <span data-ttu-id="9fb4b-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9fb4b-129">None</span></span> | <span data-ttu-id="9fb4b-130">Exclua um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-130">Delete a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="9fb4b-131">Lista appliesTo</span><span class="sxs-lookup"><span data-stu-id="9fb4b-131">List appliesTo</span></span>](../api/claimsmappingpolicy-list-appliesto.md) | <span data-ttu-id="9fb4b-132">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="9fb4b-132">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="9fb4b-133">Obter a lista de directoryObjects aos qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-133">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="9fb4b-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9fb4b-134">Properties</span></span>

| <span data-ttu-id="9fb4b-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fb4b-135">Property</span></span>     | <span data-ttu-id="9fb4b-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fb4b-136">Type</span></span>        | <span data-ttu-id="9fb4b-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fb4b-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9fb4b-138">id</span><span class="sxs-lookup"><span data-stu-id="9fb4b-138">id</span></span>|<span data-ttu-id="9fb4b-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9fb4b-139">String</span></span>| <span data-ttu-id="9fb4b-140">Identificador exclusivo dessa política.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-140">Unique identifier for this policy.</span></span> <span data-ttu-id="9fb4b-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-141">Read-only.</span></span>|
|<span data-ttu-id="9fb4b-142">definition</span><span class="sxs-lookup"><span data-stu-id="9fb4b-142">definition</span></span>|<span data-ttu-id="9fb4b-143">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9fb4b-143">String collection</span></span>| <span data-ttu-id="9fb4b-144">Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-144">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="9fb4b-145">Consulte abaixo para obter mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-145">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="9fb4b-146">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-146">Required.</span></span>|
|<span data-ttu-id="9fb4b-147">description</span><span class="sxs-lookup"><span data-stu-id="9fb4b-147">description</span></span>|<span data-ttu-id="9fb4b-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9fb4b-148">String</span></span>| <span data-ttu-id="9fb4b-149">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-149">Description for this policy.</span></span>|
|<span data-ttu-id="9fb4b-150">displayName</span><span class="sxs-lookup"><span data-stu-id="9fb4b-150">displayName</span></span>|<span data-ttu-id="9fb4b-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9fb4b-151">String</span></span>| <span data-ttu-id="9fb4b-152">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-152">Display name for this policy.</span></span> <span data-ttu-id="9fb4b-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-153">Required.</span></span>|
|<span data-ttu-id="9fb4b-154">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="9fb4b-154">isOrganizationDefault</span></span>|<span data-ttu-id="9fb4b-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fb4b-155">Boolean</span></span>|<span data-ttu-id="9fb4b-156">Ignore essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-156">Ignore this property.</span></span> <span data-ttu-id="9fb4b-157">A política de mapeamento de declarações só pode ser aplicada a entidades de serviço e não pode ser definida globalmente para a organização.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-157">The claims-mapping policy can only be applied to service principals and can't be set globally for the organization.</span></span>|

### <a name="properties-of-a-claims-mapping-policy-definition"></a><span data-ttu-id="9fb4b-158">Propriedades de uma definição de política de mapeamento de declarações</span><span class="sxs-lookup"><span data-stu-id="9fb4b-158">Properties of a claims-mapping policy definition</span></span>

<span data-ttu-id="9fb4b-159">As propriedades abaixo formam o objeto JSON que representa uma política de mapeamento de declarações.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-159">The properties below form the JSON object that represents a claims-mapping policy.</span></span> <span data-ttu-id="9fb4b-160">Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com** aspas que escapam para serem inseridas na propriedade **definition.**</span><span class="sxs-lookup"><span data-stu-id="9fb4b-160">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="9fb4b-161">Alguns exemplos de definição são mostrados abaixo:</span><span class="sxs-lookup"><span data-stu-id="9fb4b-161">A few definition examples are shown below:</span></span>

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a><span data-ttu-id="9fb4b-162">Exemplo: **definição** para incluir EmployeeID e TenantCountry como declarações em tokens</span><span class="sxs-lookup"><span data-stu-id="9fb4b-162">Example: **definition** to include the EmployeeID and TenantCountry as claims in tokens</span></span>
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

#### <a name="example-definition-that-uses-a-claims-transformation"></a><span data-ttu-id="9fb4b-163">Exemplo: **definição** que usa uma transformação de declarações</span><span class="sxs-lookup"><span data-stu-id="9fb4b-163">Example: **definition** that uses a claims transformation</span></span>
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

| <span data-ttu-id="9fb4b-164">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fb4b-164">Property</span></span>     | <span data-ttu-id="9fb4b-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fb4b-165">Type</span></span>   |<span data-ttu-id="9fb4b-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fb4b-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fb4b-167">Versão</span><span class="sxs-lookup"><span data-stu-id="9fb4b-167">Version</span></span>|<span data-ttu-id="9fb4b-168">Inteiro</span><span class="sxs-lookup"><span data-stu-id="9fb4b-168">Integer</span></span>|<span data-ttu-id="9fb4b-169">Definir o valor de 1.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-169">Set value of 1.</span></span> <span data-ttu-id="9fb4b-170">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-170">Required.</span></span>|
|<span data-ttu-id="9fb4b-171">IncludeBasicClaimSet</span><span class="sxs-lookup"><span data-stu-id="9fb4b-171">IncludeBasicClaimSet</span></span>|<span data-ttu-id="9fb4b-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fb4b-172">Boolean</span></span>|<span data-ttu-id="9fb4b-173">Se definido como true, todas as declarações no conjunto de declarações básico são emitidas em tokens afetados pela política.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-173">If set to true, all claims in the basic claim set are emitted in tokens affected by the policy.</span></span> <span data-ttu-id="9fb4b-174">Se definido como false, as declarações no conjunto de declarações básicas não estão nos tokens, a menos que sejam adicionadas individualmente na propriedade ClaimsSchema da mesma política.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-174">If set to false, claims in the basic claim set are not in the tokens, unless they are individually added in the ClaimsSchema property of the same policy.</span></span>|
|<span data-ttu-id="9fb4b-175">ClaimsSchema</span><span class="sxs-lookup"><span data-stu-id="9fb4b-175">ClaimsSchema</span></span>|<span data-ttu-id="9fb4b-176">Objeto JSON</span><span class="sxs-lookup"><span data-stu-id="9fb4b-176">JSON object</span></span>|<span data-ttu-id="9fb4b-177">Define quais declarações estão presentes nos tokens afetados pela política, além do conjunto de declarações básico e do conjunto de declarações principais.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-177">Defines which claims are present in the tokens affected by the policy, in addition to the basic claim set and the core claim set.</span></span> <span data-ttu-id="9fb4b-178">Para cada entrada de esquema de declaração definida nesta propriedade, determinadas informações são necessárias.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-178">For each claim schema entry defined in this property, certain information is required.</span></span> <span data-ttu-id="9fb4b-179">Especifique de onde os dados estão vindo (par Valor ou Fonte/ID) e que dizem que os dados são emitidos como (Tipo de Declaração).</span><span class="sxs-lookup"><span data-stu-id="9fb4b-179">Specify where the data is coming from (Value or Source/ID pair), and which claim the data is emitted as (Claim Type).</span></span> <span data-ttu-id="9fb4b-180">Para obter mais informações, consulte [ClaimsSchema definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span><span class="sxs-lookup"><span data-stu-id="9fb4b-180">For more information, see [ClaimsSchema definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span></span>|
|<span data-ttu-id="9fb4b-181">ClaimsTransformation</span><span class="sxs-lookup"><span data-stu-id="9fb4b-181">ClaimsTransformation</span></span>|<span data-ttu-id="9fb4b-182">Objeto JSON</span><span class="sxs-lookup"><span data-stu-id="9fb4b-182">JSON object</span></span>| <span data-ttu-id="9fb4b-183">Define transformações comuns que podem ser aplicadas aos dados de origem, para gerar os dados de saída para declarações especificadas no ClaimsSchema.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-183">Defines common transformations that can be applied to source data, to generate the output data for claims specified in the ClaimsSchema.</span></span> <span data-ttu-id="9fb4b-184">Para obter mais informações, consulte [ClaimsTransformation definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span><span class="sxs-lookup"><span data-stu-id="9fb4b-184">For more information, see [ClaimsTransformation definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span></span>|


## <a name="relationships"></a><span data-ttu-id="9fb4b-185">Relações</span><span class="sxs-lookup"><span data-stu-id="9fb4b-185">Relationships</span></span>

| <span data-ttu-id="9fb4b-186">Relação</span><span class="sxs-lookup"><span data-stu-id="9fb4b-186">Relationship</span></span> | <span data-ttu-id="9fb4b-187">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fb4b-187">Type</span></span>        | <span data-ttu-id="9fb4b-188">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fb4b-188">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9fb4b-189">appliesTo</span><span class="sxs-lookup"><span data-stu-id="9fb4b-189">appliesTo</span></span>|<span data-ttu-id="9fb4b-190">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="9fb4b-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="9fb4b-191">A [coleção directoryObject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-191">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="9fb4b-192">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-192">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9fb4b-193">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9fb4b-193">JSON representation</span></span>

<span data-ttu-id="9fb4b-194">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9fb4b-194">The following is a JSON representation of the resource.</span></span>

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
