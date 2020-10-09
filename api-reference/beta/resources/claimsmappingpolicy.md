---
title: tipo de recurso claimsMappingPolicy
description: Representa uma política que pode controlar o tempo de vida de um token de acesso emitido pelo Azure Active Directory (Azure AD).
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 09d68f6c9561ba0bf433c56abbba640b485a6fba
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405600"
---
# <a name="claimsmappingpolicy-resource-type"></a><span data-ttu-id="46bd8-103">tipo de recurso claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="46bd8-103">claimsMappingPolicy resource type</span></span>

<span data-ttu-id="46bd8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46bd8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46bd8-105">Representa as políticas de mapeamento de declaração para protocolos WS-Alimentad, SAML, OAuth 2,0 e OpenID Connect, para tokens emitidos para um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="46bd8-105">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> <span data-ttu-id="46bd8-106">Você pode usar políticas de mapeamento de declarações para:</span><span class="sxs-lookup"><span data-stu-id="46bd8-106">You can use claims-mapping policies to:</span></span>

- <span data-ttu-id="46bd8-107">Selecionar quais declarações são incluídas nos tokens</span><span class="sxs-lookup"><span data-stu-id="46bd8-107">Select which claims are included in tokens</span></span>
- <span data-ttu-id="46bd8-108">Criar tipos de declaração que ainda não existem</span><span class="sxs-lookup"><span data-stu-id="46bd8-108">Create claim types that do not already exist</span></span>
- <span data-ttu-id="46bd8-109">Escolha ou altere a fonte de dados emitidos em declarações específicas</span><span class="sxs-lookup"><span data-stu-id="46bd8-109">Choose or change the source of data emitted in specific claims</span></span>  

