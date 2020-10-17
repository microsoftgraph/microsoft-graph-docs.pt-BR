---
title: tipo de recurso claimsMappingPolicy
description: Representa as políticas de mapeamento de declaração para protocolos WS-Alimentad, SAML, OAuth 2,0 e OpenID Connect, para tokens emitidos para um aplicativo específico.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e170008bf42cbf5d1d218d2b82570fc0dfff8444
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581271"
---
# <a name="claimsmappingpolicy-resource-type"></a><span data-ttu-id="8e6f4-103">tipo de recurso claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="8e6f4-103">claimsMappingPolicy resource type</span></span>

<span data-ttu-id="8e6f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e6f4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e6f4-105">Representa as políticas de mapeamento de declaração para protocolos WS-Alimentad, SAML, OAuth 2,0 e OpenID Connect, para tokens emitidos para um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-105">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> <span data-ttu-id="8e6f4-106">Você pode usar políticas de mapeamento de declarações para:</span><span class="sxs-lookup"><span data-stu-id="8e6f4-106">You can use claims-mapping policies to:</span></span>

- <span data-ttu-id="8e6f4-107">Selecionar quais declarações são incluídas nos tokens</span><span class="sxs-lookup"><span data-stu-id="8e6f4-107">Select which claims are included in tokens</span></span>
- <span data-ttu-id="8e6f4-108">Criar tipos de declaração que ainda não existem</span><span class="sxs-lookup"><span data-stu-id="8e6f4-108">Create claim types that do not already exist</span></span>
- <span data-ttu-id="8e6f4-109">Escolha ou altere a fonte de dados emitidos em declarações específicas</span><span class="sxs-lookup"><span data-stu-id="8e6f4-109">Choose or change the source of data emitted in specific claims</span></span>  