<span data-ttu-id="46bd8-110">Para obter mais detalhes de cenário e configuração, consulte [como: Personalizar declarações emitidas em tokens para um aplicativo específico em um locatário](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span><span class="sxs-lookup"><span data-stu-id="46bd8-110">For more scenario and configuration details see [How to: Customize claims emitted in tokens for a specific app in a tenant](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span></span>

<span data-ttu-id="46bd8-111">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="46bd8-111">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="46bd8-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="46bd8-112">Methods</span></span>

| <span data-ttu-id="46bd8-113">Método</span><span class="sxs-lookup"><span data-stu-id="46bd8-113">Method</span></span>       | <span data-ttu-id="46bd8-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="46bd8-114">Return Type</span></span> | <span data-ttu-id="46bd8-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="46bd8-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="46bd8-116">Criar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="46bd8-116">Create claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [<span data-ttu-id="46bd8-117">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="46bd8-117">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="46bd8-118">Criar um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="46bd8-118">Create a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="46bd8-119">Obter claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="46bd8-119">Get claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-get.md) | [<span data-ttu-id="46bd8-120">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="46bd8-120">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="46bd8-121">Ler propriedades e relações de um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="46bd8-121">Read properties and relationships of a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="46bd8-122">Listar claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="46bd8-122">List claimsMappingPolicies</span></span>](../api/claimsmappingpolicy-list.md) | [<span data-ttu-id="46bd8-123">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="46bd8-123">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="46bd8-124">Ler propriedades e relações de objetos claimsMappingPolicies.</span><span class="sxs-lookup"><span data-stu-id="46bd8-124">Read properties and relationships of claimsMappingPolicies objects.</span></span> |
| [<span data-ttu-id="46bd8-125">Atualizar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="46bd8-125">Update claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-update.md) | <span data-ttu-id="46bd8-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46bd8-126">None</span></span> | <span data-ttu-id="46bd8-127">Atualizar um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="46bd8-127">Update a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="46bd8-128">Excluir claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="46bd8-128">Delete claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-delete.md) | <span data-ttu-id="46bd8-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46bd8-129">None</span></span> | <span data-ttu-id="46bd8-130">Excluir um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="46bd8-130">Delete a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="46bd8-131">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="46bd8-131">List appliesTo</span></span>](../api/claimsmappingpolicy-list-appliesto.md) | <span data-ttu-id="46bd8-132">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="46bd8-132">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="46bd8-133">Obtenha a lista de directoryObjects à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="46bd8-133">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="46bd8-134">Atribuir claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="46bd8-134">Assign claimsMappingPolicy</span></span>](../api/serviceprincipal-post-claimsmappingpolicies.md) | <span data-ttu-id="46bd8-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46bd8-135">None</span></span> | <span data-ttu-id="46bd8-136">Atribuir um claimsMappingPolicy a um objeto [servicePrincipalName](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="46bd8-136">Assign a claimsMappingPolicy to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="46bd8-137">Lista atribuída claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="46bd8-137">List assigned claimsMappingPolicy</span></span>](../api/serviceprincipal-list-claimsmappingpolicies.md) | <span data-ttu-id="46bd8-138">Conjunto [claimsMappingPolicy](claimsmappingpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="46bd8-138">[claimsMappingPolicy](claimsmappingpolicy.md) collection</span></span> | <span data-ttu-id="46bd8-139">Lista os objetos claimsMappingPolicy que são atribuídos a um objeto [servicePrincipalName](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="46bd8-139">List the claimsMappingPolicy objects that are assigned to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="46bd8-140">Remover claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="46bd8-140">Remove claimsMappingPolicy</span></span>](../api/serviceprincipal-delete-claimsmappingpolicies.md) | <span data-ttu-id="46bd8-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46bd8-141">None</span></span> | <span data-ttu-id="46bd8-142">Remover um claimsMappingPolicy de um objeto [servicePrincipalName](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="46bd8-142">Remove a claimsMappingPolicy from a [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="46bd8-143">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46bd8-143">Properties</span></span>

| <span data-ttu-id="46bd8-144">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46bd8-144">Property</span></span>     | <span data-ttu-id="46bd8-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="46bd8-145">Type</span></span>        | <span data-ttu-id="46bd8-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="46bd8-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="46bd8-147">id</span><span class="sxs-lookup"><span data-stu-id="46bd8-147">id</span></span>|<span data-ttu-id="46bd8-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46bd8-148">String</span></span>| <span data-ttu-id="46bd8-149">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="46bd8-149">Unique identifier for this policy.</span></span> <span data-ttu-id="46bd8-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46bd8-150">Read-only.</span></span>|
|<span data-ttu-id="46bd8-151">definir</span><span class="sxs-lookup"><span data-stu-id="46bd8-151">definition</span></span>|<span data-ttu-id="46bd8-152">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="46bd8-152">String collection</span></span>| <span data-ttu-id="46bd8-153">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="46bd8-153">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="46bd8-154">Veja mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="46bd8-154">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="46bd8-155">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46bd8-155">Required.</span></span>|
|<span data-ttu-id="46bd8-156">description</span><span class="sxs-lookup"><span data-stu-id="46bd8-156">description</span></span>|<span data-ttu-id="46bd8-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46bd8-157">String</span></span>| <span data-ttu-id="46bd8-158">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="46bd8-158">Description for this policy.</span></span>|
|<span data-ttu-id="46bd8-159">displayName</span><span class="sxs-lookup"><span data-stu-id="46bd8-159">displayName</span></span>|<span data-ttu-id="46bd8-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46bd8-160">String</span></span>| <span data-ttu-id="46bd8-161">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="46bd8-161">Display name for this policy.</span></span> <span data-ttu-id="46bd8-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46bd8-162">Required.</span></span>|
|<span data-ttu-id="46bd8-163">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="46bd8-163">isOrganizationDefault</span></span>|<span data-ttu-id="46bd8-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="46bd8-164">Boolean</span></span>|<span data-ttu-id="46bd8-165">Ignore essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="46bd8-165">Ignore this property.</span></span> <span data-ttu-id="46bd8-166">A política de mapeamento de declarações só pode ser aplicada a entidades de serviço e não pode ser definida globalmente para a organização.</span><span class="sxs-lookup"><span data-stu-id="46bd8-166">The claims-mapping policy can only be applied to service principals and can't be set globally for the organization.</span></span>|

### <a name="properties-of-a-claims-mapping-policy-definition"></a><span data-ttu-id="46bd8-167">Propriedades de uma definição de política de mapeamento de declarações</span><span class="sxs-lookup"><span data-stu-id="46bd8-167">Properties of a claims-mapping policy definition</span></span>

<span data-ttu-id="46bd8-168">As propriedades abaixo formam o objeto JSON que representa uma política de mapeamento de declarações.</span><span class="sxs-lookup"><span data-stu-id="46bd8-168">The properties below form the JSON object that represents a claims-mapping policy.</span></span> <span data-ttu-id="46bd8-169">Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** .</span><span class="sxs-lookup"><span data-stu-id="46bd8-169">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="46bd8-170">Alguns exemplos de definição são mostrados abaixo:</span><span class="sxs-lookup"><span data-stu-id="46bd8-170">A few definition examples are shown below:</span></span>

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a><span data-ttu-id="46bd8-171">Exemplo: **definição** para incluir o EmployeeID e TenantCountry como declarações em tokens</span><span class="sxs-lookup"><span data-stu-id="46bd8-171">Example: **definition** to include the EmployeeID and TenantCountry as claims in tokens</span></span>
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

#### <a name="example-definition-that-uses-a-claims-transformation"></a><span data-ttu-id="46bd8-172">Exemplo: **definição** que usa uma transformação de declarações</span><span class="sxs-lookup"><span data-stu-id="46bd8-172">Example: **definition** that uses a claims transformation</span></span>
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

| <span data-ttu-id="46bd8-173">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46bd8-173">Property</span></span>     | <span data-ttu-id="46bd8-174">Tipo</span><span class="sxs-lookup"><span data-stu-id="46bd8-174">Type</span></span>   |<span data-ttu-id="46bd8-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="46bd8-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46bd8-176">Versão</span><span class="sxs-lookup"><span data-stu-id="46bd8-176">Version</span></span>|<span data-ttu-id="46bd8-177">Inteiro</span><span class="sxs-lookup"><span data-stu-id="46bd8-177">Integer</span></span>|<span data-ttu-id="46bd8-178">Defina o valor 1.</span><span class="sxs-lookup"><span data-stu-id="46bd8-178">Set value of 1.</span></span> <span data-ttu-id="46bd8-179">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46bd8-179">Required.</span></span>|
|<span data-ttu-id="46bd8-180">IncludeBasicClaimSet</span><span class="sxs-lookup"><span data-stu-id="46bd8-180">IncludeBasicClaimSet</span></span>|<span data-ttu-id="46bd8-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="46bd8-181">Boolean</span></span>|<span data-ttu-id="46bd8-182">Se for definido como true, todas as declarações no conjunto de declarações básicas serão emitidas em tokens afetados pela política.</span><span class="sxs-lookup"><span data-stu-id="46bd8-182">If set to true, all claims in the basic claim set are emitted in tokens affected by the policy.</span></span> <span data-ttu-id="46bd8-183">Se definido como false, as declarações no conjunto de declarações básicas não estão nos tokens, a menos que sejam individualmente adicionadas à propriedade ClaimsSchema da mesma política.</span><span class="sxs-lookup"><span data-stu-id="46bd8-183">If set to false, claims in the basic claim set are not in the tokens, unless they are individually added in the ClaimsSchema property of the same policy.</span></span>|
|<span data-ttu-id="46bd8-184">ClaimsSchema</span><span class="sxs-lookup"><span data-stu-id="46bd8-184">ClaimsSchema</span></span>|<span data-ttu-id="46bd8-185">Objeto JSON</span><span class="sxs-lookup"><span data-stu-id="46bd8-185">JSON object</span></span>|<span data-ttu-id="46bd8-186">Define quais declarações estão presentes nos tokens afetados pela política, além do conjunto de declarações básico e o conjunto de declarações principal.</span><span class="sxs-lookup"><span data-stu-id="46bd8-186">Defines which claims are present in the tokens affected by the policy, in addition to the basic claim set and the core claim set.</span></span> <span data-ttu-id="46bd8-187">Para cada entrada de esquema de declaração definida nessa propriedade, determinadas informações são necessárias.</span><span class="sxs-lookup"><span data-stu-id="46bd8-187">For each claim schema entry defined in this property, certain information is required.</span></span> <span data-ttu-id="46bd8-188">Especifique onde os dados vêm vindo (par de valor ou código-fonte/ID) e quais declarações os dados são emitidos como (tipo de declaração).</span><span class="sxs-lookup"><span data-stu-id="46bd8-188">Specify where the data is coming from (Value or Source/ID pair), and which claim the data is emitted as (Claim Type).</span></span> <span data-ttu-id="46bd8-189">Mais detalhes estão disponíveis na [definição ClaimsSchema](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span><span class="sxs-lookup"><span data-stu-id="46bd8-189">Further details are available in the [ClaimsSchema definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span></span>|
|<span data-ttu-id="46bd8-190">ClaimsTransformation</span><span class="sxs-lookup"><span data-stu-id="46bd8-190">ClaimsTransformation</span></span>|<span data-ttu-id="46bd8-191">Objeto JSON</span><span class="sxs-lookup"><span data-stu-id="46bd8-191">JSON object</span></span>| <span data-ttu-id="46bd8-192">Define transformações comuns que podem ser aplicadas aos dados de origem, para gerar os dados de saída para declarações especificadas no ClaimsSchema.</span><span class="sxs-lookup"><span data-stu-id="46bd8-192">Defines common transformations that can be applied to source data, to generate the output data for claims specified in the ClaimsSchema.</span></span> <span data-ttu-id="46bd8-193">Mais detalhes estão disponíveis na [definição ClaimsTransformation](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span><span class="sxs-lookup"><span data-stu-id="46bd8-193">Further details are available in the [ClaimsTransformation definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span></span>|


## <a name="relationships"></a><span data-ttu-id="46bd8-194">Relações</span><span class="sxs-lookup"><span data-stu-id="46bd8-194">Relationships</span></span>

| <span data-ttu-id="46bd8-195">Relação</span><span class="sxs-lookup"><span data-stu-id="46bd8-195">Relationship</span></span> | <span data-ttu-id="46bd8-196">Tipo</span><span class="sxs-lookup"><span data-stu-id="46bd8-196">Type</span></span>        | <span data-ttu-id="46bd8-197">Descrição</span><span class="sxs-lookup"><span data-stu-id="46bd8-197">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="46bd8-198">appliesTo</span><span class="sxs-lookup"><span data-stu-id="46bd8-198">appliesTo</span></span>|<span data-ttu-id="46bd8-199">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="46bd8-199">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="46bd8-200">A coleção [directoryobject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="46bd8-200">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="46bd8-201">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46bd8-201">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="46bd8-202">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46bd8-202">JSON representation</span></span>

<span data-ttu-id="46bd8-203">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="46bd8-203">The following is a JSON representation of the resource.</span></span>

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