<span data-ttu-id="8e6f4-110">Para obter mais detalhes de cenário e configuração, consulte [como: Personalizar declarações emitidas em tokens para um aplicativo específico em um locatário](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span><span class="sxs-lookup"><span data-stu-id="8e6f4-110">For more scenario and configuration details see [How to: Customize claims emitted in tokens for a specific app in a tenant](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span></span>

<span data-ttu-id="8e6f4-111">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8e6f4-111">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8e6f4-112">Methods</span><span class="sxs-lookup"><span data-stu-id="8e6f4-112">Methods</span></span>

| <span data-ttu-id="8e6f4-113">Método</span><span class="sxs-lookup"><span data-stu-id="8e6f4-113">Method</span></span>       | <span data-ttu-id="8e6f4-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8e6f4-114">Return Type</span></span> | <span data-ttu-id="8e6f4-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e6f4-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8e6f4-116">Criar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="8e6f4-116">Create claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [<span data-ttu-id="8e6f4-117">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="8e6f4-117">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="8e6f4-118">Criar um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-118">Create a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="8e6f4-119">Obter claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="8e6f4-119">Get claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-get.md) | [<span data-ttu-id="8e6f4-120">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="8e6f4-120">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="8e6f4-121">Ler propriedades e relações de um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-121">Read properties and relationships of a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="8e6f4-122">Listar claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="8e6f4-122">List claimsMappingPolicies</span></span>](../api/claimsmappingpolicy-list.md) | [<span data-ttu-id="8e6f4-123">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="8e6f4-123">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="8e6f4-124">Ler propriedades e relações de objetos claimsMappingPolicies.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-124">Read properties and relationships of claimsMappingPolicies objects.</span></span> |
| [<span data-ttu-id="8e6f4-125">Atualizar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="8e6f4-125">Update claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-update.md) | <span data-ttu-id="8e6f4-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e6f4-126">None</span></span> | <span data-ttu-id="8e6f4-127">Atualizar um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-127">Update a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="8e6f4-128">Excluir claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="8e6f4-128">Delete claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-delete.md) | <span data-ttu-id="8e6f4-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e6f4-129">None</span></span> | <span data-ttu-id="8e6f4-130">Excluir um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-130">Delete a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="8e6f4-131">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="8e6f4-131">List appliesTo</span></span>](../api/claimsmappingpolicy-list-appliesto.md) | <span data-ttu-id="8e6f4-132">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="8e6f4-132">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="8e6f4-133">Obtenha a lista de directoryObjects à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-133">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="8e6f4-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e6f4-134">Properties</span></span>

| <span data-ttu-id="8e6f4-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e6f4-135">Property</span></span>     | <span data-ttu-id="8e6f4-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e6f4-136">Type</span></span>        | <span data-ttu-id="8e6f4-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e6f4-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8e6f4-138">id</span><span class="sxs-lookup"><span data-stu-id="8e6f4-138">id</span></span>|<span data-ttu-id="8e6f4-139">String</span><span class="sxs-lookup"><span data-stu-id="8e6f4-139">String</span></span>| <span data-ttu-id="8e6f4-140">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-140">Unique identifier for this policy.</span></span> <span data-ttu-id="8e6f4-141">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-141">Read-only.</span></span>|
|<span data-ttu-id="8e6f4-142">definir</span><span class="sxs-lookup"><span data-stu-id="8e6f4-142">definition</span></span>|<span data-ttu-id="8e6f4-143">String collection</span><span class="sxs-lookup"><span data-stu-id="8e6f4-143">String collection</span></span>| <span data-ttu-id="8e6f4-144">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-144">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="8e6f4-145">Veja mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-145">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="8e6f4-146">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-146">Required.</span></span>|
|<span data-ttu-id="8e6f4-147">description</span><span class="sxs-lookup"><span data-stu-id="8e6f4-147">description</span></span>|<span data-ttu-id="8e6f4-148">String</span><span class="sxs-lookup"><span data-stu-id="8e6f4-148">String</span></span>| <span data-ttu-id="8e6f4-149">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-149">Description for this policy.</span></span>|
|<span data-ttu-id="8e6f4-150">displayName</span><span class="sxs-lookup"><span data-stu-id="8e6f4-150">displayName</span></span>|<span data-ttu-id="8e6f4-151">String</span><span class="sxs-lookup"><span data-stu-id="8e6f4-151">String</span></span>| <span data-ttu-id="8e6f4-152">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-152">Display name for this policy.</span></span> <span data-ttu-id="8e6f4-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-153">Required.</span></span>|
|<span data-ttu-id="8e6f4-154">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="8e6f4-154">isOrganizationDefault</span></span>|<span data-ttu-id="8e6f4-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="8e6f4-155">Boolean</span></span>|<span data-ttu-id="8e6f4-156">Ignore essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-156">Ignore this property.</span></span> <span data-ttu-id="8e6f4-157">A política de mapeamento de declarações só pode ser aplicada a entidades de serviço e não pode ser definida globalmente para a organização.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-157">The claims-mapping policy can only be applied to service principals and can't be set globally for the organization.</span></span>|

### <a name="properties-of-a-claims-mapping-policy-definition"></a><span data-ttu-id="8e6f4-158">Propriedades de uma definição de política de mapeamento de declarações</span><span class="sxs-lookup"><span data-stu-id="8e6f4-158">Properties of a claims-mapping policy definition</span></span>

<span data-ttu-id="8e6f4-159">As propriedades abaixo formam o objeto JSON que representa uma política de mapeamento de declarações.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-159">The properties below form the JSON object that represents a claims-mapping policy.</span></span> <span data-ttu-id="8e6f4-160">Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** .</span><span class="sxs-lookup"><span data-stu-id="8e6f4-160">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="8e6f4-161">Alguns exemplos de definição são mostrados abaixo:</span><span class="sxs-lookup"><span data-stu-id="8e6f4-161">A few definition examples are shown below:</span></span>

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a><span data-ttu-id="8e6f4-162">Exemplo: **definição** para incluir o EmployeeID e TenantCountry como declarações em tokens</span><span class="sxs-lookup"><span data-stu-id="8e6f4-162">Example: **definition** to include the EmployeeID and TenantCountry as claims in tokens</span></span>
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

#### <a name="example-definition-that-uses-a-claims-transformation"></a><span data-ttu-id="8e6f4-163">Exemplo: **definição** que usa uma transformação de declarações</span><span class="sxs-lookup"><span data-stu-id="8e6f4-163">Example: **definition** that uses a claims transformation</span></span>
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

| <span data-ttu-id="8e6f4-164">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e6f4-164">Property</span></span>     | <span data-ttu-id="8e6f4-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e6f4-165">Type</span></span>   |<span data-ttu-id="8e6f4-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e6f4-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e6f4-167">Versão</span><span class="sxs-lookup"><span data-stu-id="8e6f4-167">Version</span></span>|<span data-ttu-id="8e6f4-168">Inteiro</span><span class="sxs-lookup"><span data-stu-id="8e6f4-168">Integer</span></span>|<span data-ttu-id="8e6f4-169">Defina o valor 1.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-169">Set value of 1.</span></span> <span data-ttu-id="8e6f4-170">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-170">Required.</span></span>|
|<span data-ttu-id="8e6f4-171">IncludeBasicClaimSet</span><span class="sxs-lookup"><span data-stu-id="8e6f4-171">IncludeBasicClaimSet</span></span>|<span data-ttu-id="8e6f4-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="8e6f4-172">Boolean</span></span>|<span data-ttu-id="8e6f4-173">Se for definido como true, todas as declarações no conjunto de declarações básicas serão emitidas em tokens afetados pela política.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-173">If set to true, all claims in the basic claim set are emitted in tokens affected by the policy.</span></span> <span data-ttu-id="8e6f4-174">Se definido como false, as declarações no conjunto de declarações básicas não estão nos tokens, a menos que sejam individualmente adicionadas à propriedade ClaimsSchema da mesma política.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-174">If set to false, claims in the basic claim set are not in the tokens, unless they are individually added in the ClaimsSchema property of the same policy.</span></span>|
|<span data-ttu-id="8e6f4-175">ClaimsSchema</span><span class="sxs-lookup"><span data-stu-id="8e6f4-175">ClaimsSchema</span></span>|<span data-ttu-id="8e6f4-176">Objeto JSON</span><span class="sxs-lookup"><span data-stu-id="8e6f4-176">JSON object</span></span>|<span data-ttu-id="8e6f4-177">Define quais declarações estão presentes nos tokens afetados pela política, além do conjunto de declarações básico e o conjunto de declarações principal.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-177">Defines which claims are present in the tokens affected by the policy, in addition to the basic claim set and the core claim set.</span></span> <span data-ttu-id="8e6f4-178">Para cada entrada de esquema de declaração definida nessa propriedade, determinadas informações são necessárias.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-178">For each claim schema entry defined in this property, certain information is required.</span></span> <span data-ttu-id="8e6f4-179">Especifique onde os dados vêm vindo (par de valor ou código-fonte/ID) e quais declarações os dados são emitidos como (tipo de declaração).</span><span class="sxs-lookup"><span data-stu-id="8e6f4-179">Specify where the data is coming from (Value or Source/ID pair), and which claim the data is emitted as (Claim Type).</span></span> <span data-ttu-id="8e6f4-180">Para obter mais informações, consulte [definição de ClaimsSchema](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span><span class="sxs-lookup"><span data-stu-id="8e6f4-180">For more information, see [ClaimsSchema definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span></span>|
|<span data-ttu-id="8e6f4-181">ClaimsTransformation</span><span class="sxs-lookup"><span data-stu-id="8e6f4-181">ClaimsTransformation</span></span>|<span data-ttu-id="8e6f4-182">Objeto JSON</span><span class="sxs-lookup"><span data-stu-id="8e6f4-182">JSON object</span></span>| <span data-ttu-id="8e6f4-183">Define transformações comuns que podem ser aplicadas aos dados de origem, para gerar os dados de saída para declarações especificadas no ClaimsSchema.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-183">Defines common transformations that can be applied to source data, to generate the output data for claims specified in the ClaimsSchema.</span></span> <span data-ttu-id="8e6f4-184">Para obter mais informações, consulte [definição de ClaimsTransformation](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span><span class="sxs-lookup"><span data-stu-id="8e6f4-184">For more information, see [ClaimsTransformation definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span></span>|


## <a name="relationships"></a><span data-ttu-id="8e6f4-185">Relações</span><span class="sxs-lookup"><span data-stu-id="8e6f4-185">Relationships</span></span>

| <span data-ttu-id="8e6f4-186">Relação</span><span class="sxs-lookup"><span data-stu-id="8e6f4-186">Relationship</span></span> | <span data-ttu-id="8e6f4-187">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e6f4-187">Type</span></span>        | <span data-ttu-id="8e6f4-188">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e6f4-188">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8e6f4-189">appliesTo</span><span class="sxs-lookup"><span data-stu-id="8e6f4-189">appliesTo</span></span>|<span data-ttu-id="8e6f4-190">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="8e6f4-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="8e6f4-191">A coleção [directoryobject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-191">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="8e6f4-192">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-192">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8e6f4-193">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e6f4-193">JSON representation</span></span>

<span data-ttu-id="8e6f4-194">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-194">The following is a JSON representation of the resource.</span></span>

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